<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Камень-Ножницы-Бумага</title>
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background: #f0f0f0; padding: 20px; }
        button { font-size: 18px; padding: 10px 20px; margin: 10px; border: none; border-radius: 5px; background: #0088cc; color: white; cursor: pointer; }
        button:hover { background: #006699; }
        #result { font-size: 24px; margin: 20px; color: #333; }
        #score { font-size: 16px; margin: 10px; }
    </style>
</head>
<body>
    <h1>Камень-Ножницы-Бумага</h1>
    <p>Выбери свой ход:</p>
    <button onclick="play('rock')">🪨 Камень</button>
    <button onclick="play('paper')">📄 Бумага</button>
    <button onclick="play('scissors')">✂️ Ножницы</button>
    
    <div id="result"></div>
    <div id="score">Твои очки: 0 | Очки ИИ: 0</div>

    <script>
        let userScore = 0;
        let aiScore = 0;

        // Базовая поддержка Telegram Web App
        if (window.Telegram && window.Telegram.WebApp) {
            Telegram.WebApp.ready();
            Telegram.WebApp.expand(); // Расширяем на весь экран
            document.body.style.background = Telegram.WebApp.themeParams.bg_color || '#f0f0f0';
        }

        function play(userChoice) {
            const choices = ['rock', 'paper', 'scissors'];
            const aiChoice = choices[Math.floor(Math.random() * 3)];

            let result = '';
            if (userChoice === aiChoice) {
                result = `Ничья! Оба выбрали ${getEmoji(userChoice)}.`;
            } else if (
                (userChoice === 'rock' && aiChoice === 'scissors') ||
                (userChoice === 'paper' && aiChoice === 'rock') ||
                (userChoice === 'scissors' && aiChoice === 'paper')
            ) {
                result = `Ты выиграл! ${getEmoji(userChoice)} бьёт ${getEmoji(aiChoice)}.`;
                userScore++;
            } else {
                result = `ИИ выиграл! ${getEmoji(aiChoice)} бьёт ${getEmoji(userChoice)}.`;
                aiScore++;
            }

            document.getElementById('result').innerHTML = `${result}<br>Твой ход: ${getEmoji(userChoice)} | Ход ИИ: ${getEmoji(aiChoice)}`;
            document.getElementById('score').innerHTML = `Твои очки: ${userScore} | Очки ИИ: ${aiScore}`;

            // В Telegram: отправляем результат в чат (опционально)
            if (window.Telegram && window.Telegram.WebApp) {
                Telegram.WebApp.sendData(JSON.stringify({ score: userScore, result: result }));
            }
        }

        function getEmoji(choice) {
            switch (choice) {
                case 'rock': return '🪨';
                case 'paper': return '📄';
                case 'scissors': return '✂️';
                default: return '';
            }
        }
    </script>
</body>
</html>
