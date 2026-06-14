<!DOCTYPE html>
<html lang="ar">
<head>
<meta charset="UTF-8">
<title>Ro7 Fight</title>

<style>
body {
  margin: 0;
  font-family: Arial;
  background: #0a0a0a;
  color: white;
}

/* 🔥 الهيرو (الصورة الجديدة) */
.hero {
  height: 100vh;
  background: url('home.png') center/cover no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}

  <a class="btn" href="https://discord.gg/hw2gh5AU">
دخول الدسكورد
</a>
.hero::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.6);
}

.hero-content {
  position: relative;
  text-align: center;
}

.hero h1 {
  font-size: 60px;
  margin: 0;
  color: white;
}

.hero span {
  color: gold;
}

.hero p {
  font-size: 18px;
  margin-top: 10px;
  opacity: 0.8;
}

.btn {
  margin-top: 20px;
  padding: 12px 20px;
  background: gold;
  border: none;
  cursor: pointer;
  font-weight: bold;
}

/* 🔗 الأقسام */
section {
  padding: 50px;
}

.card {
  background: #1c1c1c;
  padding: 20px;
  margin-top: 20px;
  border-radius: 10px;
}
</style>
</head>

<body>

<!-- 🔥 الصورة الرئيسية -->
<div class="hero">
  <div class="hero-content">
    <h1>RO7 <span>FIGHT</span></h1>
    <p>سيرفر فايتات احترافي بإدارة Rio M4</p>
    <button class="btn" onclick="scrollToSection()">ابدأ الآن</button>
  </div>
</div>

<!-- 📌 المعلومات -->
<section id="info">
  <div class="card">
    <h2>عن السيرفر</h2>
    <p>Ro7 Fight هو سيرفر فايتات قوي يقدم نظام قتالات احترافي وتحديات يومية.</p>
  </div>

  <div class="card">
    <h2>Owner</h2>
    <p>Rio M4 👑</p>
  </div>

  <div class="card">
    <h2>القوانين</h2>
    <ul>
      <li>احترام الجميع</li>
      <li>ممنوع الغش</li>
      <li>ممنوع السب</li>
    </ul>
  </div>
</section>

<script>
function scrollToSection(){
  document.getElementById("info").scrollIntoView({behavior:"smooth"});
}
</script>

</body>
</html>
