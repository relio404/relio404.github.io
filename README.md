<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>موقع سكربتات روبلوكس</title>
  <style>
    body { font-family: Arial, sans-serif; background: #121212; color: #eee; margin: 0; padding: 0; }
    header, footer { background: #1f1f1f; padding: 15px; text-align: center; }
    header h1 { margin: 0; font-size: 28px; }
    nav { background: #222; padding: 10px; text-align: center; }
    nav a { color: #eee; margin: 0 12px; text-decoration: none; font-weight: bold; }
    nav a:hover { text-decoration: underline; }
    main { padding: 20px; max-width: 1000px; margin: auto; }
    .search-box { margin-bottom: 15px; }
    input[type="text"] { width: 100%; padding: 8px; font-size: 16px; border-radius: 4px; border: none; }
    .scripts-count { margin-bottom: 10px; font-weight: bold; }
    .category { margin-bottom: 40px; }
    .category h2 { border-bottom: 2px solid #444; padding-bottom: 6px; margin-bottom: 15px; }
    .script-item { background: #222; margin-bottom: 10px; padding: 10px; border-radius: 6px; white-space: pre-wrap; position: relative; }
    .script-title { font-weight: bold; font-size: 18px; margin-bottom: 6px; }
    .copy-btn {
      position: absolute;
      top: 10px; left: 10px;
      background: #444; border: none; color: #eee;
      padding: 5px 10px; border-radius: 3px; cursor: pointer;
      font-size: 12px;
    }
    .copy-btn:hover { background: #666; }
    footer small { color: #666; }
  </style>
</head>
<body>

<header>
  <h1>موقع سكربتات روبلوكس - مصطفى جلال</h1>
</header>

<nav>
  <a href="#home">الرئيسية</a>
  <a href="#scripts">السكربتات</a>
  <a href="#privacy">الخصوصية</a>
  <a href="#contact">اتصل بنا</a>
</nav>

<main>

<section id="home">
  <h2>أهلاً بك في موقع السكربتات</h2>
  <p>ابحث عن السكربت الذي تريد وانسخه بسهولة بالضغط على زر النسخ.</p>
</section>

<section id="scripts">
  <div class="search-box">
    <input type="text" id="searchInput" placeholder="ابحث عن سكربت..." oninput="filterScripts()" />
  </div>
  <div class="scripts-count" id="scriptsCount">عدد السكربتات: 38</div>

  <!-- قديم ثابت لا تحذف أو تعدل -->
  <div class="category" id="old-scripts">
    <h2>السكربتات القديمة والثابتة</h2>

    <div class="script-item">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">الشبح (اختفاء)</div>
      loadstring(game:HttpGet('https://pastebin.com/raw/3Rnd9rHf'))()
    </div>
    <div class="script-item">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">Emergency Hamburg</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/InfernusScripts/Null-Fire/main/Loader"))()
    </div>
    <div class="script-item">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">Brookhaven</div>
      loadstring(game:HttpGet('https://raw.githubusercontent.com/hdhjvcfik/KAY-HUB-Script1/refs/heads/main/chalet%2570mohamed'))()
    </div>
    <!-- أضف هنا بقية السكربتات القديمة التي تريد تثبيتها -->
  </div>

  <!-- السكربتات الجديدة التي طلبتها -->
  <div class="category" id="new-scripts">
    <h2>السكربتات الجديدة</h2>

    <div class="script-item" data-title="Dead Rails">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">Dead Rails الجديد</div>
      loadstring(game:HttpGet("https://rawscripts.net/raw/Dead-Rails-Alpha-Dead-Rails-OP-KiciaHook-Script-Fastest-Auto-Farm-35961"))()
    </div>

    <div class="script-item" data-title="تخريب">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">تخريب 😈</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/VR7ss/OMK/main/VR7%20RAGDOLL"))()
    </div>

    <div class="script-item" data-title="ام ام تو قوي 2">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">ام ام تو قوي 2</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Murder%20Mystery"))()
    </div>

    <div class="script-item" data-title="رحمه شغال">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">رحمه شغال كل مابات ☠️</div>
      loadstring(game:HttpGet('https://raw.githubusercontent.com/M1ZZ001/BrookhavenR4D/main/Brookhaven%20R4D%20Script'))()
    </div>

    <div class="script-item" data-title="Muscle legends">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">Muscle legends 💪🏻</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/harisiskandar178/Roblox-Script/main/Muscle%20Legend"))()
    </div>

    <div class="script-item" data-title="زيادة فريمات FPS">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">زيادة فريمات 🫀FPS</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/CasperFlyModz/discord.gg-rips/main/FPSBooster.lua"))()
    </div>

    <div class="script-item" data-title="اختفاء">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">اختفاء</div>
      loadstring(game:HttpGet('https://pastebin.com/raw/3Rnd9rHf'))()
    </div>

    <div class="script-item" data-title="قفل">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">قفل 🔒</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/Sector9922/SECTOR-SHIFT-LOCK/main/SECTOR%20SHIFT%20LOCK"))()
    </div>

    <div class="script-item" data-title="ايم بوت">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">ايم بوت</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/ds5x/Scripts-Xhub/refs/heads/main/IMBOT-XHUB"))()
    </div>

    <div class="script-item" data-title="تنقل">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">تنقل</div>
      loadstring(game:HttpGet('https://raw.githubusercontent.com/Ndora1/Ndora1/main/Nokies'))()
    </div>

    <div class="script-item" data-title="TPS">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">TPS</div>
      loadstring(game:HttpGet("https://paste.ee/r/ykM2s", true))()
    </div>

    <div class="script-item" data-title="نسخ سكنات 2">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">نسخ سكنات 2</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/ahmidd409/-/refs/heads/main/CopyAvatar.txt"))()
    </div>

    <div class="script-item" data-title="عربي انجليزي">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">عربي انجليزي</div>
      loadstring(game:HttpGet("https://raw.githubusercontent.com/as6cd0/SP_Hub/refs/heads/main/Brookhaven"))()
    </div>

    <div class="script-item" data-title="طيران سيارة">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">طيران سيارة</div>
      Loadstring(game:HttpGet("https://raw.githubusercontent.com/hasan08122020108181818/HASA/759cc1030d8a4f4c23b32e8cb8550b47f567d1b9/carflyronald"))()
    </div>

    <div class="script-item" data-title="بلوكس فروت الجديد">
      <button class="copy-btn" onclick="copyCode(this)">نسخ</button>
      <div class="script-title">بلوكس فروت الجديد 🍓</div>
      local Settings = {
  JoinTeam = "Pirates";
  Translator = true;
}

