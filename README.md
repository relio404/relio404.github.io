<!DOCTYPE html>
<html lang="ar">
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
      height: 150px;
      background-color: #333;
      color: #fff;
      border: none;
      padding: 10px;
      resize: none;
      font-family: monospace;
      margin-bottom: 10px;
    }
    .copy-btn {
      background-color: #FFD700;
      border: none;
      padding: 6px 10px;
      border-radius: 5px;
      cursor: pointer;
      color: #000;
      font-weight: bold;
      font-size: 14px;
    }
    .hidden {
      display: none;
    }
    .premium-text {
      font-family: 'Roboto Slab', serif;
      font-size: 24px;
      font-weight: bold;
      color: #FFD700;
      text-align: center;
      margin-bottom: 15px;
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
<body>

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

  <!-- سكربت: Emergency hamburg -->
  <div class="script-box">
    <div class="premium-text">Emergency hambuurg</div>
    <h2>باتمان | batman</h2>
    <textarea readonly id="s1">loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</textarea>
    <button class="copy-btn" onclick="copyText('s1')">نسخ السكربت</button>
  </div>

  <!-- سكربت: Ghost and Fly -->
  <div class="script-box">
    <div class="premium-text">جميع المابات</div>
    <h2>الشبح | Ghost</h2>
    <textarea readonly id="s2">loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</textarea>
    <button class="copy-btn" onclick="copyText('s2')">نسخ السكربت</button>

    <h2>طيران | Fly</h2>
    <textarea readonly id="s3">loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()</textarea>
    <button class="copy-btn" onclick="copyText('s3')">نسخ السكربت</button>
  </div>

  <!-- سكربت: Brookhaven -->
  <div class="script-box">
    <div class="premium-text">Brookhaven</div>
    <h2>قتل كنبه | Kill couch</h2>
    <textarea readonly id="s4">loadstring(game:HttpGet('https://raw.githubusercontent.com/SnoobG/Lua-Script-s/refs/heads/main/BrookHaven%20TvonHub'))()</textarea>
    <button class="copy-btn" onclick="copyText('s4')">نسخ السكربت</button>

    <h2>نسخ سكنات</h2>
    <textarea readonly id="s5">loadstring(game:HttpGet("https://raw.githubusercontent.com/as6cd0/SP_Hub/refs/heads/main/Brookhaven"))()</textarea>
    <button class="copy-btn" onclick="copyText('s5')">نسخ السكربت</button>

    <h2>قتل كنبه قوي جداً</h2>
    <textarea readonly id="s6">loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Auto%20Fling%20Player'))()</textarea>
    <button class="copy-btn" onclick="copyText('s6')">نسخ السكربت</button>
  </div>

  <!-- سكربت: MM2 -->
  <div class="script-box">
    <div class="premium-text">MM2</div>
    <h2>ام ام تو قوي</h2>
    <textarea readonly id="s7">loadstring(game:HttpGet("https://raw.githubusercontent.com/Au0yX/Community/main/XhubMM2"))()</textarea>
    <button class="copy-btn" onclick="copyText('s7')">نسخ السكربت</button>
  </div>

  <!-- سكربت: Blox Fruit -->
  <div class="script-box">
    <div class="premium-text">Blox Fruit</div>
    <h2>القمر | The moon</h2>
    <textarea readonly id="s8">loadstring(game:HttpGet("https://raw.githubusercontent.com/UserDevEthical/Loadstring/main/CokkaHub.lua"))()</textarea>
    <button class="copy-btn" onclick="copyText('s8')">نسخ السكربت</button>
  </div>

  <!-- سكربت: Pet Simulator -->
  <div class="script-box">
    <div class="premium-text">Pet Simulator</div>
    <h2>بت سمليتر</h2>
    <textarea readonly id="s9">loadstring(game:HttpGet("https://raw.githubusercontent.com/mzkv/ps99/refs/heads/main/zapHub"))()</textarea>
    <button class="copy-btn" onclick="copyText('s9')">نسخ السكربت</button>
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
    function toggleTheme() {
      document.body.classList.toggle("light-mode");
    }

    function copyText(id) {
      const textarea = document.getElementById(id);
      navigator.clipboard.writeText(textarea.value);
    }

    function searchScripts() {
      const filter = document.getElementById("searchBox").value.toUpperCase();
      const boxes = document.getElementsByClassName("script-box");
      let count = 0;
      for (let box of boxes) {
        const text = box.innerText.toUpperCase();
        const match = text.includes(filter);
        box.classList.toggle("hidden", !match);
        if (match) count++;
      }
      document.getElementById("scriptCount").textContent = "السكربتات: " + count;
    }

    window.onload = searchScripts;
  </script>
</body>
</html>
