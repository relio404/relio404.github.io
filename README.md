<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <title>موقع السكربتات</title>
  <style>
    body {
      background-color: #121212;
      color: white;
      font-family: Arial, sans-serif;
      padding: 20px;
    }

    #searchBox {
      width: 100%;
      padding: 10px;
      margin-bottom: 20px;
      font-size: 16px;
      border-radius: 8px;
      border: none;
    }

    .script-box {
      background-color: #1e1e1e;
      padding: 15px;
      margin-bottom: 10px;
      border-radius: 10px;
    }

    .hidden {
      display: none;
    }

    footer {
      margin-top: 40px;
      border-top: 1px solid #333;
      padding-top: 20px;
    }

    .footer-section {
      margin-bottom: 30px;
    }

    a {
      color: #00bfff;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body onkeydown="return disableKeys(event)">

  <input type="text" id="searchBox" placeholder="ابحث عن سكربت..." onkeyup="searchScripts()">

  <div class="script-box">
    <h3>سكربت 1</h3>
    <textarea rows="5" cols="50">-- سكربت مثال 1</textarea>
  </div>

  <div class="script-box">
    <h3>سكربت 2</h3>
    <textarea rows="5" cols="50">-- سكربت مثال 2</textarea>
  </div>

  <p id="scriptCount">السكربتات: 0</p>

  <footer>
    <div class="footer-section">
      <h3>اتصل بنا</h3>
      <p>راسلنا على البريد الإلكتروني: <a href="mailto:relio201277@gmail.com">relio201277@gmail.com</a></p>
    </div>
    <div class="footer-section">
      <h3>سياسة الخصوصية</h3>
      <p>نحن نحترم خصوصيتك. لا نقوم بجمع أي معلومات شخصية بدون إذنك. قد نستخدم ملفات تعريف الارتباط لتحسين تجربتك على الموقع.</p>
    </div>
  </footer>

  <script>
    function searchScripts() {
      var input = document.getElementById("searchBox");
      var filter = input.value.toUpperCase();
      var boxes = document.getElementsByClassName("script-box");

      for (var i = 0; i < boxes.length; i++) {
        var text = boxes[i].innerText || boxes[i].textContent;
        boxes[i].classList.toggle("hidden", text.toUpperCase().indexOf(filter) === -1);
      }

      updateScriptCount();
    }

    function updateScriptCount() {
      const scripts = document.querySelectorAll("textarea");
      const visibleScripts = Array.from(scripts).filter(t => !t.closest('.script-box').classList.contains("hidden"));
      document.getElementById("scriptCount").textContent = "السكربتات: " + visibleScripts.length;
    }

    window.onload = updateScriptCount;

    document.addEventListener('copy', e => e.preventDefault());

    function disableKeys(e) {
      if ((e.ctrlKey && e.key === 'u') || e.key === 'PrintScreen') {
        return false;
      }
    }
  </script>

</body>
</html>
