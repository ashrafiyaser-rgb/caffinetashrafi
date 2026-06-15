<DOCTYPE html>
<html lang="fa" dir="rtl">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>کافی نت اشرفی</title>

<link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;700&display=swap" rel="stylesheet">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Vazirmatn',sans-serif;
}

body{
background:
linear-gradient(
135deg,
#4fc3f7 0%,
#26c6da 45%,
#ffe082 100%
);

min-height:100vh;
display:flex;
justify-content:center;
align-items:center;
overflow-x:hidden;
position:relative;
}

.sun{
position:fixed;
top:25px;
right:25px;
width:90px;
height:90px;
border-radius:50%;
background:#FFD54F;

box-shadow:
0 0 25px #FFD54F,
0 0 50px #FFD54F,
0 0 80px #FFD54F;

animation:sunPulse 4s infinite;
z-index:1;
}

@keyframes sunPulse{

0%{transform:scale(1);}
50%{transform:scale(1.08);}
100%{transform:scale(1);}

}

.wave{
position:fixed;
bottom:0;
left:0;

width:200%;
height:140px;

background:
rgba(255,255,255,.35);

border-radius:
100% 100% 0 0;

animation:
waveMove 12s linear infinite;

z-index:0;
}

.wave2{
bottom:25px;
opacity:.25;
animation-duration:18s;
}

@keyframes waveMove{

from{
transform:translateX(0);
}

to{
transform:translateX(-50%);
}

}

.card{

width:390px;
max-width:95vw;

padding:30px;

border-radius:28px;

background:
rgba(255,255,255,.18);

backdrop-filter:blur(14px);

border:
1px solid rgba(255,255,255,.30);

box-shadow:
0 10px 40px rgba(0,0,0,.18);

position:relative;

z-index:5;

}

.msg1{

font-size:28px;
font-weight:700;

text-align:center;

color:#004d40;

margin-bottom:12px;

}

.msg2{

text-align:center;
color:#00695c;

font-size:15px;

margin-bottom:10px;

}

.msg3{

text-align:center;

line-height:2;

font-size:14px;

margin-bottom:10px;

}

.msg4{

text-align:center;

font-size:13px;

color:#c62828;

margin-bottom:20px;

}

.links-container{

display:flex;

flex-wrap:wrap;

gap:10px;

justify-content:space-between;

}

.link-box{

flex:1 1 calc(50% - 10px);

padding:14px;

border-radius:18px;

text-align:center;

text-decoration:none;

cursor:pointer;

color:#fff;

font-size:14px;

font-weight:500;

transition:.25s;

box-shadow:
0 6px 15px rgba(0,0,0,.15);

user-select:none;

}

.link-box:hover{

transform:
translateY(-4px)
scale(1.03);

}

.service-item{

background:
linear-gradient(
135deg,
#ff9800,
#f57c00
);

}

.back-btn{

flex-basis:100% !important;

background:
linear-gradient(
135deg,
#7e57c2,
#5e35b1
) !important;

}

.hidden{

display:none !important;

}

.modal{

position:fixed;

inset:0;

background:
rgba(0,0,0,.55);

display:flex;

justify-content:center;

align-items:center;

z-index:9999;

}

.modal-content{

width:320px;

background:#fff;

padding:20px;

border-radius:20px;

text-align:center;

}

.modal-btn{

padding:10px 20px;

border:none;

border-radius:12px;

cursor:pointer;

margin:5px;

}

.btn-yes{

background:#2ecc71;
color:#fff;

}

.btn-no{

background:#e74c3c;
color:#fff;

}

.call-btn{

position:fixed;

left:20px;
bottom:20px;

width:60px;
height:60px;

border-radius:50%;

.btn-yes{
background:#2ecc71;
color:#fff;
}

.btn-no{
background:#e74c3c;
color:#fff;
}

.hidden{
display:none !important;
}

background:#25D366;

display:flex;

justify-content:center;
align-items:center;

color:#fff;

font-size:24px;

text-decoration:none;

z-index:999;

box-shadow:
0 6px 20px rgba(0,0,0,.25);

}

</style>

</head>

<body>

<!-- خورشید -->
<div class="sun"></div>

