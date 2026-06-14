ro7-fight-website/
│
├── server.js
├── package.json
├── .env
│
├── /public
│   ├── index.html
│   ├── rules.html
│   ├── shop.html
│   ├── admin.html
│   ├── style.css
│
└── /views (اختياري لو تبي EJS)
<!DOCTYPE html>
<html>
<head>
  <title>Ro7 Fight</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <header>
    <h1>🔥 Ro7 Fight Server</h1>
    <a href="rules.html">القوانين</a>
    <a href="shop.html">المتجر</a>
    <a href="/auth/discord">تسجيل دخول ديسكورد</a>
  </header>

  <section class="hero">
    <h2>مرحبا بك في سيرفر Ro7 Fight</h2>
    <p>أفضل سيرفر فايت في FiveM</p>
  </section>

</body>
</html>
<h1>📝 Server Rules | قوانين السيرفر</h1>

<h2>Server Rules</h2>
<ul>
<li>يجب عليك الاحترام بين اللاعبين</li>
<li>ممنوع الشخصنة</li>
<li>ممنوع التهكير أو الغش</li>
<li>ممنوع انتحال شخصية إداري</li>
<li>يجب تصوير اللعب</li>
<li>ممنوع التوكسك</li>
</ul>

<h2>Playing Rules</h2>
<ul>
<li>ممنوع الهكر بجميع أنواعه</li>
<li>ممنوع اللبس الجاهز</li>
<li>ممنوع استخدام القلتشات</li>
</ul>

<h1>🛒 متجر Ro7 Fight</h1>

<div class="item">
  <h3>ايدي ثنائي سالب</h3>
  <p>45 دولار</p>
</div>

<div class="item">
  <h3>ايدي ثلاثي سالب</h3>
  <p>25 دولار</p>
</div>

<div class="item">
  <h3>رموز القبائل</h3>
  <p>25 دولار</p>
</div>

<p>للطلب: افتح تكت في ديسكورد</p>

body {
  background: #0f0f0f;
  color: white;
  font-family: Arial;
  text-align: center;
}

header {
  background: #111;
  padding: 20px;
}

a {
  color: gold;
  margin: 10px;
  text-decoration: none;
}

.item {
  background: #1c1c1c;
  margin: 10px;
  padding: 10px;
  border-radius: 10px;
}

const express = require("express");
const app = express();

app.use(express.static("public"));

app.get("/", (req, res) => {
  res.sendFile(__dirname + "/public/index.html");
});

app.listen(3000, () => {
  console.log("Server running on port 3000");
});

