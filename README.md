# sorry
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>I'm Really Sorry</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      height: 100vh;
      background: linear-gradient(135deg, #1f1c2c, #928dab);
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      color: white;
    }

    .container {
      text-align: center;
      max-width: 600px;
      padding: 40px;
      animation: fadeIn 1.5s ease;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      animation: slideDown 1s ease;
    }

    h1 span {
      color: #ffb3c6;
    }

    p {
      font-size: 1.1rem;
      opacity: 0.9;
      margin-top: 20px;
      line-height: 1.8;
      animation: fadeInUp 2s ease;
    }

    .heart {
      font-size: 4rem;
      margin: 25px 0;
      animation: heartbeat 1.5s infinite;
    }

    button {
      margin-top: 35px;
      padding: 14px 30px;
      font-size: 1rem;
      border: none;
      border-radius: 30px;
      background: #ffb3c6;
      color: #1f1c2c;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    button:hover {
      transform: scale(1.08);
      background: #ffc8dd;
    }

    .hidden {
      display: none;
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes slideDown {
      from { transform: translateY(-40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes fadeInUp {
      from { transform: translateY(40px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes heartbeat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>I’m <span>Really</span> Sorry</h1>

    <div class="heart">💗</div>

    <p>
      I know I disappeared.<br>
      I know I didn’t talk when I should have.<br><br>
      And honestly… that wasn’t fair to you.
    </p>

    <button onclick="showMessage()">Tap if you forgive me 🥺</button>

    <p id="finalMessage" class="hidden">
      I never meant to make you feel ignored or unimportant.<br>
      You matter more than my silence ever should.<br><br>
      I’m sorry — not just casually sorry,<br>
      but the kind of sorry that means *I’ll do better*. 🌸
    </p>
  </div>

  <script>
    function showMessage() {
      document.getElementById("finalMessage").classList.remove("hidden");
    }
  </script>

</body>
</html>
