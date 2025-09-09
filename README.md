<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>¿Quieres ser mi novia?</title>
  <style>
    body {
      background: linear-gradient(to right, #ffdde1, #ee9ca7);
      font-family: 'Arial', sans-serif;
      text-align: center;
      padding: 50px;
      color: #333;
      position: relative;
      overflow: hidden;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 20px;
    }
    p {
      font-size: 1.2em;
      margin-bottom: 40px;
    }
    .btn {
      font-size: 1.2em;
      padding: 10px 20px;
      background-color: #ff5e78;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      margin: 10px;
      position: relative;
    }
    #noBtn {
      position: absolute;
    }
  </style>
</head>
<body>
  <h1>Hola 💕</h1>
  <p>Desde hace tiempo quería decirte algo muy especial...</p>
  <h1>¿Quieres ser mi novia? 💖</h1>

  <button class="btn" onclick="alert('¡Gracias! Me haces muy feliz 😊')">Sí, quiero 💘</button>
  <button class="btn" id="noBtn">No 😅</button>

  <script>
    const noBtn = document.getElementById('noBtn');

    function moveButton() {
      const x = Math.random() * (window.innerWidth - noBtn.offsetWidth);
      const y = Math.random() * (window.innerHeight - noBtn.offsetHeight);
      noBtn.style.left = `${x}px`;
      noBtn.style.top = `${y}px`;
    }

    noBtn.addEventListener('mouseover', moveButton);
  </script>
</body>
</html>
