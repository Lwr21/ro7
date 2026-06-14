const express = require("express");
const session = require("express-session");
const axios = require("axios");
require("dotenv").config();

const app = express();

app.use(session({
  secret: "secret123",
  resave: false,
  saveUninitialized: false
}));

app.get("/", (req, res) => {
  if (!req.session.user) {
    return res.send(`
      <h1>Discord Login</h1>
      <a href="/login">
        <button>تسجيل دخول ديسكورد</button>
      </a>
    `);
  }

  res.send(`
    <h1>مرحبا ${req.session.user.username}</h1>
    <p>ID: ${req.session.user.id}</p>
    <a href="/dashboard">الدخول للداشبورد</a><br><br>
    <a href="/logout">تسجيل خروج</a>
  `);
});

// رابط تسجيل الدخول
app.get("/login", (req, res) => {
  const CLIENT_ID = process.env.DISCORD_CLIENT_ID;
  const REDIRECT = process.env.DISCORD_REDIRECT;

  const url = `https://discord.com/oauth2/authorize?client_id=${CLIENT_ID}&redirect_uri=${encodeURIComponent(REDIRECT)}&response_type=code&scope=identify`;

  res.redirect(url);
});

// كول باك ديسكورد
app.get("/callback", async (req, res) => {
  const code = req.query.code;

  try {
    const tokenRes = await axios.post(
      "https://discord.com/api/oauth2/token",
      new URLSearchParams({
        client_id: process.env.DISCORD_CLIENT_ID,
        client_secret: process.env.DISCORD_CLIENT_SECRET,
        grant_type: "authorization_code",
        code,
        redirect_uri: process.env.DISCORD_REDIRECT
      }),
      {
        headers: {
          "Content-Type": "application/x-www-form-urlencoded"
        }
      }
    );

    const userRes = await axios.get("https://discord.com/api/users/@me", {
      headers: {
        Authorization: `Bearer ${tokenRes.data.access_token}`
      }
    });

    req.session.user = userRes.data;

    res.redirect("/");
  } catch (err) {
    res.send("خطأ في تسجيل الدخول");
  }
});

// داشبورد
app.get("/dashboard", (req, res) => {
  if (!req.session.user) return res.redirect("/");

  res.send(`
    <h1>Dashboard</h1>
    <p>Welcome ${req.session.user.username}</p>
    <p>Discord ID: ${req.session.user.id}</p>

    <hr>

    <h3>نظام الإدارة (جاهز للتطوير)</h3>
    <ul>
      <li>✔ تسجيل دخول ديسكورد</li>
      <li>⏳ نظام صلاحيات (لاحقاً)</li>
      <li>⏳ ربط FiveM (لاحقاً)</li>
      <li>⏳ لوحة تحكم كاملة</li>
    </ul>

    <a href="/">رجوع</a>
  `);
});

// تسجيل خروج
app.get("/logout", (req, res) => {
  req.session.destroy();
  res.redirect("/");
});

app.listen(3000, () => {
  console.log("Server running on http://localhost:3000");
});