loadstring(game:HttpGet("https://raw.githubusercontent.com/newredz/BloxFruits/refs/heads/main/Source.luau"))(Settings)
    </div>
  </div>
</section>

<section id="privacy">
  <h2>الخصوصية</h2>
  <p>نحن نحترم خصوصيتك ولا نشارك بياناتك مع أي طرف ثالث. الموقع فقط لعرض السكربتات بشكل مجاني للزوار.</p>
</section>

<section id="contact">
  <h2>اتصل بنا</h2>
  <p>للتواصل مع مصطفى جلال: example@email.com</p>
</section>

</main>

<footer>
  <small>جميع الحقوق محفوظة &copy; 2025 مصطفى جلال | mustafa jalal</small>
</footer>

<script>
  function copyCode(button) {
    const scriptItem = button.parentElement;
    const codeText = scriptItem.textContent.replace('نسخ', '').trim();
    navigator.clipboard.writeText(codeText).then(() => {
      button.textContent = 'تم النسخ';
      setTimeout(() => button.textContent = 'نسخ', 1500);
    });
  }

  function filterScripts() {
    const filter = document.getElementById('searchInput').value.toLowerCase();
    const scripts = document.querySelectorAll('.script-item');
    let count = 0;
    scripts.forEach(script => {
      const title = script.querySelector('.script-title').textContent.toLowerCase();
      if(title.includes(filter)) {
        script.style.display = '';
        count++;
      } else {
        script.style.display = 'none';
      }
    });
    document.getElementById('scriptsCount').textContent = `عدد السكربتات: ${count}`;
  }
</script>

</body>
</html>
