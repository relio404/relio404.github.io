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

    <!-- خانة مصطفى جلال | Mustafa Jalal -->
    <div class="script-box" id="mustafa-jalal">
        <div class="premium-text">مصطفى جلال | Mustafa Jalal</div>
        <h2>سكربت خاص</h2>
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
            var input, filter, boxes, text, i;
            input = document.getElementById("searchBox");
            filter = input.value.toUpperCase();
            boxes = document.getElementsByClassName("script-box");

            // تصفية كل خانة من السكربتات
            for (i = 0; i < boxes.length; i++) {
                // جمع النصوص التي ستؤخذ في الحسبان أثناء البحث
                text = boxes[i].innerText || boxes[i].textContent;

                // إذا كانت النصوص تتضمن النص المدخل، نقوم بعرضها، وإذا لا نقوم بإخفائها
                if (text.toUpperCase().indexOf(filter) > -1) {
                    boxes[i].classList.remove("hidden");
                } else {
                boxes[i].classList.add("hidden");
                }
            }
        }
    </script>

</body>
</html>
