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

    #searchBox {
      width: 100%;
      padding: 10px;
      margin-bottom: 20px;
      background-color: #333;
      color: white;
      border: 2px solid #444;
      border-radius: 8px;
      font-size: 16px;
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
  </style>
</head>
<body oncontextmenu="return false" onkeydown="return disableKeys(event)">

  <!-- أعلى الصفحة -->
  <div id="topBar">
    <div id="developer">مصطفى جلال | Mustafa Jalal</div>
    <div id="settingsMenu">
      <button class="btn-setting" onclick="toggleTheme()">تغيير الوضع</button>
    </div>
  </div>

  <!-- شريط البحث -->
  <input type="text" id="searchBox" onkeyup="searchScripts()" placeholder="ابحث عن السكربتات...">

  <!-- خانة Emergency hambuurg -->
  <div class="script-box" id="emergency-hambuurg">
    <div class="premium-text">Emergency hambuurg</div>
    <h2>باتمان | batman 🦇</h2>
    <textarea readonly>
loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()
    </textarea>
  </div>

  <!-- خانة Other Scripts -->
  <div class="script-box" id="other-scripts">
    <div class="premium-text">جميع المابات</div>
    <h2>الشبح | Ghost 👻</h2>
    <textarea readonly>
loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
    </textarea>

    <div class="premium-text">جميع المابات</div>
    <h2>طيران | fly 🕊️</h2>
    <textarea readonly>
loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()
    </textarea>
  </div>

  <!-- خانة Brookhaven -->
  <div class="script-box" id="brookhaven">
    <div class="premium-text">Brookhaven</div>
    <h2>قتل كنبه | Kill couch 🤙🏻</h2>
    <textarea readonly>
loadstring(game:HttpGet('https://raw.githubusercontent.com/SnoobG/Lua-Script-s/refs/heads/main/BrookHaven%20TvonHub'))()
    </textarea>

    <div class="premium-text">Brookhaven</div>
    <h2>نسخ سكنات | Copy housing 💯</h2>
    <textarea readonly>
loadstring(game:HttpGet("https://raw.githubusercontent.com/as6cd0/SP_Hub/refs/heads/main/Brookhaven"))()
    </textarea>

    <div class="premium-text">Brookhaven</div>
    <h2>قتل كنبه قوي جداً | Kill couch (Very Strong) ☠️</h2>
    <textarea readonly>
loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Auto%20Fling%20Player'))()
    </textarea>

    <div class="premium-text">Brookhaven</div>
    <h2>رحمه | bang 🔞</h2>
    <textarea readonly>
loadstring(game:HttpGet("https://raw.githubusercontent.com/n0kc/AtomicHub/main/Map-Al-Biout.lua"))()
    </textarea>
  </div>

  <!-- التواصل مع المطور -->
  <div class="contact-dev">
    تواصل مع المطور لطلب السكربتات:<br>
    <span>Tiktok: The_Smiths505</span><br>
    <span>Email: relio201277@gmail.com</span>
  </div>

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
      var input = document.getElementById("searchBox");
      var filter = input.value.toUpperCase();
      var boxes = document.getElementsByClassName("script-box");

      for (var i = 0; i < boxes.length; i++) {
        var text = boxes[i].innerText || boxes[i].textContent;
        boxes[i].classList.toggle("hidden", text.toUpperCase().indexOf(filter) === -1);
      }
    }

    document.addEventListener('copy', e => e.preventDefault());
    function disableKeys(e) {
      if ((e.ctrlKey && e.key === 'u') || e.key === 'PrintScreen') {
        return false;
      }
    }
  </script>

</body>
</html>
