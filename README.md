<img width="1840" height="2448" alt="23950" src="https://github.com/user-attachments/assets/177c6994-6fe0-44af-b42a-5e7b1a0844c7" />
# Lucy-love-surprise<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>A Surprise For Lucy ❤️</title>

  <style>
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      font-family: Arial, sans-serif;
      text-align: center;
      color: white;
      overflow: hidden;
    }

    .container {
      padding: 30px;
    }

    h1 {
      font-size: 30px;
    }

    p {
      font-size: 18px;
    }

    .heart {
      font-size: 100px;
      cursor: pointer;
      animation: beat 1s infinite;
      user-select: none;
    }

    @keyframes beat {
      0%, 100% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.25);
      }
    }

    #message {
      display: none;
      margin-top: 25px;
      font-size: 22px;
      line-height: 1.6;
      animation: appear 1s ease-in;
    }

    @keyframes appear {
      from {
        opacity: 0;
        transform: translateY(20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .small {
      margin-top: 25px;
      font-size: 14px;
      opacity: 0.9;
    }
  </style>
</head>

<body>

  <div class="container">

    <h1>Lucy ❤️</h1>

    <p>I have a little surprise for you...</p>

    <div class="heart" onclick="showLove()">❤️</div>

    <div id="message">
      <strong>I LOVE YOU LUCY ❤️</strong>
      <br><br>
      This is from Cliff, your love. 💕
      <br>
      You mean so much to me. 🥰
    </div>

    <div class="small">
      Tap the ❤️
    </div>

  </div>

  <script>
    function showLove() {

      document.getElementById("message").style.display = "block";

      const message =
        "I love you Lucy. This is from Cliff, your love.";

      if ("speechSynthesis" in window) {
        window.speechSynthesis.cancel();

        const voice = new SpeechSynthesisUtterance(message);

        voice.rate = 0.85;
        voice.pitch = 1.1;
        voice.volume = 1;

        window.speechSynthesis.speak(voice);
      }
    }
  </script>

</body>
</html><img width="1840" height="2448" alt="23950" src="https://github.com/user-attachments/assets/0ac30d5d-7c4e-4d1e-b324-5871aae62e1a" />
