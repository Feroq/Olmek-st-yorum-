<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Özür Dilerim Sevgilim</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: "Poppins", sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      position: relative;
    }
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

    /* Giriş animasyonu */
    .intro {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(255,192,203,0.9);
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 9999;
      animation: fadeOut 3s forwards;
    }
    .intro h2 {
      font-size: 2.2em;
      color: #fff;
      text-shadow: 0 0 15px rgba(255,255,255,0.9);
      animation: zoom 3s ease-in-out;
      text-align: center;
      padding: 0 10px;
    }
    @keyframes zoom {
      0% { transform: scale(0.5); opacity: 0; }
      50% { transform: scale(1.5); opacity: 1; }
      100% { transform: scale(1); opacity: 0; }
    }
    @keyframes fadeOut {
      0% { opacity: 1; }
      90% { opacity: 0; }
      100% { display: none; }
    }

    /* Ana container */
    .container {
      text-align: center;
      width: 100%;
      height: 100%;
      padding: 10px;
      display: flex;
      flex-direction: column;
      justify-content: space-around;
      align-items: center;
      position: relative;
      z-index: 1;
    }

    h1 {
      font-size: 1.8em;
      color: #fff;
      margin: 0;
      font-weight: 700;
      text-shadow: 0 0 12px rgba(255,255,255,0.8);
    }

    p {
      font-size: 1em;
      color: #fff;
      margin: 0;
      font-weight: 400;
      text-align: center;
    }

    .poem {
      font-size: 0.95em;
      color: #fff;
      font-style: italic;
      text-align: center;
      margin: 0;
    }

    .video {
      width: 180px;
      height: 320px;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 0 15px rgba(0,0,0,0.5);
    }

    .heart {
      position: absolute;
      color: rgba(255, 0, 100, 0.8);
      font-size: 18px;
      animation: floatUp 6s linear infinite;
    }
    @keyframes floatUp {
      0% { transform: translateY(100vh) scale(0.5); opacity: 1; }
      100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
    }
  </style>
</head>
<body>
  <!-- Giriş animasyonu -->
  <div class="intro">
    <h2>Seni Seviyorum ❤️</h2>
  </div>

  <div class="container">
    <h1>Özür Dilerim ❤️</h1>
    <p>Sensiz hayat eksik…</p>
    <div class="poem">Canıma kıyarım, seni üzmektense…</div>
    <div class="video">
      <iframe width="180" height="320"
        src="https://www.youtube.com/embed/lk95g7LjZ6E?autoplay=1&mute=1&loop=1&playlist=lk95g7LjZ6E"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        allowfullscreen>
      </iframe>
    </div>
  </div>

  <script>
    function createHeart() {
      const heart = document.createElement("div");
      heart.classList.add("heart");
      heart.innerHTML = "❤️";
      heart.style.left = Math.random() * window.innerWidth + "px";
      heart.style.fontSize = Math.random() * 20 + 12 + "px";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }
    setInterval(createHeart, 400);
  </script>
</body>
</html>
