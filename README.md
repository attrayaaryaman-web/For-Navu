<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>For You, Navu</title>

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', sans-serif;
      color: #fff;
      text-align: center;
    }

    .card {
      background: rgba(255, 255, 255, 0.2);
      padding: 45px;
      border-radius: 25px;
      max-width: 520px;
      box-shadow: 0 25px 50px rgba(0, 0, 0, 0.25);
      backdrop-filter: blur(10px);
    }

    h1 {
      font-size: 2.7em;
      margin-bottom: 10px;
    }

    h2 {
      margin-top: 30px;
      font-size: 1.8em;
    }

    p {
      font-size: 1.25em;
      line-height: 1.7;
      margin-top: 20px;
    }

    .buttons {
      margin-top: 35px;
    }

    button {
      font-size: 1.1em;
      padding: 14px 30px;
      border: none;
      border-radius: 40px;
      cursor: pointer;
      margin: 10px;
      transition: all 0.3s ease;
    }

    .yes {
      background: #fff;
      color: #ff5f7e;
      font-weight: bold;
      box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    }

    .yes:hover {
      transform: scale(1.1);
    }

    .no {
      background: transparent;
      color: #fff;
      border: 2px solid #fff;
    }

    .final {
      display: none;
      margin-top: 30px;
      font-size: 1.3em;
    }

    .heart {
      font-size: 3.5em;
      margin-top: 20px;
      animation: beat 1.2s infinite;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }
  </style>
</head>

<body>
  <div class="card">
    <h1>Navu</h1>

    <p id="message">
      Dekh mainu ni pta ki likha but mai ena kehna ki I want to be part of your whole life.<br><br>
      I will try my best to be the best for ya.<br><br>
      I want to be always with you in any up and down.<br><br>
      I really love you more than anyone.
    </p>

    <h2 id="question">I want you to be next to me, do you feel the same?</h2>

    <div class="buttons" id="buttons">
      <button class="yes" onclick="sayYes()">Yes</button>
      <button class="no" onclick="sayNo()">I need time</button>
    </div>

    <div class="final" id="final">
      <div class="heart">❤️</div>
      <p>
        Thank you for choosing me.<br>
        I promise honesty, care, and a heart that’s always yours.<br>
        I am the happiest person in the world.
      </p>
    </div>
  </div>

  <script>
    function sayYes() {
      document.getElementById("message").innerText =
        "You have no idea how much this means to me.\nEvery heartbeat just got a little louder because of you.";

      document.getElementById("question").innerText =
        "This is the beginning of something beautiful 💖";

      document.getElementById("buttons").style.display = "none";
      document.getElementById("final").style.display = "block";
    }

    function sayNo() {
      document.getElementById("question").innerText =
        "It is okay Navi. If you do not want to be in a relationship with me, I respect and appreciate your decision.";
    }
  </script>
</body>
</html>
