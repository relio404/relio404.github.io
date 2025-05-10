<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Scripts</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #111;
            color: white;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            padding: 10px;
            text-align: center;
        }
        .container {
            margin: 20px;
        }
        .script-box {
            background-color: #222;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
        }
        h1 {
            font-size: 30px;
            margin-bottom: 20px;
        }
        h2 {
            font-size: 20px;
        }
        button {
            padding: 10px;
            background-color: #444;
            border: none;
            color: white;
            cursor: pointer;
            width: 100%;
            margin-top: 10px;
        }
        button:hover {
            background-color: #666;
        }
        .search-container {
            text-align: center;
            margin: 20px 0;
        }
        input[type="text"] {
            padding: 10px;
            width: 50%;
            font-size: 16px;
            margin-right: 10px;
            border: none;
            border-radius: 5px;
        }
    </style>
</head>

<body>
    <header>
        <h1>My Roblox Scripts</h1>
    </header>

    <div class="search-container">
        <input type="text" id="search" placeholder="Search for scripts..." onkeyup="searchScripts()">
    </div>

    <div class="container" id="scripts-container">
        <h2>Emergency Hambuurg</h2>
        <div class="script-box">
            <p>Batman 🦇</p>
            <button onclick="runScript('https://raw.githubusercontent.com/Farx11122/Dupess/main/SecondDupe')">Run Script</button>
        </div>
        
        <h2>Other Scripts</h2>
        <div class="script-box">
            <p>Ghost 👻</p>
            <button onclick="runScript('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/GhostHub')">Run Script</button>
        </div>
        <div class="script-box">
            <p>Fly 🕊️</p>
            <button onclick="runScript('https://raw.githubusercontent.com/XNEOFF/FlyGuiV3/main/FlyGuiV3.txt')">Run Script</button>
        </div>
    </div>

    <script>
        function runScript(url) {
            var script = document.createElement('script');
            script.src = url;
            document.body.appendChild(script);
        }

        function searchScripts() {
            let searchQuery = document.getElementById("search").value.toLowerCase();
            let scripts = document.querySelectorAll('.container .script-box');
            scripts.forEach(script => {
                let title = script.querySelector('p').textContent.toLowerCase();
                if (title.includes(searchQuery)) {
                    script.style.display = "block";
                } else {
                    script.style.display = "none";
                }
            });
        }
    </script>
</body>

</html>
