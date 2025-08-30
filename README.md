<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Özür Dilerim Sevgilim</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: "Poppins", sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
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
      animation: fadeOut 4s forwards;
    }
    .intro h2 {
      font-size: 3em;
      color: #fff;
      text-shadow: 0 0 20px rgba(255,255,255,0.9);
      animation: zoom 4s ease-in-out;
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

    .container {
      text-align: center;
      background: rgba(255,255,255,0.2);
      padding: 30px;
      border-radius: 25px;
      box-shadow: 0 0 25px rgba(0,0,0,0.3);
      backdrop-filter: blur(12px);
      max-width: 650px;
      animation: fadeIn 2s ease-in-out;
      z-index: 1;
    }
    h1 {
      font-size: 2.8em;
      color: #fff;
      margin-bottom: 15px;
      font-weight: 700;
      text-shadow: 0 0 12px rgba(255,255,255,0.8);
    }
    p {
      font-size: 1.3em;
      color: #fff;
      margin-bottom: 10px;
      font-weight: 400;
    }
    .poem {
      font-size: 1.2em;
      color: #fff;
      font-style: italic;
      white-space: pre-line;
      margin-top: 15px;
      line-height: 1.6;
    }
    .video {
      margin-top: 20px;
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
      width: 250px;
      height: 450px;
      margin-left:auto;
      margin-right:auto;
    }
    .heart {
      position: absolute;
      color: rgba(255, 0, 100, 0.8);
      font-size: 22px;
      animation: floatUp 7s linear infinite;
    }
    @keyframes floatUp {
      0% { transform: translateY(100vh) scale(0.5); opacity: 1; }
      100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
    }
    @keyframes fadeIn {
      0% { opacity: 0; transform: scale(0.8); }
      100% { opacity: 1; transform: scale(1); }
    }
  </style>
</head>
<body>
  <!-- Giriş animasyonu -->
  <div class="intro">
    <h2>Seni Seviyorum ❤️</h2>
  </div>

  <div class="container">
    <h1>Özür Dilerim Sevgilim ❤️</h1>

    <p>Seni üzdüğüm için çok pişmanım...</p>
    <p>Ne olur affet beni, sensiz hayat eksik 💔</p>
    <p>Kalbim sadece sana ait...</p>

    <div class="poem">
      Sensiz olmaz, yüreğim daralır,<br>
      Canıma kıyarım, seni üzmektense…<br>
      Gözlerim dolar, kalbim ağlar,<br>
      Çünkü senin sevginle hayat var… ❤️<br><br>
      Her nefesimde adın yankılanır,<br>
      Kalbimde tek taht kuran sensin,<br>
      Affet beni, aşkım, ne olur,<br>
      Sensiz ben, ben değilim…
    </div>

    <div class="video">
      <iframe width="250" height="450"
        src="https://www.youtube.com/embed/lk95g7LjZ6E?autoplay=1&mute=1&loop=1&playlist=lk95g7LjZ6E"
        title="YouTube Shorts"
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
      heart.style.fontSize = Math.random() * 25 + 15 + "px";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 7000);
    }
    setInterval(createHeart, 400);
  </script>
</body>
</html>
