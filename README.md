<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Выбор</title>
    <style>
	body {
            text-align: center;
            font-family: Arial, sans-serif;
            margin-top: 50px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
        }
    </style>
	<script>
        function sendMessage() {
            let botToken = "AAFIl_v7D_0NdizS1-amKZpUveJofX3nWug"; //
            let chatId = "52096208225"; //
            let message = "Она согласилась пойти в кино! 🎉";

            fetch(`https://api.telegram.org/bot${botToken}/sendMessage?chat_id=${chatId}&text=${encodeURIComponent(message)}`)
                .then(response => {
                    window.location.href = "https://t.me/K_k_xxsk"; //
                })
                .catch(error => {
                    console.error("Ошибка:", error);
                    window.location.href = "https://t.me/K_k_xxsk";
                });
        }
    </script>
</head>
<body>
    <h2>Пойдешь со мной на фильм? 🎬</h2>
    <button onclick="window.location.href='https://t.me/K_k_xxsk'">Да 😊</button>
    <button onclick="window.location.href='sad.html'">Нет 😢</button>
</body>
</html>index.html…]()
