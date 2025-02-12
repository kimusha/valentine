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
            const botToken = "7716322705:AAFIl_v7D_0NdizS1-amKZpUveJofX3nWug"; // Вставь сюда токен бота
            const chatId = "5209620825"; // Вставь сюда свой Telegram ID
            const message = "Она согласилась пойти в кино! 🎉";

            fetch(`https://api.telegram.org/bot${botToken}/sendMessage?chat_id=${chatId}&text=${encodeURIComponent(message)}`)
                .then(response => {
                    if (response.ok) {
                        window.location.href = "https://t.me/K_k_xxsk"; // Ссылка на твой Telegram
                    } else {
                        throw new Error('Ошибка сети.');
                    }
                })
                .catch(error => {
                    console.error("Ошибка:", error);
                    alert("Произошла ошибка при отправке сообщения.");
                    window.location.href = "https://t.me/K_k_xxsk";
                });
        }
    </script>
</head>
<body>
    <h2>Нужен человек для секретной миссии: взять попкорн и посмотреть новый фильм. ты в деле? 🎬</h2>
    <button onclick="sendMessage()">Да 😊</button>
    <button onclick="window.location.href='sad.html'">Нет 😢</button>
</body>
</html>
