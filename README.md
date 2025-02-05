<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Will You Be My Valentine?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #ffebee;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
    }
    .container {
      text-align: center;
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }
    h1 {
      color: #d32f2f;
    }
    .buttons {
      margin-top: 20px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin: 0 10px;
    }
    #yes-btn {
      background-color: #4caf50;
      color: white;
    }
    #no-btn {
      background-color: #f44336;
      color: white;
    }
    .emoji {
      font-size: 48px;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Can you be my Valentine?</h1>
    <div class="buttons">
      <button id="yes-btn">Yes</button>
      <button id="no-btn">No</button>
    </div>
    <div id="emoji" class="emoji"></div>
  </div>

  <script>
    const yesBtn = document.getElementById('yes-btn');
    const noBtn = document.getElementById('no-btn');
    const emoji = document.getElementById('emoji');

    yesBtn.addEventListener('click', () => {
      emoji.textContent = '🎉🥳🎊';
    });

    noBtn.addEventListener('click', () => {
      emoji.textContent = '😢😭😞';
    });
  </script>
</body>
</html>
