<!DOCTYPE html><html lang="ar">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>سكربتات Roblox</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #181818;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
    }
    #topBar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 20px;
    }
    #developer {
      font-family: 'Roboto Slab', serif;
      font-size: 20px;
      color: #FFD700;
    }
    #settingsMenu {
      display: flex;
      gap: 10px;
    }
    .btn-setting {
      padding: 6px 10px;
      background-color: #444;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
    }
    #searchContainer {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 20px;
    }
    #searchBox {
      flex: 1;
      padding: 10px;
      background-color: #333;
      color: white;
      border: 2px solid #444;
      border-radius: 8px;
      font-size: 16px;
    }
    #scriptCount {
      background-color: #444;
      color: white;
      padding: 6px 12px;
      border-radius: 8px;
      font-size: 14px;
      white-space: nowrap;
    }
    .script-box {
      border: 2px solid #333;
      border-radius: 8px;
      padding: 15px;
      margin-bottom: 20px;
      background-color: #222;
    }
    h2 {
      font-size: 18px;
      margin-bottom: 10px;
    }
    textarea {
      width: 100%;
      height: 120px;
      background-color: #333;
      color: #fff;
      border: none;
      padding: 10px;
      resize: none;
      font-family: monospace;
      margin-bottom: 10px;
    }
    .premium-text {
      font-family: 'Roboto Slab', serif;
      font-size: 24px;
      font-weight: bold;
      color: #FFD700;
      text-align: center;
      margin-bottom: 15px;
    }
    .copy-btn {
      padding: 5px 10px;
      background-color: #555;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-size: 14px;
    }
    .contact-dev {
      text-align: center;
      margin-top: 30px;
      font-family: 'Roboto Slab', serif;
      font-size: 18px;
    }
    .contact-dev span {
      color: #FFD700;
      font-weight: bold;
    }
    footer {
      text-align: center;
      margin-top: 40px;
      font-size: 14px;
    }
    footer a {
      color: #FFD700;
      margin: 0 10px;
      text-decoration: none;
    }
  </style>
</head>
<body oncontextmenu="return false" onkeydown="return disableKeys(event)">
  <div id="topBar">
    <div id="developer">مصطفى جلال | Mustafa Jalal</div>
    <div id="settingsMenu">
      <button class="btn-setting" onclick="toggleTheme()">تغيير الوضع</button>
    </div>
  </div>

  <div id="searchContainer">
    <input type="text" id="searchBox" onkeyup="searchScripts()" placeholder="ابحث عن السكربتات...">
    <div id="scriptCount">السكربتات: 0</div>
  </div>

  <!-- Emergency hamburg -->
  <div class="script-box">
    <div class="premium-text">Emergency hamburg</div>
    <h2>باتمان | batman 🦇</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</textarea>
    <button class="copy-btn" onclick="copyText(this)">نسخ السكربت</button>
  </div>

  <!-- Ghost and Fly -->
  <div class="script-box">
    <div class="premium-text">جميع المابات</div>
    <h2>الشبح | Ghost 👻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</textarea>
    <button class="copy-btn" onclick="copyText(this)">نسخ السكربت</button>
  </div>

  <!-- Brookhaven -->
  <div class="script-box">
    <div class="premium-text">Brookhaven</div>
    <h2>قتل كنبه | Kill couch 🤙🏻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/SnoobG/Lua-Script-s/refs/heads/main/BrookHaven%20TvonHub'))()</textarea>
    <button class="copy-btn" onclick="copyText(this)">نسخ السكربت</button>
  </div>

  <!-- Dead Rails -->
  <div class="script-box">
    <div class="premium-text">Dead Rails</div>
    <h2>Dead Rails</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/InfernusScripts/Null-Fire/main/Loader"))()</textarea>
    <button class="copy-btn" onclick="copyText(this)">نسخ السكربت</button>
  </div>

  <!-- TPS -->
  <div class="script-box">
    <div class="premium-text">TPS</div>
    <h2>TPS</h2>
    <textarea readonly>loadstring(game:HttpGet("https://paste.ee/r/ykM2s", true))()</textarea>
    <button class="copy-btn" onclick="copyText(this)">نسخ السكربت</button>
  </div>

  <div class="contact-dev">
    تواصل مع المطور:<br>
    <span>Tiktok: The_Smiths505</span><br>
    <span>Email: relio201277@gmail.com</span>
  </div>

  <footer>
    <a href="privacy.html">سياسة الخصوصية</a> |
    <a href="contact.html">اتصل بنا</a>
  </footer>

  <script>
    let dark = true;
    function toggleTheme() {
      document.body.style.backgroundColor = dark ? "#f0f0f0" : "#181818";
      document.body.style.color = dark ? "#000" : "#fff";
      document.querySelectorAll('.script-box').forEach(box => box.style.backgroundColor = dark ? '#fff' : '#222');
      document.querySelectorAll('textarea').forEach(t => t.style.backgroundColor = dark ? '#ddd' : '#333');
      dark = !dark;
    }

    function searchScripts() {
      const input = document.getElementById("searchBox").value.toUpperCase();
      const boxes = document.getElementsByClassName("script-box");
      let count = 0;

      for (let box of boxes) {
        const text = box.innerText.toUpperCase();
        const match = text.includes(input);
        box.style.display = match ? "" : "none";
        if (match) count++;
      }

      document.getElementById("scriptCount").textContent = "السكربتات: " + count;
    }

    function copyText(btn) {
      const textarea = btn.previousElementSibling;
      textarea.select();
      textarea.setSelectionRange(0, 99999);
      navigator.clipboard.writeText(textarea.value);
      btn.textContent = "تم النسخ!";
      setTimeout(() => btn.textContent = "نسخ السكربت", 1500);
    }

    window.onload = () => searchScripts();

    document.addEventListener('copy', e => e.preventDefault());
    function disableKeys(e) {
      if ((e.ctrlKey && e.key === 'u') || e.key === 'PrintScreen') {
        return false;
      }
    }
  </script>
</body>
</html>
