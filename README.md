# PROJECT
FOR FUN
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semangat Belajar</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #f8f9fa;
            color: #343a40;
        }
        .container {
            text-align: center;
            max-width: 400px;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        input[type="text"] {
            padding: 10px;
            width: 80%;
            margin: 10px 0;
            border: 1px solid #ced4da;
            border-radius: 5px;
            font-size: 16px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #0056b3;
        }
        .message {
            margin-top: 20px;
            font-size: 18px;
            color: #343a40;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Masukkan Namamu</h1>
        <input type="text" id="nameInput" placeholder="Nama kamu...">
        <button onclick="showMessage()">Semangat!</button>
        <p class="message" id="message"></p>
    </div>

    <script>
        function showMessage() {
            const name = document.getElementById("nameInput").value;
            const messageElement = document.getElementById("message");

            if (name) {
                messageElement.innerHTML = `Hai ${name}, tahu nggak? Setiap kali kamu belajar, kamu seperti bintang yang semakin bersinar di langit malamku. Ingat, aku selalu ada untuk mendukungmu, karena aku yakin kamu akan mencapai semua mimpi-mimpimu. Semangat, ya, cintaku!`;
            } else {
                messageElement.innerHTML = "Masukkan namamu dulu, ya!";
            }
        }
    </script>

</body>
</html>