<!-- موج ها -->
<div class="wave"></div>
<div class="wave wave2"></div>

<!-- تماس سریع -->
<a
class="call-btn"
href="tel:+989309166187">

<i class="fa-solid fa-phone"></i>

</a>

<!-- کارت اصلی -->

<div class="card">

<div id="messages">

<div class="msg1">

کافی نت دیجیتال
</div>

<div class="msg2">

خدمات اینترنتی، اداری، ملکی و نرم افزاری

</div>

<div class="msg3">

به کافی نت دیجیتال خوش آمدید

<br>

لطفاً یکی از گزینه‌های زیر را انتخاب کنید

</div>

<div class="msg4">

ارسال خودکار درخواست فقط از طریق
واتساپ و تلگرام امکان پذیر است

</div>

</div>

<!-- منوی اصلی -->

<div
id="main-menu"
class="links-container">

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#ff9800,
#fb8c00
);"
href="javascript:void(0)"
onclick="showPage('services')">

<i class="fa-solid fa-screwdriver-wrench"></i>

<br>

خدمات

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#00acc1,
#00838f
);"
href="javascript:void(0)"
onclick="showPage('contacts')">

<i class="fa-solid fa-address-book"></i>

<br>

لینک های ارتباطی

</a>

</div>

<!-- صفحه خدمات -->

<div
id="services"
class="links-container hidden">

<div class="link-box service-item">
📄 اسکن مدارک
</div>

<div class="link-box service-item">
📋 کپی رنگی و سیاه و سفید
</div>

<div class="link-box service-item">
🌐 انواع ثبت نام های اینترنتی
</div>

<div class="link-box service-item">
📨 ابلاغیه الکترونیکی
</div>

<div class="link-box service-item">
💳 چک صیادی
</div>

<div class="link-box service-item">
⚖️ گواهی عدم سوء پیشینه
</div>

<div class="link-box service-item">
🚘 نوبت گیری تعویض پلاک
</div>

<div class="link-box service-item">
🏛️ اظهارنامه مالیاتی
</div>

<div class="link-box service-item">
👶 وام ازدواج و فرزندآوری
</div>

<div class="link-box service-item">
📑 سوابق تامین اجتماعی
</div>

<div class="link-box service-item">
📚 صحافی و فنر زنی
</div>

<div class="link-box service-item">
📝 طراحی انواع فرم
</div>

<div class="link-box service-item">
📮 تاییدیه کد پستی
</div>

<div class="link-box service-item">
🪪 سخا
</div>

<div class="link-box service-item">
💻 نصب ویندوز و برنامه های کاربردی
</div>

<div class="link-box service-item">
🏠 ثبت اقامتگاه سامانه املاک و اسکان
</div>

<div class="link-box service-item">
📊 ساخت نرم افزارهای حسابداری تحت اکسل
</div>

<div class="link-box service-item">
🌍 ساخت نرم افزارهای حسابداری تحت وب
</div>

<div class="link-box service-item">
📑 ثبت نام قرارداد فروش و اجاره و دریافت کد رهگیری
</div>

<div class="link-box service-item">
🏡 ثبت نام وام ودیعه مسکن
</div>

<div class="link-box service-item">
💰 خرید و فروش وام امتیازی
</div>

<div class="link-box service-item">
🚗 خرید و فروش حواله خودرو
</div>

<div class="link-box service-item">
🧑‍💻 طراحی و ساخت انواع نرم افزار حسابداری و مدیریتی کاملاً شخصی و متناسب با سلیقه شما
</div>

<a
class="link-box back-btn"
href="javascript:void(0)"
onclick="showPage('main-menu')">

<i class="fa-solid fa-arrow-right"></i>

بازگشت

</a>
</div>

<!-- صفحه ارتباطی -->

<div
id="contacts"
class="links-container hidden">

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#25D366,
#128C7E
);"
href="javascript:void(0)"
onclick="openWhatsApp()">

<i class="fab fa-whatsapp"></i>

<br>

واتساپ

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#229ED9,
#0088cc
);"
href="javascript:void(0)"
onclick="openTelegram()">

<i class="fab fa-telegram"></i>

<br>

تلگرام

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#6a1b9a,
#8e24aa
);"
href="https://rubika.ir/ashrafi_c_net"
target="_blank">

