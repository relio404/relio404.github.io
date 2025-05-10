<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mustafa Jalal | مصطفى جلال - Roblox Scripts</title>
  <style>
    body {
      background-color: #181818;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
    }
    .navbar {
      background-color: #181818;
      padding: 15px;
      text-align: center;
    }
    .navbar a {
      color: white;
      text-decoration: none;
      font-size: 20px;
      margin: 0 15px;
    }
    .search-bar {
      margin-top: 20px;
      display: flex;
      justify-content: center;
    }
    .search-bar input {
      padding: 10px;
      font-size: 16px;
      width: 300px;
      border: none;
      border-radius: 5px;
      margin-right: 10px;
    }
    .search-bar button {
      padding: 10px;
      background-color: #0D74FF;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .script-container {
      margin: 20px auto;
      width: 80%;
      text-align: center;
    }
    .script-box {
      background-color: #222222;
      padding: 15px;
      border-radius: 10px;
      margin-bottom: 15px;
      width: 100%;
    }
    .script-title {
      font-size: 20px;
      font-weight: bold;
      margin-bottom: 10px;
    }
    .script-code {
      background-color: #000;
      color: #0D74FF;
      padding: 15px;
      border-radius: 10px;
      font-family: 'Courier New', monospace;
      white-space: pre-wrap;
    }
    .comment-section {
      margin-top: 20px;
    }
    .comment-box {
      margin: 10px auto;
      padding: 10px;
      background-color: #333;
      width: 80%;
      border-radius: 5px;
      font-size: 16px;
      color: white;
    }
    .btn-login {
      margin-top: 20px;
      background-color: #0D74FF;
      padding: 10px 20px;
      border-radius: 5px;
      color: white;
      font-size: 18px;
      cursor: pointer;
    }
    .btn-login:hover {
      background-color: #0859c0;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <div class="navbar">
    <a href="#">Home</a>
    <a href="#">Scripts</a>
    <a href="#">About</a>
  </div>

  <!-- Search Bar -->
  <div class="search-bar">
    <input type="text" id="search" placeholder="Search for scripts...">
    <button onclick="searchScript()">Search</button>
  </div>

  <!-- Emergency Hambuurg Section -->
  <div class="script-container">
    <div class="script-box">
      <div class="script-title">باتمان | Batman 🦇</div>
      <div class="script-title">Emergency Hambuurg | إيميرجنسى هامبورغ 🍔</div>
      <div class="script-code">
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()
      </div>
      <div class="comment-section">
        <div class="comment-box">Comment 1: Great for emergencies!</div>
        <div class="comment-box">Comment 2: Useful in game!</div>
      </div>
    </div>
  </div>

  <!-- Other Scripts Section -->
  <div class="script-container">
    <div class="script-box">
      <div class="script-title">Other Scripts | سكربتات أخرى</div>
      <div class="script-code">
        <b>طيران | Fly 🕊️</b><br>
        loadstring(game:HttpGet("https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt"))()<br><br>
        <b>الشبح | Ghost 👻</b><br>
        loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub'))()
      </div>
      <div class="comment-section">
        <div class="comment-box">Comment 1: Fly script works great!</div>
        <div class="comment-box">Comment 2: Ghost is so cool!</div>
      </div>
    </div>
  </div>

  <!-- Login Button -->
  <div class="btn-login" onclick="login()">Login with Google</div>

  <script>
    function searchScript() {
      let searchTerm = document.getElementById('search').value.toLowerCase();
      let scriptBoxes = document.querySelectorAll('.script-box');

      scriptBoxes.forEach(box => {
        let title = box.querySelector('.script-title').textContent.toLowerCase();
        if (title.includes(searchTerm)) {
          box.style.display = 'block';
        } else {
          box.style.display = 'none';
        }
      });
    }

    function login() {
      alert('Login functionality will be implemented.');
    }
  </script>

</body>
</html>
