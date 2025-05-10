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

    /* نمط السكربتات */
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
      box-shadow: 0 0 10px rgba(88, 166, 255, 0.3);
    }

    .script-box h2 {
      color: #58a6ff;
      font-size: 1.4rem;
      margin-bottom: 10px;
      text-shadow: 0 0 5px #58a6ff;
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
      <p style="font-size: 0.8rem; color: #fff;">Loadstring(لتنفيذ السكربت)</p>
      <pre>loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</pre>
    </div>

    <!-- Other Scripts Section -->
    <div class="expandable" onclick="toggleContent('otherScriptsContent')">
      Other Scripts
    </div>
    <div id="otherScriptsContent" class="expandable-content">
      <p style="font-size: 0.8rem; color: #fff;">Loadstring(لتنفيذ السكربت)</p>
      <pre>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</pre>
    </div>

  </div>

  <!-- Footer Section -->
  <footer>
    <p>© 2025 جميع الحقوق محفوظة. <a href="#">الشروط والأحكام</a></p>
  </footer>

</body>
</html>
