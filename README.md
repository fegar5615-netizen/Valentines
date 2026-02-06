
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Hey Sediq 💌</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      background: black;
      color: white;
      font-family: 'Segoe UI', sans-serif;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      overflow: hidden;
    }

    .card {
      max-width: 400px;
      padding: 30px;
    }

    h1 {
      font-size: 2.2rem;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.1rem;
      opacity: 0.9;
    }

    .buttons {
      margin-top: 30px;
      position: relative;
      height: 150px;
    }

    button {
      padding: 12px 22px;
      font-size: 1rem;
      border-radius: 25px;
      border: none;
      cursor: pointer;
    }

    #yes {
      background: #ff4d6d;
      color: white;
      margin-right: 10px;
    }

    #no {
      background: white;
      color: black;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Sediq 🖤</h1>
    <p>
      So… I’ve been thinking about you a lot lately 👀<br><br>
      And I was wondering… will you be my Valentine? 💘
    </p>

    <div class="buttons">
      <button id="yes" onclick="yesClicked()">Yes 💕</button>
      <button id="no" onmouseover="moveNo()">No 😅</button>
    </div>
  </div>

  <script>
    function moveNo() {
      const noBtn = document.getElementById("no");
      const x = Math.random() * 250;
      const y = Math.random() * 120;
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }

    function yesClicked() {
      document.body.innerHTML = `
        <div style="text-align:center; color:white;">
          <h1>Yayyy 💖</h1>
          <p>
            Okay so it’s official now 😌<br>
            Valentine secured 💌
          </p>
          <p style="margin-top:20px;">
            Can’t wait to spend it with you, Sediq 🖤
          </p>
        </div>
      `;
    }
  </script>

</body>
</html>