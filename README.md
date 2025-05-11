<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>سكربتات Roblox</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@700&display=swap" rel="stylesheet">
  <style>
    body {
      background-color: #181818;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
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

    .section-title {
      font-family: 'Roboto Slab', serif;
      font-size: 22px;
      font-weight: bold;
      color: #FFD700;
      text-align: center;
      margin-bottom: 10px;
    }
  </style>
</head>
<body>

  <!-- زر تسجيل الدخول -->
  <div style="text-align: center; margin-bottom: 20px;">
    <button onclick="loginWithGoogle()" style="padding: 10px 20px; background-color: #4285F4; color: white; border: none; border-radius: 5px; font-size: 16px;">
      تسجيل الدخول باستخدام Google
    </button>
    <p id="user-info" style="margin-top: 10px;"></p>
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

  <script>
    // دالة البحث لتصفية السكربتات
    function searchScripts() {
      var input = document.getElementById("searchBox");
      var filter = input.value.toUpperCase();
      var boxes = document.getElementsByClassName("script-box");

      for (let i = 0; i < boxes.length; i++) {
        let text = boxes[i].innerText || boxes[i].textContent;
        if (text.toUpperCase().indexOf(filter) > -1) {
          boxes[i].classList.remove("hidden");
        } else {
          boxes[i].classList.add("hidden");
        }
      }
    }
  </script>

  <!-- Firebase Auth + Google Sign-In -->
  <script type="module">
    import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-app.js";
    import { getAuth, signInWithPopup, GoogleAuthProvider, onAuthStateChanged, signOut } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-auth.js";

    const firebaseConfig = {
      apiKey: "AIzaSyB0tRNgdTJNvJ9XWUbFZSpM8fjGbEiEN84",
      authDomain: "jfjfjfhdud-47f01.firebaseapp.com",
      projectId: "jfjfjfhdud-47f01",
      storageBucket: "jfjfjfhdud-47f01.firebasestorage.app",
      messagingSenderId: "485677364722",
      appId: "1:485677364722:web:6e9d6e403483b4eaf8a76b",
      measurementId: "G-MGC8VB54S4"
    };

    const app = initializeApp(firebaseConfig);
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider();

    window.loginWithGoogle = () => {
      signInWithPopup(auth, provider)
        .then((result) => {
          const user = result.user;
          document.getElementById("user-info").innerText = "مرحباً " + user.displayName;
        }).catch((error) => {
          alert("خطأ في تسجيل الدخول: " + error.message);
        });
    };

    onAuthStateChanged(auth, (user) => {
      if (user) {
        document.getElementById("user-info").innerText = "مرحباً " + user.displayName;
      }
    });

    window.logout = () => {
      signOut(auth).then(() => {
        document.getElementById("user-info").innerText = "";
      });
    };
  </script>

</body>
</html>
