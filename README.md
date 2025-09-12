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
      flex-direction: column;
      gap: 10px;
    }
    .link-box {
      padding: 12px;
      border-radius: 20px;
      background: #3498db;
      color: white;
      text-decoration: none;
      font-size: 16px;
      transition: 0.3s;
      box-shadow: 0 4px 8px rgba(0,0,0,0.15);
      text-align: center;
      display: block;
    }
    .link-box:hover {
      transform: translateY(-3px);
      background: #2ecc71;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div class="card">
    <!-- پیام‌ها (همیشه نمایش داده میشن) -->
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
      <a class="link-box" href="#" onclick="showPage('main-menu')">بازگشت به صفحه قبل</a>
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
      <a class="link-box" href="#" onclick="showPage('main-menu')">بازگشت به صفحه قبل</a>
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
