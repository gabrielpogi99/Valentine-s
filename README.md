# Valentine-s
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Coleen 💖 Will You Be My Valentine?</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      color: #fff;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .card {
      background: rgba(255, 255, 255, 0.2);
      padding: 30px;
      border-radius: 18px;
      max-width: 420px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.25);
      position: relative;
    }
    h1 {
      font-size: 2.2em;
    }
    p {
      font-size: 1.1em;
      line-height: 1.6;
      white-space: pre-line;
    }
    .buttons {
      margin-top: 25px;
    }
    button {
      border: none;
      padding: 14px 22px;
      font-size: 1em;
      border-radius: 30px;
      cursor: pointer;
      margin: 8px;
      transition: 0.3s;
    }
    #yesBtn {
      background: #ff4d6d;
      color: white;
    }
    #yesBtn:hover {
      transform: scale(1.1);
    }
    #noBtn {
      background: #6c757d;
      color: white;
      position: absolute;
    }
    footer {
      margin-top: 18px;
      font-size: 0.9em;
      opacity: 0.9;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Coleen 💕</h1>
    <p>
I miss you more than I should, but also exactly the right amount 😤
Distance is annoying, but you’re worth every second of it.
You’re my favorite person, my comfort, and the reason my phone feels special.
I love you, Coleen! Mahal kita!
    </p>

    <p><strong>Will you be my Valentine?</strong></p>

    <div class="buttons">
      <button id="yesBtn" onclick="yesClicked()">YES 💖</button>
      <button id="noBtn" onmouseover="moveButton()">No 🙃</button>
    </div>

    <footer>
      Made with love by boching 💌
    </footer>
  </div>

  <script>
    function yesClicked() {
      alert("I love you, Love! 💕\n\nHappy Valentine’s Day!\nCan’t wait to celebrate such occasion with you in the future!");
    }

    function moveButton() {
      const btn = document.getElementById("noBtn");
      const card = document.querySelector(".card");

      const maxX = card.offsetWidth - btn.offsetWidth;
      const maxY = card.offsetHeight - btn.offsetHeight;

      const x = Math.random() * maxX;
      const y = Math.random() * maxY;

      btn.style.left = x + "px";
      btn.style.top = y + "px";
    }
  </script>

</body>
</html>
