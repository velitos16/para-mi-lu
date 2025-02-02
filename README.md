<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>San Valentino - Una Richiesta Speciale</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: url('https://staticfanpage.akamaized.net/wp-content/uploads/sites/34/2024/11/lunapienapixa1411-1200x675.jpg') no-repeat center center fixed;
      background-size: cover;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      color: #fff;
      text-align: center;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 0.5em;
    }
    .btn-container {
      display: flex;
      gap: 20px;
      margin-bottom: 1em;
    }
    button {
      background: #fff;
      color: #f06292;
      border: none;
      padding: 1em 2em;
      font-size: 1.2em;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #f8bbd0;
    }
    .message {
      font-size: 1.5em;
      display: none;
      margin-top: 20px;
    }
  </style>
</head>
<body>
  <h1>mi niña… ¿quieres ser mi San Valentín?</h1>
  <div class="btn-container">
    <button id="yesBtn">Sí</button>
    <button id="noBtn">No</button>
  </div>
  <div class="message" id="message"></div>
  
  <script>
    const yesBtn = document.getElementById("yesBtn");
    const noBtn = document.getElementById("noBtn");
    const messageDiv = document.getElementById("message");
    let noClickCount = 0;

    yesBtn.addEventListener("click", function() {
      messageDiv.textContent = "yeyeyey gachassss mi niña me haces feliz♥️ (sabía que ibas a decir que sí eheheheh😌)";
      messageDiv.style.display = "block";
    });

    noBtn.addEventListener("click", function() {
      noClickCount++;
      if (noClickCount === 1) {
        messageDiv.textContent = "ay nuuu ¿por qué?";
      } else if (noClickCount === 2) {
        messageDiv.textContent = "qué mala…";
      } else if (noClickCount === 3) {
        messageDiv.textContent = "está bien, no me quieres, ya vi🥺";
      } else if (noClickCount >= 4) {
        messageDiv.textContent = "no me importa, estás obligada a decir que sí, así que aprieta el otro botón, gracias😌🔪";
      }
      messageDiv.style.display = "block";
    });
  </script>
</body>
</html>
