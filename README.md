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

    #scriptCount {
      background-color: #444;
      color: white;
      padding: 5px 10px;
      border-radius: 5px;
      font-size: 16px;
      display: inline-block;
      margin-left: 10px;
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

  <!-- شريط البحث + عدد السكربتات -->
  <div style="display: flex; align-items: center;">
    <input type="text" id="searchBox" onkeyup="searchScripts()" placeholder="ابحث عن السكربتات...">
    <div id="scriptCount">عدد السكربتات: <span id="countNumber">10</span></div>
  </div>

  <!-- خانة MM2 -->
  <div class="script-box" id="MM2">
    <div class="premium-text">ام ام تو قوي | MM2 🔪</div>
    <h2>MM2</h2>
    <textarea readonly>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Au0yX/Community/main/XhubMM2"))()
    </textarea>
  </div>

  <!-- خانة Blox Fruit -->
  <div class="script-box" id="BloxFruit">
    <div class="premium-text">القمر | The moon 🌚</div>
    <h2>القمر | The moon 🌚</h2>
    <textarea readonly>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/UserDevEthical/Loadstring/main/CokkaHub.lua"))()
    </textarea>

    <div class="premium-text">ريدز | Redz 🍒</div>
    <h2>ريدز | Redz 🍒</h2>
    <textarea readonly>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/newredz/BloxFruits/refs/heads/main/Source.luau"))(Settings)
    </textarea>

    <div class="premium-text">صيد فواكه | Fruit hunting 🍓</div>
    <h2>صيد فواكه | Fruit hunting 🍓</h2>
    <textarea readonly>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/VNT-UNIVERSAL/Panda-Hub/main/Release/fruitfarm.lua"))()
    </textarea>
  </div>

  <!-- خانة Pet Simulator -->
  <div class="script-box" id="PetSimulator">
    <div class="premium-text">بت سمليتر | Pet Simulator 🐕</div>
    <h2>بت سمليتر | Pet Simulator 🐕</h2>
    <textarea readonly>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/mzkv/ps99/refs/heads/main/zapHub"))()
    </textarea>
  </div>

  <!-- التواصل مع المطور -->
  <div class="contact-dev">
    تواصل مع المطور لطلب السكربتات:<br>
    <span>Tiktok: The_Smiths505</span><br>
    <span>Email: relio201277@gmail.com</span>
  </div>

  <script>
    // تغيير الوضع الداكن والفاتح
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

    // البحث
    function searchScripts() {
      var input = document.getElementById("searchBox");
      var filter = input.value.toUpperCase();
      var boxes = document.getElementsByClassName("script-box");
      var count = 0;

      for (var i = 0; i < boxes.length; i++) {
        var text = boxes[i].innerText || boxes[i].textContent;
        if (text.toUpperCase().indexOf(filter) !== -1) {
          boxes[i].classList.remove("hidden");
          count++;
        } else {
          boxes[i].classList.add("hidden");
        }
      }

      // تحديث عدد السكربتات
      document.getElementById("countNumber").textContent = count;
    }

    // منع النسخ والسكربتات
    document.addEventListener('copy', e => e.preventDefault());
    function disableKeys(e) {
      if ((e.ctrlKey && e.key === 'u') || e.key === 'PrintScreen') {
        return false;
      }
    }
  </script>

</body>
</html>
