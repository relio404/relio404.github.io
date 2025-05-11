<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>سكربتات Roblox</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@700&display=swap" rel="stylesheet">
  <script type="module">
    // Firebase
    import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-app.js";
    import { getAuth, signInWithPopup, GoogleAuthProvider, onAuthStateChanged, signOut } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-auth.js";

    const firebaseConfig = {
      apiKey: "AIzaSyB0tRNgdTJNvJ9XWUbFZSpM8fjGbEiEN84",
      authDomain: "jfjfjfhdud-47f01.firebaseapp.com",
      projectId: "jfjfjfhdud-47f01",
      storageBucket: "jfjfjfhdud-47f01.appspot.com",
      messagingSenderId: "485677364722",
      appId: "1:485677364722:web:6e9d6e403483b4eaf8a76b",
      measurementId: "G-MGC8VB54S4"
    };

    const app = initializeApp(firebaseConfig);
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider();

    document.addEventListener("DOMContentLoaded", () => {
      const loginBtn = document.getElementById("loginBtn");
      const logoutBtn = document.getElementById("logoutBtn");
      const userInfo = document.getElementById("userInfo");

      loginBtn.onclick = () => {
        signInWithPopup(auth, provider)
          .then((result) => {
            const user = result.user;
            userInfo.textContent = `مرحباً، ${user.displayName}`;
            loginBtn.style.display = "none";
            logoutBtn.style.display = "inline-block";
          }).catch((error) => {
            alert("حدث خطأ أثناء تسجيل الدخول");
          });
      };

      logoutBtn.onclick = () => {
        signOut(auth).then(() => {
          userInfo.textContent = "";
          loginBtn.style.display = "inline-block";
          logoutBtn.style.display = "none";
        });
      };

      onAuthStateChanged(auth, (user) => {
        if (user) {
          userInfo.textContent = `مرحباً، ${user.displayName}`;
          loginBtn.style.display = "none";
          logoutBtn.style.display = "inline-block";
        } else {
          userInfo.textContent = "";
          loginBtn.style.display = "inline-block";
          logoutBtn.style.display = "none";
        }
      });
    });
  </script>
  <style>
    body {
      background-color: #181818;
      color: white;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
    }

    #loginContainer {
      position: absolute;
      top: 20px;
      left: 20px;
      display: flex;
      align-items: center;
      gap: 10px;
    }

    #loginBtn, #logoutBtn {
      background-color: #333;
      color: white;
      border: none;
      padding: 8px 16px;
      border-radius: 6px;
      cursor: pointer;
      font-weight: bold;
    }

    #userInfo {
      font-weight: bold;
      color: #FFD700;
    }

    /* بقية تنسيق السكربتات */
  </style>
</head>
<body>

  <!-- تسجيل الدخول -->
  <div id="loginContainer">
    <button id="loginBtn">تسجيل الدخول بـ Google</button>
    <button id="logoutBtn" style="display:none;">تسجيل خروج</button>
    <div id="userInfo"></div>
  </div>

  <!-- المحتوى الأصلي هنا... ضع سكربتاتك وأي عناصر تحتها -->

</body>
</html>
