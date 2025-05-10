<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>موقع سكربتات روبلوكس</title>
  <style>
    /* الخلفية والأنماط العامة */
    body {
      font-family: Arial, sans-serif;
      background-color: #0a0d12;
      color: #c9d1d9;
      margin: 0;
      padding: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    header {
      width: 100%;
      background-color: #121417;
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

    /* النمط الخاص للقوائم القابلة للفتح */
    .expandable {
      cursor: pointer;
      padding: 10px;
      background-color: #1c1f26;
      border: 1px solid #444;
      margin: 5px 0;
      width: 90%;
      text-align: center;
      color: #58a6ff;
      border-radius: 5px;
    }

    .expandable-content {
      display: none;
      background-color: #121417;
      padding: 10px;
      color: #fff;
      font-size: 0.9rem;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.3);
    }

    .expandable-content pre {
      background-color: #0a0d12;
      color: #fff;
      padding: 15px;
      border-radius: 5px;
      font-size: 0.9rem;
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.2);
    }

    /* مربع النص - بنفس حجم شاشة الجوال */
    .script-box {
      background-color: #161b22;
      border: 1px solid #444;
      width: 90%;
      margin: 10px 0;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.3);
    }

    .script-box pre {
      background-color: #0a0d12;
      color: #fff;
      padding: 15px;
      font-size: 1rem;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.2);
    }

    /* النمط الخاص بالمربع مع اللون الأزرق الخفيف */
    .script-box {
      background-color: #121417;
      color: #fff;
      font-size: 0.9rem;
      border-radius: 5px;
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.1);
    }

    /* التصميم المتجاوب للجوال */
    @media screen and (max-width: 600px) {
      h1 {
        font-size: 1.5rem;
      }

      .search-bar input {
        width: 90%;
      }

      .expandable-content pre {
        font-size: 0.8rem;
      }

      .expandable {
        width: 90%;
        padding: 10px;
      }
    }

  </style>
  <script>
    // وظيفة لفتح وغلق المحتوى
    function toggleContent(id) {
      var content = document.getElementById(id);
      if (content.style.display === "block") {
        content.style.display = "none";
      } else {
        content.style.display = "block";
      }
    }
  </script>
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
    <!-- Emergency Hamburger Script -->
    <div class="expandable" onclick="toggleContent('emergencyHamburgerContent')">
      Emergency Hamburger
    </div>
    <div id="emergencyHamburgerContent" class="expandable-content">
      <div class="script-box">
        <pre>loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</pre>
      </div>
    </div>

    <!-- Other Scripts Section -->
    <div class="expandable" onclick="toggleContent('otherScriptsContent')">
      Other Scripts
    </div>
    <div id="otherScriptsContent" class="expandable-content">
      <div class="script-box">
        <pre>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</pre>
      </div>
    </div>

  </div>

  <!-- Footer Section -->
  <footer>
    <p>© 2025 جميع الحقوق محفوظة. <a href="#">الشروط والأحكام</a></p>
  </footer>

</body>
</html>
