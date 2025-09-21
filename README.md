# 21septiembre_index.html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Feliz 21 de Septiembre 🌼</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: radial-gradient(circle, #fffde7, #fff8dc);
      font-family: 'Segoe UI', sans-serif;
      text-align: center;
      overflow: hidden;
    }

    h1 {
      margin-top: 60px;
      color: #e6b800;
      font-size: 3.2em;
      animation: fadeInDrop 2s ease-out;
    }

    .epic-text {
      font-size: 2em;
      font-weight: bold;
      color: #ffcc00;
      text-shadow: 0 0 15px #ffd700, 0 0 30px #fbc02d;
      animation: glow 2s ease-in-out infinite alternate, fadeInZoom 2.5s ease-out;
    }

    p {
      font-size: 1.4em;
      color: #5c4033;
      max-width: 600px;
      margin: 20px auto;
      animation: fadeIn 3s ease-out;
    }

    .flower {
      position: absolute;
      width: 60px;
      height: 60px;
      background: radial-gradient(circle at center, #ffeb3b, #fbc02d);
      border-radius: 50%;
      animation: float 10s infinite ease-in-out;
    }

    .footer {
      position: absolute;
      bottom: 20px;
      width: 100%;
      color: #8b4513;
      font-style: italic;
      font-size: 1.1em;
      animation: fadeIn 4s ease-out;
    }

    @keyframes float {
      0% {
        transform: translateY(0) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-100vh) rotate(360deg);
        opacity: 0;
      }
    }

    @keyframes glow {
      from {
        text-shadow: 0 0 10px #fbc02d, 0 0 20px #fdd835;
      }
      to {
        text-shadow: 0 0 20px #ffeb3b, 0 0 40px #ffeb3b;
      }
    }

    @keyframes fadeInDrop {
      from {
        opacity: 0;
        transform: translateY(-50px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @keyframes fadeInZoom {
      from {
        opacity: 0;
        transform: scale(0.7);
      }
      to {
        opacity: 1;
        transform: scale(1);
      }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <h1>🌼 FELIZ 21 DE SEPTIEMBRE 🌼</h1>
  <div class="epic-text">Estas flores son para ti 💛</div>
  <p>
    Que esta primavera te llene de luz, amor y momentos inolvidables.<br>
    Como estas flores, deseo que cada día florezca con alegría en tu vida.
  </p>

  <div class="footer">Con mucho cariño, tu persona especial 🌻</div>

  <script>
    // Generar flores aleatorias
    for (let i = 0; i < 60; i++) {
      const flower = document.createElement("div");
      flower.classList.add("flower");
      flower.style.left = Math.random() * 100 + "vw";
      flower.style.top = Math.random() * 100 + 100 + "vh";
      flower.style.animationDuration = 5 + Math.random() * 5 + "s";
      flower.style.opacity = Math.random();
      document.body.appendChild(flower);
    }
  </script>
</body>
</html>

