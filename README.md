<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>موقع سكربتات روبلوكس</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #1a1a1a;
      color: #f5f5f5;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #333;
      padding: 20px;
      text-align: center;
    }

    h1 {
      color: #ffcc00;
      font-size: 3rem;
    }

    nav {
      background-color: #222;
      padding: 10px;
      text-align: center;
    }

    nav a {
      color: #f5f5f5;
      padding: 10px 20px;
      text-decoration: none;
      font-size: 1.2rem;
      margin: 0 10px;
      border-radius: 5px;
    }

    nav a:hover {
      background-color: #444;
    }

    .container {
      max-width: 1200px;
      margin: 30px auto;
      padding: 20px;
    }

    .script-box {
      background-color: #333;
      border: 1px solid #ffcc00;
      padding: 20px;
      margin-bottom: 30px;
      border-radius: 5px;
    }

    .script-box h2 {
      color: #ffcc00;
      font-size: 2rem;
    }

    .script-box pre {
      background-color: #222;
      padding: 10px;
      border-radius: 5px;
      color: #f5f5f5;
      font-family: monospace;
      font-size: 1rem;
      white-space: pre-wrap;
      word-wrap: break-word;
    }

    footer {
      background-color: #333;
      padding: 20px;
      text-align: center;
      color: #f5f5f5;
    }

    footer a {
      color: #ffcc00;
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <!-- Header Section -->
  <header>
    <h1>موقع سكربتات روبلوكس</h1>
    <p>أفضل السكربتات للألعاب في روبلوكس</p>
  </header>

  <!-- Navigation -->
  <nav>
    <a href="#">الرئيسية</a>
    <a href="#">سكربتات أخرى</a>
    <a href="#">دروس تعليمية</a>
    <a href="#">تواصل معنا</a>
  </nav>

  <!-- Main Content -->
  <div class="container">
    <div class="script-box">
      <h2>سكربت Emergency Hamburger</h2>
      <p>هذا سكربت لإضافة خاصية الهامبرغر الطوارئ في روبلوكس.</p>
      <pre>
-- سكربت Emergency Hamburger
local ReplicatedStorage = game:GetService("ReplicatedStorage")
local EmergencyHamburger = Instance.new("Model")
EmergencyHamburger.Name = "EmergencyHamburger"
EmergencyHamburger.Parent = ReplicatedStorage

local function createHamburger()
    local hamburger = Instance.new("Part")
    hamburger.Size = Vector3.new(4, 0.5, 4)
    hamburger.Position = Vector3.new(0, 5, 0)
    hamburger.Color = Color3.fromRGB(255, 128, 0)
    hamburger.Anchored = true
    hamburger.Parent = EmergencyHamburger
end

createHamburger()
print("سكربت هامبرغر الطوارئ جاهز!")
      </pre>
    </div>

    <!-- Add more script boxes here -->

  </div>

  <!-- Footer Section -->
  <footer>
    <p>© 2025 جميع الحقوق محفوظة. <a href="#">الشروط والأحكام</a></p>
  </footer>

</body>
</html>
</body>
</html>
