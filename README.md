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
      transition: background-color 0.3s, color 0.3s;
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
      position: relative;
    }
    h2, h3 {
      font-size: 18px;
      margin-bottom: 10px;
      color: #FFD700;
      font-family: 'Roboto Slab', serif;
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
    }
    button.copy-btn {
      position: absolute;
      top: 15px;
      right: 15px;
      padding: 6px 12px;
      border: none;
      background-color: #FFD700;
      color: #000;
      font-weight: bold;
      border-radius: 6px;
      cursor: pointer;
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

  <!-- Emergency hambuurg -->
  <div class="script-box">
    <div class="premium-text">Emergency hambuurg</div>
    <h2>باتمان | batman 🦇</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <!-- Ghost and Fly -->
  <div class="script-box">
    <div class="premium-text">جميع المابات</div>
    <h2>الشبح | Ghost 👻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>

    <h2>طيران | fly 🕊️</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <!-- Brookhaven -->
  <div class="script-box">
    <div class="premium-text">Brookhaven</div>
    <h2>قتل كنبه | Kill couch 🤙🏻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/SnoobG/Lua-Script-s/refs/heads/main/BrookHaven%20TvonHub'))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>

    <h2>نسخ سكنات | Copy housing 💯</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/as6cd0/SP_Hub/refs/heads/main/Brookhaven"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>

    <h2>قتل كنبه قوي جداً | Kill couch ☠️</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Auto%20Fling%20Player'))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>

    <h2>رحمه | bang 🔞</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/n0kc/AtomicHub/main/Map-Al-Biout.lua"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <!-- MM2 -->
  <div class="script-box">
    <div class="premium-text">MM2</div>
    <h2>ام ام تو قوي | MM2 🔪</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/Au0yX/Community/main/XhubMM2"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <!-- Blox Fruit -->
  <div class="script-box">
    <div class="premium-text">Blox Fruit</div>
    <h2>القمر | The moon 🌚</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/UserDevEthical/Loadstring/main/CokkaHub.lua"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>

    <h2>ريدز | Redz 🍒</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/newredz/BloxFruits/refs/heads/main/Source.luau"))(Settings)</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>

    <h2>صيد فواكه | Fruit hunting 🍓</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/VNT-UNIVERSAL/Panda-Hub/main/Release/fruitfarm.lua"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <!-- Pet Simulator -->
  <div class="script-box">
    <div class="premium-text">Pet Simulator</div>
    <h2>بت سمليتر | Pet Simulator 🐕</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/mzkv/ps99/refs/heads/main/zapHub"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <!-- Dead Rails -->
  <div class="script-box">
    <div class="premium-text">Dead Rails</div>
    <h2>Dead Rails</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/InfernusScripts/Null-Fire/main/Loader"))()</textarea>
    <button class="copy-btn" onclick="copyToClipboard(this)">نسخ</button>
  </div>

  <footer>
    جميع الحقوق محفوظة © مصطفى جلال | Mustafa Jalal
  </footer>

  <script>
    const searchBox = document.getElementById('searchBox');
    const scriptBoxes = Array.from(document.getElementsByClassName('script-box'));
    const scriptCount = document.getElementById('scriptCount');

    function copyToClipboard(button) {
      const textarea = button.previousElementSibling;
      textarea.select();
      textarea.setSelectionRange(0, 99999);
      navigator.clipboard.writeText(textarea.value).then(() => {
        button.textContent = "تم النسخ!";
        setTimeout(() => button.textContent = "نسخ", 1500);
      });
    }

    function searchScripts() {
      const filter = searchBox.value.toLowerCase().trim();
      let visibleCount = 0;
      scriptBoxes.forEach(box => {
        const text = box.innerText.toLowerCase();
        if (text.includes(filter)) {
          box.style.display = "";
          visibleCount++;
        } else {
          box.style.display = "none";
        }
      });
      scriptCount.textContent = `السكربتات: ${visibleCount}`;
    }

    // تحديث عدد السكربتات عند التحميل
    searchScripts();

    // منع الأزرار Ctrl+U و PrintScreen و F12
    function disableKeys(e) {
      if ((e.ctrlKey && e.key.toLowerCase() === 'u') || 
          e.key === 'PrintScreen' || 
          e.key === 'F12') {
        return false;
      }
      return true;
    }

    // تغيير الوضع (فاتح / داكن)
    function toggleTheme() {
      if (document.body.style.backgroundColor === 'white') {
        document.body.style.backgroundColor = '#181818';
        document.body.style.color = 'white';
      } else {
        document.body.style.backgroundColor = 'white';
        document.body.style.color = 'black';
      }
    }
  </script>
</body>
</html>
