<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Roblox Scripts - مصطفى جلال</title>
  <style>
    body {
      margin: 0;
      background-color: #0d1117;
      color: #c9d1d9;
      font-family: 'Segoe UI', sans-serif;
    }

    header {
      background-color: #161b22;
      padding: 1rem;
      text-align: center;
      font-size: 1.5rem;
      color: #58a6ff;
      position: relative;
    }

    /* زر تغيير اللغة */
    .language-switch {
      position: absolute;
      top: 10px;
      right: 20px;
      font-size: 1rem;
      background-color: #21262d;
      padding: 5px 10px;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }

    .search-box {
      text-align: center;
      margin: 1rem;
    }

    .search-box input {
      width: 90%;
      max-width: 400px;
      padding: 0.5rem;
      font-size: 1rem;
      border: none;
      border-radius: 8px;
      background-color: #21262d;
      color: white;
    }

    .container {
      padding: 1rem;
    }

    .category {
      background-color: #161b22;
      padding: 10px;
      margin-bottom: 20px;
      border-radius: 5px;
    }

    .category h3 {
      color: #58a6ff;
    }

    .category button {
      background-color: #21262d;
      color: #58a6ff;
      border: none;
      padding: 10px;
      width: 100%;
      cursor: pointer;
      border-radius: 5px;
    }

    .category button:hover {
      background-color: #58a6ff;
      color: black;
    }

    /* تصميم نافذة تسجيل الدخول */
    .login-container {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(0, 0, 0, 0.8);
      align-items: center;
      justify-content: center;
    }

    .login-box {
      background-color: #21262d;
      padding: 20px;
      border-radius: 10px;
      width: 300px;
    }

    .login-box input {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      background-color: #161b22;
      color: white;
      border: 1px solid #58a6ff;
      border-radius: 5px;
    }

    .login-box button {
      width: 100%;
      padding: 10px;
      background-color: #58a6ff;
      border: none;
      color: white;
      border-radius: 5px;
      cursor: pointer;
    }

    .login-box button:hover {
      background-color: #0d1117;
    }

    /* زر فتح نافذة تسجيل الدخول */
    .login-btn {
      background-color: #58a6ff;
      padding: 10px;
      color: white;
      border-radius: 5px;
      cursor: pointer;
      border: none;
    }

    .login-btn:hover {
      background-color: #0d1117;
    }
  </style>
</head>
<body>

  <!-- Header Section -->
  <header>
    <span>Roblox Scripts - مصطفى جلال</span>
    <button class="language-switch" onclick="toggleLanguage()">Change to Arabic</button>
  </header>

  <!-- Search Box -->
  <div class="search-box">
    <input type="text" id="search" placeholder="Search for scripts...">
  </div>

  <!-- Container for Categories -->
  <div class="container">
    <div class="category">
      <h3>Emergency Hamburg Script - باتمان | Batman 🦇</h3>
      <button onclick="openScript('EmergencyHamburgScript')">Open Script</button>
    </div>

    <div class="category">
      <h3>Other Scripts - الشبح | Ghost 👻</h3>
      <button onclick="openScript('GhostScript')">Open Script</button>
    </div>

    <div class="category">
      <h3>Fly Script - طيران | fly 🕊️</h3>
      <button onclick="openScript('FlyScript')">Open Script</button>
    </div>
  </div>

  <!-- Login Modal -->
  <div class="login-container" id="loginContainer">
    <div class="login-box">
      <input type="email" id="email" placeholder="Enter your email">
      <input type="password" id="password" placeholder="Enter your password">
      <button onclick="login()">Login with Email</button>
      <button onclick="loginWithGoogle()">Login with Google</button>
    </div>
  </div>

  <!-- Login Button -->
  <button class="login-btn" onclick="showLogin()">Login / Sign Up</button>

  <script>
    // Toggle between languages
    function toggleLanguage() {
      const header = document.querySelector('header span');
      const languageSwitch = document.querySelector('.language-switch');

      if (languageSwitch.innerHTML === 'Change to Arabic') {
        header.innerHTML = 'سكربتات روبلوكس - مصطفى جلال';
        languageSwitch.innerHTML = 'تغيير إلى الإنجليزية';
      } else {
        header.innerHTML = 'Roblox Scripts - مصطفى جلال';
        languageSwitch.innerHTML = 'Change to Arabic';
      }
    }

    // Show Login Modal
    function showLogin() {
      document.getElementById('loginContainer').style.display = 'flex';
    }

    // Hide Login Modal
    function hideLogin() {
      document.getElementById('loginContainer').style.display = 'none';
    }

    // Simulate Login
    function login() {
      const email = document.getElementById('email').value;
      const password = document.getElementById('password').value;

      alert(`Logged in with email: ${email}`);
      hideLogin();
    }

    // Simulate Google Login
    function loginWithGoogle() {
      alert('Logged in with Google!');
      hideLogin();
    }

    // Open Script
    function openScript(scriptName) {
      alert(`Opening script: ${scriptName}`);
      // هنا يمكنك إضافة كود لفتح السكربت في نافذة منبثقة أو لتعديله
    }
  </script>
</body>
</html>
