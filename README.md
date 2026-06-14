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
background:linear-gradient(rgba(0,0,0,.7),rgba(0,0,0,.7)),url('https://images.unsplash.com/photo-1511512578047-dfb367046420') center/cover}
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
<div class="card">**# 📝Server Rules  | قوانين السيرفر



1 . يجب عليك الاحترام بين اللاعبين داخل السيرفر

2 . يُمنع الشخصنة بجميع اشكالها وانواعها

3 . يُمنع تدبيل الحسابات بشكل كامل وعقوبتها باند نهائي

4 . يُمنع منعاً باتاً انتحالك لشخصيه اداريه وانت ليس اداري

5 . يُمنع منعاً باتاً استخدام اي برنامج لرفع البنق بهدف الانتقالات او الخ .. وعقوبتها باند نهائي

6 . يجب عليك تشغيل برنامج التصوير ( 20 د) اثناء اللعب في حال عدم وجوده بيتم محاسبتك

7 . يُمنع استخدام اي اداءة للتحكم ( اللعب) غير الماوس والكيبورد

8 . في حال تفتيشك والعثور على اشياء ممنوعه في جهازك يعرضك للباند بشكل نهائي

9 . يمنع التوكسك بجميع انواعه

10 . يمنع الاسبام في طلب الاداري داخل السيرفر 

11 . يمنع منعا باتا تركب اشياء تعطيك افضليه على لاعب اخر 

# 📝 Playing Rules  | قوانين اللعب




1 . يُمنع لبس الخوذ بجميع انواعها

2 . يُمنع منعاً باتاً استخدام اي قلتش او استخدام ثغره او ملفات او هاك بجميع انواعه ومن يستخدم اياَ منها يعرض نفسه للمخالفة وعقوبتها باند نهائي

3 . يُمنع منعاً باتاً لبس اللبس الجاهز

4 . يُمنع حشر الرسبون



||@everyone|| **
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
<input placeholder="اسمك داخل السيرفر">
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
<div class="card"><h3>Bronze</h3><p></p>ايدي ثنائي من اختيارك سالب = 45 دولار</div>
<div class="card"><h3>Silver</h3><p>ايدي ثلاثي من اختيارك سالب = 25 دولار</p></div>
<div class="card"><h3>Gold</h3><p>رموز القبائل  =  25 دولار
</p></div>
<div class="card"><h3>Diamond</h3><p>الايدي ثنائي مكرر = 30 دولار
</p></div>
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
