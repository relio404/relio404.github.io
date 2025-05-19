<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>سكربتات Roblox</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@700&display=swap" rel="stylesheet" />
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
      min-width: 90px;
      text-align: center;
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
    <input type="text" id="searchBox" onkeyup="searchScripts()" placeholder="ابحث عن السكربتات..." />
    <div id="scriptCount">السكربتات: 0</div>
  </div>

  <!-- سكربتات عامة ومشهورة -->
  <div id="scriptsContainer">

    <div class="script-box" data-name="Speed Hack تغيير سرعة المشي">
      <h2>تغيير سرعة المشي | Speed Hack</h2>
      <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

humanoid.WalkSpeed = 50 -- غيّر الرقم للسرعة اللي تبيها (الافتراضي 16)
      </textarea>
      <div class="credits">مصطفى جلال | Mustafa Jalal</div>
    </div>

    <div class="script-box" data-name="Jump Power تغيير قوة القفز">
      <h2>تغيير قوة القفز | Jump Power</h2>
      <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

humanoid.JumpPower = 100 -- الافتراضي 50
      </textarea>
      <div class="credits">مصطفى جلال | Mustafa Jalal</div>
    </div>

    <div class="script-box" data-name="Fly طيران بسيط">
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
    </div>

    <div class="script-box" data-name="God Mode وقف الضرر">
      <h2>وقف الضرر | God Mode</h2>
      <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

-- تفعيل وضع عدم التعرض للضرر
humanoid.Health = humanoid.MaxHealth
humanoid:GetPropertyChangedSignal("Health"):Connect(function()
    humanoid.Health = humanoid.MaxHealth
end)
      </textarea>
      <div class="credits">مصطفى جلال | Mustafa Jalal</div>
    </div>

    <div class="script-box" data-name="Auto Jump القفز التلقائي">
      <h2>القفز التلقائي | Auto Jump</h2>
      <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

while true do
    wait(0.5)
    if humanoid:GetState() == Enum.HumanoidStateType.Running then
        humanoid.Jump = true
    end
end
      </textarea>
      <div class="credits">مصطفى جلال | Mustafa Jalal</div>
    </div>

    <div class="script-box" data-name="Noclip وضع عدم الاصطدام">
      <h2>وضع عدم الاصطدام | Noclip</h2>
      <textarea readonly>
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

local function noclip()
    for _, part in pairs(character:GetDescendants()) do
        if part:IsA("BasePart") then
            part.CanCollide = false
        end
    end
end

game:GetService("RunService").Stepped:Connect(noclip)
      </textarea>
      <div class="credits">مصطفى جلال | Mustafa Jalal</div>
    </div>

    <div class="script-box" data-name="ESP كشف اللاعبين">
      <h2>كشف اللاعبين | ESP</h2>
      <textarea readonly>
local Players = game:GetService("Players")
local RunService = game:GetService("RunService")

for _, player in pairs(Players:GetPlayers()) do
    if player ~= Players.LocalPlayer then
        local highlight = Instance.new("Highlight")
        highlight.Adornee = player.Character
        highlight.Parent = workspace
        highlight.FillColor = Color3.fromRGB(255, 0, 0)
        highlight.OutlineColor = Color3.fromRGB(0, 0, 0)
    end
end
      </textarea>
      <div class="credits">مصطفى جلال | Mustafa Jalal</div>
    </div>

  </div>

  <footer>
    جميع الحقوق محفوظة &copy; 2025 مصطفى جلال
  </footer>

  <script>
    function toggleTheme() {
      if (document.body.style.backgroundColor === 'white') {
        document.body.style.backgroundColor = '#181818';
        document.body.style.color = 'white';
      } else {
        document.body.style.backgroundColor = 'white';
        document.body.style.color = 'black';
      }
    }

    function disableKeys(e) {
      if (
        e.ctrlKey && 
        (e.key === 'u' || e.key === 'U' || e.key === 's' || e.key === 'S' || e.key === 'p' || e.key === 'P')
      ) {
        return false;
      }
      if (e.key === 'PrintScreen') {
        return false;
      }
      return true;
    }

    function searchScripts() {
      const input = document.getElementById('searchBox').value.toLowerCase();
      const scripts = document.querySelectorAll('.script-box');
      let count = 0;
      scripts.forEach(script => {
        const name = script.getAttribute('data-name').toLowerCase();
        if (name.includes(input)) {
          script.style.display = 'block';
          count++;
        } else {
          script.style.display = 'none';
        }
      });
      document.getElementById('scriptCount').textContent = 'السكربتات: ' + count;
    }

    // تفعيل عداد السكربتات عند تحميل الصفحة
    window.onload = () => {
      searchScripts();
    };
  </script>
</body>
</html>
