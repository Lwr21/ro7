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
background:linear-gradient(rgba(0,0,0,.7),rgba(0,0,0,.7)),url("https://cdn.discordapp.com/attachments/1489628491602202674/1515867736645828728/content.png?ex=6a309157&is=6a2f3fd7&hm=027d692e48a18ed56d4fe1a0658f02f3d7a0db090b0875e648f4123ce068e6a5&" />
') center/cover}
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
<div class="card">
1- احترام الجميع<br>
2- يمنع الغش<br>
3- يمنع استغلال الثغرات<br>
4- يمنع السب والشتم<br>
5- الالتزام بقرارات الإدارة
</div>
</section>

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
<input placeholder="اسمك">
<input placeholder="العمر">
<input placeholder="الدسكورد">
<textarea placeholder="لماذا تريد الانضمام للإدارة؟"></textarea>
<button type="submit">إرسال الطلب</button>
</form>
</div>
</section>

<section id="shop" class="reveal">
<h2>المتجر</h2>
<div class="grid">
<div class="card"><h3>Bronze</h3><p>الباقة البرونزية</p></div>
<div class="card"><h3>Silver</h3><p>الباقة الفضية</p></div>
<div class="card"><h3>Gold</h3><p>الباقة الذهبية</p></div>
<div class="card"><h3>Diamond</h3><p>الباقة الماسية</p></div>
</div>
</section>

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

<section>
<h2>الإدارة</h2>

<div class="card">
<h3>Lwr Rio M4 jizan 3bo MFLM Rakan </h3>
<p> </p>
</div>
</section>

