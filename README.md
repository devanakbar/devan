
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nembak Cewek - Trik Romantis</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe4e1;
            padding: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin: 10px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff7f7f;
            color: white;
        }
        .no {
            background-color: #d3d3d3;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>💖 Apakah kamu mau jadi pacarku? 💖</h1>
    <p>Jawab jujur ya!</p>
    <button class="yes" onclick="jawabYa()">Iya, aku mau!</button>
    <button class="no" id="noButton" onmouseover="gerak()">Maaf, nggak bisa...</button>

    <script>
        function jawabYa() {
            alert("Aku tahu kamu akan bilang iya! 🥰 Aku janji akan selalu membahagiakanmu.");
            document.body.innerHTML = "<h1>💍 Selamat, kita resmi jadi pasangan! 💕</h1>";
        }

        function gerak() {
            const noButton = document.getElementById("noButton");
            const x = Math.random() * (window.innerWidth - 100);
            const y = Math.random() * (window.innerHeight - 50);
            noButton.style.left = `${x}px`;
            noButton.style.top = `${y}px`;
        }
    </script>
</body>
</html>
