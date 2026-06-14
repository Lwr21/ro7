<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>RO7 Fight Server</title>
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:Tahoma,sans-serif;background:#000;color:#fff;scroll-behavior:smooth}
nav{position:fixed;top:0;width:100%;background:rgba(0,0,0,.9);padding:15px;z-index:1000;text-align:center}
nav a{color:#fff;text-decoration:none;margin:0 12px}
.hero{height:100vh;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;
background:linear-gradient(rgba(0,0,0,.7),rgba(0,0,0,.7)),url('[https://images.unsplash.com/photo-1511512578047-dfb367046420](https://cdn.discordapp.com/attachments/1471169865330069736/1515848642232188938/home.png?ex=6a307f8f&is=6a2f2e0f&hm=1dc781d8b7421055525423010c1cedfd392bcbd70f2cf8e2b0a336224cf7fa27&)') center/cover}
.hero h1{font-size:5rem}
.hero p{margin:20px;font-size:1.3rem}
.btn{display:inline-block;padding:14px 30px;border:1px solid #fff;border-radius:8px;color:#fff;text-decoration:none;margin:8px}
.btn:hover{background:#fff;color:#000}
section{padding:90px 10%}
h2{text-align:center;margin-bottom:25px}
.card{background:#111;padding:20px;border-radius:12px;margin:15px 0}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:20px}
input,textarea{width:100%;padding:12px;margin:8px 0;background:#000;border:1px solid #333;color:#fff}
button{padding:12px 20px;border:none;border-radius:8px;cursor:pointer}
.reveal{opacity:0;transform:translateY(40px);transition:1s}
.reveal.active{opacity:1;transform:none}
footer{text-align:center;padding:30px;background:#111}
</style>
</head>
<body>

<nav>
<a href="#rules">القوانين</a>
<a href="#staff">الإدارة</a>
<a href="#apply">التقديم</a>
<a href="#shop">المتجر</a>
</nav>

<section class="hero">
<h1>RO7</h1>
<p>أقوى سيرفر فايتات فايف إم</p>
<div>
<a class="btn" href="https://discord.gg/hw2gh5AU">Discord</a>
<a class="btn" href="#">connect 4ozoao</a>
</div>
</section>

<section id="rules" class="reveal">
<h2>القوانين</h2>
<div class="card"><h1>📝 Server Rules | قوانين السيرفر</h1>

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

<section id="staff" class="reveal">
<h2>الإدارة</h2>
<div class="grid">
<div class="card"><h3>Owner</h3><p>Rio</p></div>
<div class="card"><h3>Owner</h3><p>M4</p></div>
</div>
</section>

<section id="apply" class="reveal">
<h2>التقديم للإدارة</h2>
<div class="card">
<form>
<input placeholder="اسمك ">
<input placeholder="العمر">
<input placeholder="الدسكورد">
<textarea placeholder="لماذا تريد الانضمام للإدارة؟"></textarea>
<button type="submit">إرسال الطلب</button>
</form>
</div>
</section>

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

<footer>
RO7 Fight Server © 2026
</footer>

<script>
const reveals=document.querySelectorAll('.reveal');
window.addEventListener('scroll',()=>{
reveals.forEach(el=>{
const top=el.getBoundingClientRect().top;
if(top<window.innerHeight-100){el.classList.add('active');}
});
});
</script>
</body>
</html>
