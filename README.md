<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>George's World</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Fredoka One', sans-serif;
      background-color: #fff0f5;
      color: #000;
      text-align: center;
      padding: 50px;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 0.5em;
    }

    .george {
      width: 120px;
      height: 120px;
      background-color: pink;
      border-radius: 50%;
      margin: 30px auto;
      animation: float 2s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-15px); }
    }

    .buttons {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      margin-top: 40px;
    }

    .btn {
      background: #ff4b81;
      color: white;
      padding: 15px 30px;
      border: none;
      border-radius: 20px;
      font-size: 1.2em;
      cursor: pointer;
      transition: transform 0.2s ease;
      animation: popIn 0.5s ease forwards;
    }

    .btn:hover {
      transform: scale(1.1) rotate(-2deg);
      animation: wiggle 0.3s ease infinite alternate;
    }

    @keyframes popIn {
      0% { transform: scale(0); opacity: 0; }
      100% { transform: scale(1); opacity: 1; }
    }

    @keyframes wiggle {
      from { transform: scale(1.1) rotate(-2deg); }
      to { transform: scale(1.1) rotate(2deg); }
    }

    .btn:active {
      transform: scale(0.95);
    }
  </style>
</head>
<body>

  <h1>Welcome to George's World!</h1>
  <div class="george"></div>
  <p>Check out more George goodness below!</p>

  <div class="buttons">
    <button class="btn" onclick="location.href='https://www.youtube.com/@GeorgeTheCool'">Watch More</button>
    <button class="btn" onclick="location.href='https://x.com/GeorgeTheCoolEH'">Follow on X</button>
    <button class="btn" onclick="location.href='mailto:georgecool.213@gmail.com'">Contact Me</button>
  </div>

</body>
</html>