📱

<br>

روبیکا

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#1565c0,
#1976d2
);"
href="https://ble.ir/ashrafi_c_net"
target="_blank">

💬

<br>

بله

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#ef6c00,
#fb8c00
);"
href="https://eitaa.com/ashrafi_c_net"
target="_blank">

📨

<br>

ایتا

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#00acc1,
#0097a7
);"
href="https://sapp.ir/ashrafi_c_net"
target="_blank">

✉️

<br>

سروش

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#3949ab,
#5c6bc0
);"
href="https://shad.ir/prfcxe5593"
target="_blank">

🎓

<br>

شاد

</a>

<a
class="link-box"
style="
background:
linear-gradient(
135deg,
#e53935,
#d32f2f
);"
href="https://maps.google.com/maps?q=37.51278296507102,45.06070375442505&z=17"
target="_blank">

<i class="fa-solid fa-location-dot"></i>

<br>

مسیریابی

</a>

<a
class="link-box back-btn"
href="javascript:void(0)"
onclick="showPage('main-menu')">

<i class="fa-solid fa-arrow-right"></i>

بازگشت

</a>
</div>

</div>

<!-- مودال درخواست -->

<div
id="requestModal"
class="modal hidden">

<div class="modal-content">

<h3>

ارسال درخواست

</h3>

<p id="serviceName"></p>

<p>

آیا مایل به ثبت درخواست هستید؟

</p>

<button
class="modal-btn btn-yes"
onclick="goToContacts()">

بله

</button>

<button
class="modal-btn btn-no"
onclick="closeModal()">

خیر

</button>

</div>

</div>

<script>

/* ==========================
   متغیر خدمت انتخاب شده
========================== */

let selectedService = '';

/* ==========================
   نمایش صفحات
========================== */

function showPage(id){

const pages = [
'main-menu',
'services',
'contacts'
];

pages.forEach(page => {

document
.getElementById(page)
.classList
.add('hidden');

});

document
.getElementById(id)
.classList
.remove('hidden');

}

/* ==========================
   باز کردن مودال
========================== */

function openRequest(serviceName){

selectedService = serviceName;

document
.getElementById('serviceName')
.innerHTML =
'<strong>' +
serviceName +
'</strong>';

document
.getElementById('requestModal')
.classList
.remove('hidden');

}

/* ==========================
   بستن مودال
========================== */

function closeModal(){

document
.getElementById('requestModal')
.classList
.add('hidden');

}

/* ==========================
   رفتن به ارتباطی
========================== */

function goToContacts(){

closeModal();

showPage('contacts');

}

/* ==========================
   اتصال کلیک خدمات
========================== */

document
.querySelectorAll('.service-item')
.forEach(item => {

item.addEventListener(
'click',
function(){

openRequest(
this.innerText.trim()
);

}
);

});

/* ==========================
   متن درخواست
========================== */

function getRequestText(){

return `سلام

درخواست من برای خدمت زیر است:

${selectedService}

لطفاً راهنمایی فرمایید.

با تشکر`;

}

/* ==========================
   واتساپ
========================== */

function openWhatsApp(){

if(selectedService === ''){

alert(
'ابتدا از بخش خدمات، خدمت مورد نظر را انتخاب کنید.'
);

return;

}

const text =
encodeURIComponent(
getRequestText()
);

window.open(

'https://wa.me/989309166187?text=' + text,

'_blank'

);

}

/* ==========================
   تلگرام
========================== */

function openTelegram(){

if(selectedService === ''){

alert(
'ابتدا از بخش خدمات، خدمت مورد نظر را انتخاب کنید.'
);

return;

}

const text =
getRequestText();

if(navigator.clipboard){

navigator.clipboard
.writeText(text)
.then(() => {

alert(
'متن درخواست کپی شد.\nپس از ورود به تلگرام آن را Paste کنید.'
);

window.open(
'https://t.me/ashrafi_c_net',
'_blank'
);

});

}else{

window.open(
'https://t.me/ashrafi_c_net',
'_blank'
);

}

}

/* ==========================
   صفحه پیش فرض
========================== */

showPage('main-menu');

</script>

</body>
</html>
