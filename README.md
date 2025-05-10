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

        #top-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }

        #settings {
            cursor: pointer;
            font-size: 16px;
            color: #FFD700;
        }

        .footer {
            margin-top: 40px;
            text-align: center;
            font-size: 14px;
            color: #ccc;
        }
    </style>
    <script>
        // منع النسخ ولقطات الشاشة
        document.addEventListener('contextmenu', event => event.preventDefault());
        document.addEventListener('keydown', function (e) {
            if ((e.ctrlKey && e.key === 'u') || (e.key === 'PrintScreen') || (e.ctrlKey && e.key === 'c')) {
                e.preventDefault();
            }
        });
    </script>
</head>
<body>
    <div id="top-bar">
        <div class="premium-text">مصطفى جلال | Mustafa Jalal</div>
        <div id="settings" onclick="toggleSettings()">⚙️ الإعدادات</div>
    </div>

    <!-- إعدادات -->
    <div id="settingsPanel" class="hidden" style="margin-bottom: 20px;">
        <button onclick="toggleTheme()">تغيير اللون</button>
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

    <!-- تذييل -->
    <div class="footer">
        <p>Tiktok : The_Smiths505</p>
        <p>تواصل مع المطور: <a href="mailto:relio201277@gmail.com" style="color: #FFD700;">relio201277@gmail.com</a></p>
    </div>

    <script>
        function searchScripts() {
            var input = document.getElementById("searchBox");
            var filter = input.value.toUpperCase();
            var boxes = document.getElementsByClassName("script-box");

            for (var i = 0; i < boxes.length; i++) {
                var text = boxes[i].innerText || boxes[i].textContent;
                if (text.toUpperCase().indexOf(filter) > -1) {
                    boxes[i].classList.remove("hidden");
                } else {
                    boxes[i].classList.add("hidden");
                }
            }
        }

        function toggleSettings() {
            var panel = document.getElementById("settingsPanel");
            panel.classList.toggle("hidden");
        }

        function toggleTheme() {
            var body = document.body;
            if (body.style.backgroundColor === 'white') {
                body.style.backgroundColor = '#181818';
                body.style.color = 'white';
            } else {
                body.style.backgroundColor = 'white';
                body.style.color = 'black';
            }
        }
    </script>
</body>
</html>
