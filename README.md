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

        #topBar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background-color: #111;
            padding: 10px 20px;
            border-bottom: 2px solid #444;
        }

        .title {
            font-family: 'Roboto Slab', serif;
            font-size: 24px;
            font-weight: bold;
            color: #FFD700;
        }

        .settings {
            display: flex;
            gap: 10px;
        }

        button {
            background-color: #333;
            color: white;
            border: none;
            padding: 8px 12px;
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

        .footer {
            text-align: center;
            margin-top: 40px;
            font-family: 'Roboto Slab', serif;
            color: #FFD700;
            font-size: 18px;
        }
    </style>
    <script>
        function searchScripts() {
            var input, filter, boxes, text, i;
            input = document.getElementById("searchBox");
            filter = input.value.toUpperCase();
            boxes = document.getElementsByClassName("script-box");
            for (i = 0; i < boxes.length; i++) {
                text = boxes[i].innerText || boxes[i].textContent;
                if (text.toUpperCase().indexOf(filter) > -1) {
                    boxes[i].classList.remove("hidden");
                } else {
                    boxes[i].classList.add("hidden");
                }
            }
        }

        function toggleTheme() {
            const body = document.body;
            body.style.backgroundColor = body.style.backgroundColor === 'white' ? '#181818' : 'white';
            body.style.color = body.style.color === 'black' ? 'white' : 'black';
        }

        // منع النسخ ولقطة الشاشة
        document.addEventListener('contextmenu', e => e.preventDefault());
        document.addEventListener('keydown', e => {
            if (e.key === 'PrintScreen') e.preventDefault();
            if (e.ctrlKey && (e.key === 'u' || e.key === 'U')) e.preventDefault();
        });
    </script>
</head>
<body>

    <div id="topBar">
        <div class="title">مصطفى جلال | Mustafa Jalal</div>
        <div class="settings">
            <button onclick="toggleTheme()">تغيير اللون</button>
            <button onclick="window.location.href='mailto:thesmiths505@gmail.com'">تواصل مع المطور</button>
        </div>
    </div>

    <input type="text" id="searchBox" onkeyup="searchScripts()" placeholder="ابحث عن السكربتات...">

    <div class="script-box" id="emergency-hambuurg">
        <div class="premium-text">Emergency hambuurg</div>
        <h2>باتمان | batman 🦇</h2>
        <textarea readonly>
            loadstring(game:HttpGet("https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe"))()
        </textarea>
    </div>

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

    <div class="footer">
        Tiktok : The_Smiths505
    </div>
</body>
</html>
