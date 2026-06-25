<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>دعوة زفاف هيثم & سميحة</title>

<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Cairo',sans-serif;
}

body{
background:#f5efe6;
color:#4a3f35;
overflow-x:hidden;
}

.hero{
min-height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
background:linear-gradient(rgba(245,239,230,.9),rgba(245,239,230,.95));
}

.bismillah{
font-size:22px;
margin-bottom:25px;
color:#8b6b3f;
}

.names{
font-size:58px;
font-weight:700;
color:#9c7a45;
margin-bottom:10px;
}

.subtitle{
font-size:22px;
margin-bottom:35px;
}

.details{
font-size:20px;
line-height:2;
margin-bottom:30px;
}

.countdown{
display:flex;
gap:15px;
margin:25px 0;
flex-wrap:wrap;
justify-content:center;
}

.box{
background:white;
padding:18px;
border-radius:16px;
min-width:90px;
box-shadow:0 4px 15px rgba(0,0,0,.08);
}

.box span{
display:block;
font-size:30px;
font-weight:bold;
color:#9c7a45;
}

.buttons{
display:flex;
gap:15px;
flex-wrap:wrap;
justify-content:center;
margin-top:25px;
}

.btn{
text-decoration:none;
padding:14px 28px;
border-radius:50px;
font-weight:bold;
transition:.3s;
}

.location{
background:#9c7a45;
color:white;
}

.whatsapp{
background:#25D366;
color:white;
}

.btn:hover{
transform:translateY(-3px);
}

.invitation{
max-width:850px;
margin:auto;
padding:60px 25px;
text-align:center;
line-height:2.2;
font-size:20px;
}

.footer{
padding:40px;
text-align:center;
color:#8b6b3f;
font-size:18px;
}

.gold-line{
width:120px;
height:2px;
background:#c9a86a;
margin:20px auto;
}

@media(max-width:768px){
.names{
font-size:42px;
}
.subtitle{
font-size:18px;
}
}
</style>
</head>

<body>

<section class="hero">

<div class="bismillah">
بسم الله الرحمن الرحيم
</div>

<div class="names">
هيثم & سميحة
</div>

<div class="gold-line"></div>

<div class="subtitle">
يسرّنا دعوتكم لمشاركتنا فرحة زفافنا
</div>

<div class="details">
📅 الخميس 6 أغسطس 2026<br>
🕗 الساعة 8:00 مساءً<br>
📍 قاعة الحزم
</div>

<div class="countdown">
<div class="box">
<span id="days">0</span>
أيام
</div>

<div class="box">
<span id="hours">0</span>
ساعات
</div>

<div class="box">
<span id="minutes">0</span>
دقائق
</div>

<div class="box">
<span id="seconds">0</span>
ثوانٍ
</div>
</div>

<div class="buttons">

<a class="btn location"
href="https://maps.app.goo.gl/cBemcmBSQ8WtMWLw5?g_st=ic"
target="_blank">
📍 موقع الحفل
</a>

<a class="btn whatsapp"
href="https://wa.me/96893991107?text=السلام%20عليكم،%20أؤكد%20حضوري%20لحفل%20زفاف%20هيثم%20وسميحة"
target="_blank">
💬 تأكيد الحضور
</a>

</div>

</section>

<section class="invitation">

<p>
﴿ وَمِنْ آيَاتِهِ أَنْ خَلَقَ لَكُم مِّنْ أَنفُسِكُمْ أَزْوَاجًا
لِّتَسْكُنُوا إِلَيْهَا وَجَعَلَ بَيْنَكُم مَّوَدَّةً وَرَحْمَةً ﴾
</p>

<br>

<p>
بكل الحب والفرح، نتشرف بحضوركم ومشاركتكم أجمل لحظات حياتنا،
لنحتفل معًا بليلة زفافنا، فوجودكم يزيد فرحتنا بهجة وسرورًا.
</p>

</section>

<div class="footer">
ننتظر حضوركم بكل شوق ❤️
</div>

<script>

const weddingDate = new Date("August 6, 2026 20:00:00").getTime();

setInterval(() => {

const now = new Date().getTime();
const distance = weddingDate - now;

const days = Math.floor(distance / (1000 * 60 * 60 * 24));
const hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
const minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
const seconds = Math.floor((distance % (1000 * 60)) / 1000);

document.getElementById("days").innerHTML = days;
document.getElementById("hours").innerHTML = hours;
document.getElementById("minutes").innerHTML = minutes;
document.getElementById("seconds").innerHTML = seconds;

},1000);

</script>

</body>
</html>