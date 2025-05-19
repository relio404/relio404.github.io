<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>سكربتات Roblox - مصطفى جلال</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #181818;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      transition: background-color 0.3s, color 0.3s;
      user-select: none;
    }
    #topBar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 20px;
      flex-wrap: wrap;
    }
    #developer {
      font-family: 'Roboto Slab', serif;
      font-size: 20px;
      color: #FFD700;
      user-select: text;
    }
    #settingsMenu {
      display: flex;
      gap: 10px;
      margin-top: 10px;
    }
    .btn-setting {
      padding: 6px 10px;
      background-color: #444;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      user-select: none;
      transition: background-color 0.3s;
    }
    .btn-setting:hover {
      background-color: #666;
    }
    #searchContainer {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-bottom: 20px;
      flex-wrap: wrap;
    }
    #searchBox {
      flex: 1 1 300px;
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
      user-select: none;
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
      user-select: text;
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
      user-select: text;
    }
    .hidden {
      display: none !important;
    }
    .premium-text {
      font-family: 'Roboto Slab', serif;
      font-size: 24px;
      font-weight: bold;
      color: #FFD700;
      text-align: center;
      margin-bottom: 15px;
      user-select: text;
    }
    .contact-dev {
      text-align: center;
      margin-top: 30px;
      font-family: 'Roboto Slab', serif;
      font-size: 18px;
      user-select: text;
    }
    .contact-dev span {
      color: #FFD700;
      font-weight: bold;
    }
    footer {
      text-align: center;
      margin-top: 40px;
      font-size: 14px;
      user-select: text;
    }
    footer a {
      color: #FFD700;
      margin: 0 10px;
      text-decoration: none;
    }
    footer a:hover {
      text-decoration: underline;
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
    <div class="premium-text">Emergency Hambuurg</div>
    <h2>باتمان | batman 🦇</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</textarea>
  </div>

  <!-- Ghost and Fly -->
  <div class="script-box">
    <div class="premium-text">جميع المابات</div>
    <h2>الشبح | Ghost 👻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</textarea>

    <h2>طيران | Fly 🕊️</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()</textarea>

    <h2>سيارة | Car 🚗</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/username/CarScript/main/car.lua"))()</textarea>
  </div>

  <!-- Brookhaven -->
  <div class="script-box">
    <div class="premium-text">Brookhaven</div>
    <h2>قتل كنبه | Kill couch 🤙🏻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/SnoobG/Lua-Script-s/refs/heads/main/BrookHaven%20TvonHub'))()</textarea>

    <h2>نسخ سكنات | Copy housing 💯</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/as6cd0/SP_Hub/refs/heads/main/Brookhaven"))()</textarea>

    <h2>قتل كنبه قوي جداً | Kill couch ☠️</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Auto%20Fling%20Player'))()</textarea>

    <h2>رحمه | Bang 🔞</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/n0kc/AtomicHub/main/Map-Al-Biout.lua"))()</textarea>
  </div>

  <!-- MM2 -->
  <div class="script-box">
    <div class="premium-text">MM2</div>
    <h2>ام ام تو قوي | MM2 🔪</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/Au0yX/Community/main/XhubMM2"))()</textarea>
  </div>

  <!-- Blox Fruit -->
  <div class="script-box">
    <div class="premium-text">Blox Fruit</div>
    <h2>القمر | The moon 🌚</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/UserDevEthical/Loadstring/main/CokkaHub.lua"))()</textarea>

    <h2>ريدز | Redz 🍒</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/newredz/BloxFruits/refs/heads/main/Source.luau"))(Settings)</textarea>

    <h2>صيد فواكه | Fruit hunting 🍓</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/VNT-UNIVERSAL/Panda-Hub/main/Release/fruitfarm.lua"))()</textarea>
  </div>

  <!-- Pet Simulator -->
  <div class="script-box">
    <div class="premium-text">Pet Simulator</div>
    <h2>بت سمليتر | Pet Simulator 🐕</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/mzkv/ps99/refs/heads/main/zapHub"))()</textarea>
  </div>

  <!-- سكربتات عامة -->
  <div class="script-box">
    <div class="premium-text">سكربتات عامة</div>
    <h2>زيادة السرعة | Speed Hack ⚡</h2>
    <textarea readonly>
-- تغيير سرعة اللاعب
local player = game.Players.LocalPlayer
local speed = 100
player.Character.Humanoid.WalkSpeed = speed
    </textarea>

    <h2>قفز عالي | High Jump ⬆️</h2>
    <textarea readonly>
-- زيادة قفز اللاعب
local player = game.Players.LocalPlayer
local jumpPower = 100
player.Character.Humanoid.JumpPower = jumpPower
    </textarea>

    <h2>تليبور | Teleport 🌀</h2>
    <textarea readonly>
-- نقل اللاعب إلى مكان معين
local player = game.Players.LocalPlayer
local targetPosition = Vector3.new(0, 10, 0)
player.Character.HumanoidRootPart.CFrame = CFrame.new(targetPosition)
    </textarea>
  </div>

  <div class="contact-dev">
    تواصل مع المطور لطلب السكربتات:<br>
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
      if (dark) {
        document.body.style.backgroundColor = "#f0f0f0";
        document.body.style.color = "#000";
        document.querySelectorAll('.script-box').forEach(box => box.style.backgroundColor = '#fff');
        document.querySelectorAll('textarea').forEach(t => t.style.backgroundColor = '#ddd');
        dark = false;
      } else {
        document.body.style.backgroundColor = "#181818";
        document.body.style.color = "#fff";
        document.querySelectorAll('.script-box').forEach(box => box.style.backgroundColor = '#222');
        document.querySelectorAll('textarea').forEach(t => t.style.backgroundColor = '#333');
        dark = true;
      }
    }

    function searchScripts() {
      const input = document.getElementById("searchBox");
      const filter = input.value.toUpperCase();
      const boxes = document.getElementsByClassName("script-box");

      for (let i = 0; i < boxes.length; i++) {
        const text = boxes[i].innerText || boxes[i].textContent;
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
      if ((e.ctrlKey && e.key.toLowerCase() === 'u') || e.key === 'PrintScreen') {
        return false;
      }
    }
  </script>
</body>
</html>
