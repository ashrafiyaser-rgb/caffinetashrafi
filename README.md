
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <title>کارت ویزیت من</title>
  <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* ===== تم زمستانی ===== */
    body{
      font-family:'Vazirmatn', sans-serif;
      background:
        radial-gradient(circle at 20% 20%, rgba(255,255,255,.35), transparent 40%),
        radial-gradient(circle at 80% 30%, rgba(255,255,255,.25), transparent 45%),
        linear-gradient(135deg,#0f2027,#203a43,#2c5364);
      display:flex;
      justify-content:center;
      align-items:center;
      height:100vh;
      margin:0;
      color:#222;
    }

    .card{
      background:rgba(255,255,255,.95);
      padding:30px;
      border-radius:22px;
      box-shadow:0 15px 35px rgba(0,0,0,.25);
      text-align:center;
      width:370px;
      backdrop-filter: blur(4px);
    }

    /* پیام‌ها */
    .msg1{ font-weight:700; margin-bottom:12px; color:#0f3c5f; font-size:20px; }
    .msg2{ font-size:14px; color:#0b8457; margin-bottom:10px; }
    .msg3{ font-size:14px; margin-bottom:10px; color:#333; }
    .msg4{ font-size:13px; color:#c0392b; margin-bottom:16px; }

    /* لینک‌ها */
    .links-container{
      display:flex;
      flex-wrap:wrap;
      gap:10px;
      justify-content:space-between;
    }

    .link-box{
      flex:1 1 calc(50% - 10px);
      padding:13px;
      border-radius:18px;
      color:#fff;
      text-decoration:none;
      font-size:14px;
      box-shadow:0 6px 12px rgba(0,0,0,.18);
      transition:.2s ease;
      background:linear-gradient(135deg,#3a7bd5,#00d2ff);
    }

    .link-box:hover{
      transform:translateY(-3px) scale(1.02);
      filter:brightness(1.08);
    }

    /* رنگ‌بندی خدمات */
    #services .link-box:nth-child(odd){
      background:linear-gradient(135deg,#1e3c72,#2a5298);
    }
    #services .link-box:nth-child(even){
      background:linear-gradient(135deg,#4ca1af,#2c3e50);
    }

    /* دکمه بازگشت */
    .back-btn{
      flex:1 1 100% !important;
      background:linear-gradient(135deg,#667eea,#764ba2) !important;
      font-weight:600;
    }

    .hidden{ display:none !important; }

    /* انیمیشن */
    .enter{
      animation:fadeIn .35s ease both;
    }
    @keyframes fadeIn{
      from{opacity:0; transform:translateY(15px);}
      to{opacity:1; transform:none;}
    }

    @media(max-width:420px){
      .card{width:92vw; padding:22px;}
    }
    /* ===== افکت برف متحرک ===== */
.snowflake{
  position: fixed;
  top: -10px;
  color: #fff;
  font-size: 14px;
  user-select: none;
  pointer-events: none;
  z-index: 9999;
  opacity: .8;
  animation-name: fall;
  animation-timing-function: linear;
}

@keyframes fall{
  to{
    transform: translateY(110vh);
  }
}
  </style>
</head>

<body>
<div class="card">

  <div id="messages">
    <div class="msg1">کافی نت اشرفی </div>
    <div class="msg2">از حسن توجه شما سپاسگزاریم</div>
    <div class="msg3">لطفاً یکی از گزینه‌های زیر را انتخاب کنید</div>
    <div class="msg4">برای تلگرام فیلترشکن لازم است</div>
  </div>

  <!-- منوی اصلی -->
  <div id="main-menu" class="links-container">
    <a class="link-box" href="javascript:void(0)" onclick="showPage('services')">خدمات</a>
    <a class="link-box" href="javascript:void(0)" onclick="showPage('contacts')">لینک‌های ارتباطی</a>
  </div>

  <!-- خدمات -->
  <div id="services" class="links-container hidden">
    <div class="link-box">پرینت رنگی و سیاه و سفید</div>
    <div class="link-box">اسکن مدارک</div>
    <div class="link-box">کپی رنگی و سیاه و سفید</div>
    <div class="link-box">انواع ثبت‌نام‌های اینترنتی</div>
    <div class="link-box">ابلاغیه الکترونیکی</div>
    <div class="link-box">چک صیادی</div>
    <div class="link-box">گواهی عدم سوءپیشینه</div>
    <div class="link-box">نوبت‌گیری تعویض پلاک</div>
    <div class="link-box">اظهارنامه مالیاتی</div>
    <div class="link-box">وام ازدواج و فرزندآوری</div>
    <div class="link-box">سوابق تامین اجتماعی</div>
    <div class="link-box">صحافی و فنر زنی</div>
    <div class="link-box">طراحی انواع فرم</div>
    <div class="link-box">تأییدیه کد پستی</div>
    <div class="link-box">سخا</div>
    <div class="link-box">نصب ویندوز و برنامه‌های کاربردی</div>

    <!-- خدمات جدید -->
    <div class="link-box">ثبت قامتگاه سامانه املاک و اسکان</div>
    <div class="link-box">ساخت نرم‌افزارهای حسابداری تحت اکسل</div>
    <div class="link-box">ساخت نرم‌افزارهای حسابداری تحت وب</div>

    <a class="link-box back-btn" href="javascript:void(0)" onclick="showPage('main-menu')">
      بازگشت
    </a>
  </div>

  <!-- ارتباطی -->
  <div id="contacts" class="links-container hidden">
    <a class="link-box" href="https://rubika.ir/ashrafi_c_net" target="_blank">روبیکا</a>
    <a class="link-box" href="https://ble.ir/ashrafi_c_net" target="_blank">بله</a>
    <a class="link-box" href="https://sapp.ir/ashrafi_c_net" target="_blank">سروش</a>
    <a class="link-box" href="https://shad.ir/prfcxe5593" target="_blank">شاد</a>
    <a class="link-box" href="https://eitaa.com/ashrafi_c_net" target="_blank">ایتا</a>
    <a class="link-box" href="https://t.me/ashrafi_c_net" target="_blank">تلگرام</a>
    <a class="link-box" href="https://wa.me/989309166187" target="_blank">واتساپ</a>
    <a class="link-box" href="tel:+989309166187">تماس تلفنی</a>
    <a class="link-box" href="https://maps.google.com/maps?q=37.51278296507102,45.06070375442505&z=17" target="_blank">مسیریابی</a>

    <a class="link-box back-btn" href="javascript:void(0)" onclick="showPage('main-menu')">
      بازگشت
    </a>
  </div>

</div>

<script>
function showPage(id){
  ['main-menu','services','contacts'].forEach(p=>{
    document.getElementById(p).classList.add('hidden');
  });
  const page=document.getElementById(id);
  page.classList.remove('hidden');
  page.classList.add('enter');

  const msg3=document.querySelector('.msg3');
  const msg4=document.querySelector('.msg4');
  if(id==='services'){
    msg3.style.display='none';
    msg4.style.display='none';
  }else{
    msg3.style.display='';
    msg4.style.display='';
  }
}
</script>
<script>
/* ===== Snow Effect (Continuous) ===== */

function createSnowflake(){
  const snow = document.createElement('div');
  snow.className = 'snowflake';

  // انواع برف
  const snowChars = ['❄','❅','❆'];
  snow.innerHTML = snowChars[Math.floor(Math.random()*snowChars.length)];

  snow.style.left = Math.random() * 100 + 'vw';
  snow.style.fontSize = (10 + Math.random() * 16) + 'px';
  snow.style.animationDuration = (6 + Math.random() * 8) + 's';
  snow.style.opacity = Math.random();

  document.body.appendChild(snow);

  // حذف برف بعد از رسیدن به پایین
  setTimeout(() => {
    snow.remove();
  }, 15000);
}

// تولید مداوم برف
setInterval(createSnowflake, 300); // هر 0.3 ثانیه یک برف

</script>
</body>
</html>
