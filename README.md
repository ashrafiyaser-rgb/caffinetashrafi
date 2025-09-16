
<html lang="fa">
<head>
  <meta charset="UTF-8">
  <title>کارت ویزیت من</title>
  <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* پایه */
    body{
      font-family: 'Vazirmatn', sans-serif;
      background: linear-gradient(135deg,#74ebd5,#ACB6E5);
      display:flex;
      justify-content:center;
      align-items:center;
      height:100vh;
      margin:0;
    }
    .card{
      background:white;
      padding:30px;
      border-radius:20px;
      box-shadow:0 10px 25px rgba(0,0,0,0.15);
      text-align:center;
      width:360px;
      overflow:hidden;
    }

    /* پیام‌ها */
    .msg1{ font-weight:700; margin-bottom:12px; color:#222; }
    .msg2{ font-size:14px; color:green; margin-bottom:10px; }
    .msg3{ font-size:14px; margin-bottom:10px; color:#333; }
    .msg4{ font-size:13px; color:red; margin-bottom:16px; }

    /* کانتینر لینک‌ها (دو ستون) */
    .links-container{
      display:flex;
      flex-wrap:wrap;
      gap:10px;
      justify-content:space-between;
    }
    .link-box{
      flex:1 1 calc(50% - 10px);
      padding:12px;
      border-radius:18px;
      color:#fff;
      text-decoration:none;
      font-size:15px;
      box-shadow:0 4px 8px rgba(0,0,0,0.12);
      text-align:center;
      transition: transform .18s ease, filter .18s ease;
      white-space:normal;
      line-height:1.4;
      display:block;
      background:#2b6ef6; /* پیش‌فرض رنگ آبی تیره برای خوانایی در صفحه اصلی */
    }
    .link-box:hover{ transform:translateY(-3px); filter:brightness(1.08); }

    /* رنگ‌های مخصوص صفحه خدمات (رنگارنگ) */
    #services .link-box:nth-child(1){ background:#3498db; }  /* آبی */
    #services .link-box:nth-child(2){ background:#9b59b6; }  /* بنفش */
    #services .link-box:nth-child(3){ background:#e67e22; }  /* نارنجی */
    #services .link-box:nth-child(4){ background:#1abc9c; }  /* سبزآبی */
    #services .link-box:nth-child(5){ background:#f39c12; }  /* زرد نارنجی */
    #services .link-box:nth-child(6){ background:#d35400; }  /* نارنجی تیره */
    #services .link-box:nth-child(7){ background:#2ecc71; }  /* سبز */
    #services .link-box:nth-child(8){ background:#8e44ad; }  /* ارغوانی */
    #services .link-box:nth-child(9){ background:#16a085; }  /* سبز تیره */
    #services .link-box:nth-child(10){ background:#c0392b; } /* قرمز */
    #services .link-box:nth-child(11){ background:#2980b9; } /* آبی تیره */
    #services .link-box:nth-child(12){ background:#27ae60; } /* سبز */
    #services .link-box:nth-child(13){ background:#e74c3c; } /* قرمز روشن */

    /* دکمه بازگشت — تک‌خطی و رنگ اختصاصی */
    .back-btn{
      flex:1 1 100% !important;
      background:#6c5ce7 !important; /* رنگ دلخواه برای بازگشت */
      padding:11px;
      border-radius:16px;
      font-weight:600;
    }

    /* انیمیشن ورود صفحه (برای جلوه هنگام باز شدن هر بخش) */
    .enter{
      animation: pageIn .32s ease both;
    }
    @keyframes pageIn{
      from{ opacity:0; transform: translateY(12px) scale(.995); }
      to{ opacity:1; transform: translateY(0) scale(1); }
    }

    .hidden{ display:none !important; }

    /* واکنش‌گرایی کوچک در موبایل */
    @media (max-width:420px){
      .card{ width:92vw; padding:20px; }
      .link-box{ font-size:14px; }
    }
  </style>
</head>
<body>
  <div class="card">
    <!-- پیام‌ها (نمایش در main و contacts؛ در services دو پیام آخر مخفی می‌شن) -->
    <div id="messages">
      <div class="msg1">کافی نت اشرفی</div>
      <div class="msg2">از حسن توجه شما بسیار سپاسگزاریم</div>
      <div class="msg3">لطفا برای ادامه یکی از گزینه‌های زیر را انتخاب کنید</div>
      <div class="msg4">توجه: برای استفاده از تلگرام باید فیلترشکن فعال باشد</div>
    </div>

    <!-- صفحه اصلی -->
    <div id="main-menu" class="links-container">
      <a class="link-box" href="javascript:void(0)" onclick="showPage('services')">خدمات</a>
      <a class="link-box" href="javascript:void(0)" onclick="showPage('contacts')">لینک‌های ارتباطی</a>
    </div>

    <!-- صفحه خدمات (پیام‌های msg3 و msg4 در این صفحه مخفی می‌شن) -->
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
      <div class="link-box">نصب ویندوز و برنامه‌های کاربردی</div>

      <!-- بازگشت تک‌خطی -->
      <a class="link-box back-btn" href="javascript:void(0)" onclick="showPage('main-menu')">بازگشت به صفحه قبل</a>
    </div>

    <!-- صفحه لینک‌ها (دکمه‌ها دو ستونه؛ بازگشت تک‌خطی در انتها) -->
    <div id="contacts" class="links-container hidden">
      <a class="link-box" href="https://rubika.ir/ashrafi_c_net" target="_blank">روبیکا</a>
      <a class="link-box" href="https://ble.ir/ashrafi_c_net" target="_blank">بله</a>
      <a class="link-box" href="https://sapp.ir/ashrafi_c_net" target="_blank">سروش</a>
      <a class="link-box" href="https://shad.ir/prfcxe5593" target="_blank">شاد</a>
      <a class="link-box" href="https://eitaa.com/ashrafi_c_net" target="_blank">ایتا</a>
      <a class="link-box" href="https://t.me/ashrafi_c_net" target="_blank">تلگرام</a>
      <a class="link-box" href="https://wa.me/989309166187" target="_blank">واتساپ</a>
      <a class="link-box" href="tel:+989309166187">تماس تلفنی</a>
      <a class="link-box" href="https://maps.google.com/maps?q=37.51278296507102%2C45.06070375442505&z=17&hl=fa" target="_blank">مسیریابی</a>
      <!-- بازگشت تک‌خطی -->
      <a class="link-box back-btn" href="javascript:void(0)" onclick="showPage('main-menu')">بازگشت به صفحه قبل</a>
    </div>
  </div>

  <script>
    // باز کردن صفحه با انیمیشن و کنترل نمایش پیام‌ها
    function showPage(pageId){
      const pages = ['main-menu','services','contacts'];
      pages.forEach(id=>{
        const el = document.getElementById(id);
        if(el) el.classList.add('hidden');
      });

      // نشان دادن صفحه انتخابی و افزودن کلاس انیمیشن
      const page = document.getElementById(pageId);
      if(!page) return;
      page.classList.remove('hidden');
      page.classList.add('enter');
      page.addEventListener('animationend', ()=> page.classList.remove('enter'), {once:true});

      // مدیریت نمایش پیام‌های msg3 و msg4:
      // در صفحه خدمات مخفی می‌شن، در بقیه صفحات نمایش داده می‌شن.
      const msg3 = document.querySelector('.msg3');
      const msg4 = document.querySelector('.msg4');
      if(pageId === 'services'){
        if(msg3) msg3.style.display = 'none';
        if(msg4) msg4.style.display = 'none';
      } else {
        if(msg3) msg3.style.display = '';
        if(msg4) msg4.style.display = '';
      }
    }

    // هنگام بارگذاری اول، انیمیشن روی صفحه اصلی اعمال شود
    window.addEventListener('DOMContentLoaded', ()=>{
      const main = document.getElementById('main-menu');
      main.classList.add('enter');
      setTimeout(()=> main.classList.remove('enter'), 400);
    });
  </script>
</body>
</html>
