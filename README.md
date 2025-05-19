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
    .credits {
      font-size: 12px;
      color: #aaa;
      margin-top: 5px;
      font-family: 'Roboto Slab', serif;
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

  <!-- سكربتاتك نفسها من غير تغيير -->
  <!-- Emergency hambuurg -->
  <div class="script-box">
    <div class="premium-text">Emergency hambuurg</div>
    <h2>باتمان | batman 🦇</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()</textarea>
  </div>

  <!-- Ghost and Fly -->
  <div class="script-box">
    <div class="premium-text">جميع المابات</div>
    <h2>الشبح | Ghost 👻</h2>
    <textarea readonly>loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()</textarea>

    <div class="premium-text">جميع المابات</div>
    <h2>طيران | fly 🕊️</h2>
    <textarea readonly>loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()</textarea>
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

    <h2>رحمه | bang 🔞</h2>
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

    <h2>تغيير سرعة المشي | Speed Hack</h2>
    <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

humanoid.WalkSpeed = 50 -- غيّر الرقم للسرعة اللي تبيها (الافتراضي 16)
    </textarea>
    <div class="credits">مصطفى جلال | Mustafa Jalal</div>

    <h2>تغيير قوة القفز | Jump Power</h2>
    <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

humanoid.JumpPower = 100 -- الافتراضي 50
    </textarea>
    <div class="credits">مصطفى جلال | Mustafa Jalal</div>

    <h2>طيران بسيط | Fly</h2>
    <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local hrp = character:WaitForChild("HumanoidRootPart")

local flying = true
local speed = 50

local UserInputService = game:GetService("UserInputService")

local function fly()
    while flying do
        wait()
        local moveDir = Vector3.new(0,0,0)
        if UserInputService:IsKeyDown(Enum.KeyCode.W) then moveDir = moveDir + workspace.CurrentCamera.CFrame.LookVector end
        if UserInputService:IsKeyDown(Enum.KeyCode.S) then moveDir = moveDir - workspace.CurrentCamera.CFrame.LookVector end
        if UserInputService:IsKeyDown(Enum.KeyCode.A) then moveDir = moveDir - workspace.CurrentCamera.CFrame.RightVector end
        if UserInputService:IsKeyDown(Enum.KeyCode.D) then moveDir = moveDir + workspace.CurrentCamera.CFrame.RightVector end
        hrp.Velocity = moveDir.Unit * speed
    end
end

spawn(fly)
    </textarea>
    <div class="credits">مصطفى جلال | Mustafa Jalal</div>

    <h2>وقف الضرر | God Mode</h2>
    <textarea readonly>
local player = game.Players.Local
