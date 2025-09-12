<html lang="fa">
<head>
  <meta charset="UTF-8">
  <title>کارت ویزیت من</title>
  <link href="https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Vazirmatn', sans-serif;
      background: linear-gradient(135deg, #74ebd5, #ACB6E5);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .card {
      background: white;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      text-align: center;
      width: 360px;
      animation: fadeIn 1s ease-in-out;
    }
    .msg1 {
      font-weight: bold;
      margin-bottom: 17px;
    }
    .msg2 {
      font-size: 15px;
      color: green;
      margin-bottom: 15px;
    }
    .msg3 {
      font-size: 15px;
      margin-bottom: 15px;
    }
    .msg4 {
      font-size: 13px;
      color: red;
      margin-bottom: 20px;
    }
    .links-container {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 10px;
    }
    .link-box {
      flex: 1 1 calc(50% - 10px);
      margin: 5px 0;
      padding: 12px;
      border-radius: 20px;
      color: white;
      text-decoration: none;
      font-size: 16px;
      transition: 0.3s;
      box-shadow: 0 4px 8px rgba(0,0,0,0.15);
      text-align: center;
      display: block;
      animation: slideIn 0.5s ease-in-out;
    }
    .link-box:hover {
      transform: translateY(-3px);
      filter: brightness(1.2);
    }
    /* رنگ‌های متنوع برای خدمات */
    #services .link-box:nth-child(1) { background: #3498db; }
    #services .link-box:nth-child(2) { background: #9b59b6; }
    #services .link-box:nth-child(3) { background: #e67e22; }
    #services .link-box:nth-child(4) { background: #1abc9c; }
    #services .link-box:nth-child(5) { background: #f39c12; }
    #services .link-box:nth-child(6) { background: #d35400; }
    #services .link-box:nth-child(7) { background: #2ecc71; }
    #services .link-box:nth-child(8) { background: #8e44ad; }
    #services .link-box:nth-child(9) { background: #16a085; }
    #services .link-box:nth-child(10) { background: #c0392b; }
    #services .link-box:nth-child(11) { background: #2980b9; }
    #services .link-box:nth-child(12) { background: #27ae60; }
    #services .link-box:nth-child(13) { background: #e74c3c; }
    /* دکمه بازگشت رنگ خاص */
    .back-btn {
      flex: 1 1 100%;
      background: #555 !important;
    }
    /* انیمیشن ورود */
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    @keyframes slideIn {
      from { opacity: 0; transform: translateX(-30px); }
      to { opacity: 1; transform: translateX(0); }
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div class="card">
    <!-- پیام‌های اصلی -->
    <div class="msg1">کافی نت اشرفی</div>
    <div class="msg2">‌از حسن توجه شما بسیار سپاسگزاریم</div>
    <div class="msg3">لطفا برای ادامه یکی از گزینه‌های زیر را انتخاب کنید</div>
    <div class="msg4">توجه: برای استفاده از تلگرام باید فیلترشکن فعال باشد</div>

    <!-- صفحه اصلی -->
    <div id="main-menu" class="links-container">
      <a class="link-box" href="#" onclick="showPage('services')">خدمات</a>
      <a class="link-box" href="#" onclick="showPage('contacts')">لینک‌های ارتباطی</a>
    </div>

    <!-- صفحه خدمات -->
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
      <a class="link-box back-btn" href="#" onclick="showPage('main-menu')">بازگشت به صفحه قبل</a>
    </div>

    <!-- صفحه لینک‌های ارتباطی -->
    <div id="contacts" class="links-container hidden">
      <a class="link-box" href="https://rubika.ir/ashrafi_c_net" target="_blank">روبیکا</a>
      <a class="link-box" href="https://ble.ir/ashrafi_c_net" target="_blank">بله</a>
      <a class="link-box" href="https://sapp.ir/ashrafi_c_net" target="_blank">سروش</a>
      <a class="link-box" href="https://shad.ir/prfcxe5593" target="_blank">شاد</a>
      <a class="link-box" href="https://eitaa.com/ashrafi_c_net" target="_blank">ایتا</a>
      <a class="link-box" href="https://t.me/ashrafi_c_net" target="_blank">تلگرام</a>
      <a class="link-box" href="https://wa.me/989309166187" target="_blank">واتساپ</a>
      <a class="link-box" href="tel:+989309166187">تماس تلفنی</a>
      <a class="link-box back-btn" href="#" onclick="showPage('main-menu')">بازگشت به صفحه قبل</a>
    </div>
  </div>

  <script>
    function showPage(pageId) {
      document.getElementById('main-menu').classList.add('hidden');
      document.getElementById('services').classList.add('hidden');
      document.getElementById('contacts').classList.add('hidden');
      document.getElementById(pageId).classList.remove('hidden');
    }
  </script>
</body>
</html>
