<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine's Question</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
            background-color: #f9f9f9;
        }
        h1 {
            color: #e91e63;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            margin: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        #yesBtn {
            background-color: #4caf50;
            color: white;
        }
        #noBtn {
            background-color: #f44336;
            color: white;
        }
        .emoji {
            font-size: 40px;
            margin-top: 20px;
        }
        .results {
            margin-top: 30px;
            font-size: 18px;
            color: #333;
        }
    </style>
</head>
<body>

    <h1>mabyy malapit na po yung valentines day,Can you be my valentine?</h1>
    
    <div class="buttons">
        <button id="yesBtn">Yes</button>
        <button id="noBtn">No</button>
    </div>

    <div class="emoji" id="emoji"></div>

    <div class="results" id="results"></div>

    <script>
        const yesBtn = document.getElementById('yesBtn');
        const noBtn = document.getElementById('noBtn');
        const emoji = document.getElementById('emoji');
        const results = document.getElementById('results');

        yesBtn.addEventListener('click', () => {
            emoji.textContent = '🎉';
            results.textContent = 'Yay! You said Yes!';
        });

        noBtn.addEventListener('click', () => {
            emoji.textContent = '😢';
            results.textContent = 'Aww, you said No...';
        });
    </script>

</body>
</html>
