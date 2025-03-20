# Barisalimmi
<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Barışalım mı bebeğim?</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            margin-top: 100px;
        }
        h1 {
            font-size: 28px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 20px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        #yes {
            background-color: green;
            color: white;
        }
        #no {
            background-color: red;
            color: white;
            position: absolute;
        }
        #flower {
            display: none;
            margin-top: 20px;
        }
    </style>
</head>
<body>

    <h1>Barışalım mı bebeğim?</h1>
    <div class="buttons">
        <button id="yes" onclick="accept()">Evet</button>
        <button id="no" onmouseover="moveNo()">Hayır</button>
    </div>

    <div id="flower">
        <img src="https://www.pngmart.com/files/1/Flower-PNG-Transparent-Image.png" alt="Çiçek" width="200">
        <h2>Teşekkürler bitanemm ❤️</h2>
    </div>

    <script>
        function accept() {
            document.querySelector('.buttons').style.display = 'none';
            document.getElementById('flower').style.display = 'block';
        }

        function moveNo() {
            let noButton = document.getElementById('no');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 100);
            noButton.style.left = x + 'px';
            noButton.style.top = y + 'px';
        }
    </script>

</body>
</html>
