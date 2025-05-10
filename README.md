<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>موقع سكربتات روبلوكس</title>
  <style>
    /* زيادة السواد في الخلفية */
    body {
      font-family: Arial, sans-serif;
      background-color: #0a0d12; /* زيادة السواد أكثر */
      color: #c9d1d9;
      margin: 0;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    /* رأس الصفحة */
    header {
      width: 100%;
      background-color: #121417; /* خلفية أغمق قليلاً */
      padding: 15px;
      text-align: center;
    }

    h1 {
      font-size: 1.8rem;
      margin: 0;
      color: #f0f0f0;
    }

    .search-bar {
      margin-top: 10px;
    }

    .search-bar input {
      padding: 8px;
      font-size: 1rem;
      width: 80%;
      border: 1px solid #444;
      background-color: #1c1f26;
      color: #fff;
      border-radius: 5px;
    }

    /* تصميم السكربتات */
    .scripts-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      width: 100%;
      padding: 20px 0;
    }

    .script-box {
      background-color: #161b22;
      border: 1px solid #444;
      width: 90%;
      margin: 10px 0;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.3); /* إضافة تأثير إضاءة خفيف للون الأزرق */
    }

    .script-box h2 {
      color: #58a6ff;
      font-size: 1.4rem;
      margin-bottom: 10px;
      text-shadow: 0 0 5px #58a6ff; /* تأثير ضوء خفيف على الأزرق */
    }

    .script-box p {
      font-size: 1rem;
      margin-bottom: 10px;
    }

    .script-box a {
      color: #58a6ff;
      text-decoration: none;
      font-size: 1rem;
    }

    .script-box a:hover {
      text-decoration: underline;
    }

    /* Footer */
    footer {
      background-color: #121417;
      padding: 20px;
      width: 100%;
      text-align: center;
    }

    footer p {
      font-size: 0.9rem;
    }

    /* التصميم المتجاوب للجوال */
    @media screen and (max-width: 600px) {
      h1 {
        font-size: 1.5rem;
      }

      .search-bar input {
        width: 90%;
      }

      .script-box h2 {
        font-size: 1.2rem;
      }

      .script-box p {
        font-size: 0.9rem;
      }
    }

  </style>
</head>
<body>

  <!-- Header Section -->
  <header>
    <h1>موقع سكربتات روبلوكس</h1>
    <div class="search-bar">
      <input type="text" placeholder="ابحث عن سكربتات..." />
    </div>
  </header>

  <!-- Scripts Container -->
  <div class="scripts-container">
    <!-- Script Box for Emergency Hamburger -->
    <div class="script-box">
      <h2>Script Emergency Hamburger</h2>
      <p>إضافة خاصية الهامبرغر الطوارئ إلى لعبة روبلوكس.</p>
      <a href="#">عرض السكربت</a>
    </div>

    <!-- يمكن إضافة المزيد من السكربتات هنا -->
    <div class="script-box">
      <h2>Script Another Game</h2>
      <p>هذا سكربت لإضافة ميزة جديدة في اللعبة.</p>
      <a href="#">عرض السكربت</a>
    </div>

    <div class="script-box">
      <h2>Script Custom HUD</h2>
      <p>سكربت لتخصيص واجهة المستخدم في اللعبة.</p>
      <a href="#">عرض السكربت</a>
    </div>
  </div>

  <!-- Footer Section -->
  <footer>
    <p>© 2025 جميع الحقوق محفوظة. <a href="#">الشروط والأحكام</a></p>
  </footer>

</body>
</html>
