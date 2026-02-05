<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For Princess Sapna 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff6a88, #ff99ac);
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Comic Sans MS', cursive;
      color: white;
      text-align: center;
    }

    .box {
      background: rgba(0, 0, 0, 0.35);
      padding: 35px;
      border-radius: 25px;
      width: 360px;
      box-shadow: 0 0 25px rgba(255, 0, 90, 0.6);
    }

    h2 {
      margin-bottom: 15px;
    }

    button {
      margin-top: 20px;
      padding: 12px 26px;
      border: none;
      border-radius: 30px;
      font-size: 16px;
      cursor: pointer;
      background: #ff2f6d;
      color: white;
      transition: 0.3s;
    }

    button:hover {
      transform: scale(1.1);
      background: #ff0a54;
    }
  </style>
</head>
<body>

  <div class="box">
    <h2 id="question">Hello Princess Sapna 👑💖</h2>
    <p id="text">May I ask you a few magical questions? ✨</p>
    <button onclick="nextQuestion()">Next 💕</button>
  </div>

  <script>
    const questions = [
      "Do you believe that some people enter your life like destiny? 🌙",
      "Do you know you make ordinary moments feel special? 💫",
      "If smiles were stars, would you mind lighting up my sky? ⭐",
      "Do you feel butterflies when someone truly cares for you? 🦋",
      "One last question, straight from my heart… ❤️"
    ];

    let index = 0;

    function nextQuestion() {
      if (index < questions.length) {
        document.getElementById("question").innerText = questions[index];
        document.getElementById("text").innerText = "";
        index++;
      } else {
        document.getElementById("question").innerText =
          "💘 Will you be my Valentine, Princess Sapna, my love? 💘";
        document.getElementById("text").innerText =
          "I promise loyalty, laughter, endless care, and a heart that’s always yours 🥰";
        document.querySelector("button").style.display = "none";
      }
    }
  </script>

</body>
</html>
