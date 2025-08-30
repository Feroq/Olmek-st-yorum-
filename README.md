# Ölmek istiyorum 
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
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }
    .container {
      text-align: center;
      background: rgba(255,255,255,0.2);
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 0 20px rgba(0,0,0,0.2);
      backdrop-filter: blur(10px);
      max-width: 650px;
    }
    h1 {
      font-size: 2.5em;
      color: #fff;
      margin-bottom: 10px;
    }
    p {
      font-size: 1.2em;
      color: #fff;
      margin-bottom: 15px;
    }
    .poem {
      font-size: 1.1em;
      color: #fff;
      font-style: italic;
      white-space: pre-line;
      margin-top: 15px;
    }
    .video {
      margin-top: 20px;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 0 15px rgba(0,0,0,0.4);
      width: 315px;
      height: 560px;
      margin-left:auto;
      margin-right:auto;
    }
    .heart {
      position: absolute;
      color: rgba(255, 0, 100, 0.7);
      font-size: 20px;
      animation: floatUp 6s linear infinite;
    }
    @keyframes floatUp {
      0% { transform: translateY(100vh) scale(0.5); opacity: 1; }
      100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Özür Dilerim Sevgilim ❤️</h1>

    <p>Seni üzdüğüm için çok pişmanım...</p>
    <p>Sensiz geçen her an eksik geliyor 💔</p>
    <p>Kalbim sadece seni istiyor...</p>

    <div class="poem">
      Sensiz olmaz, yüreğim daralır,<br>
      Canıma kıyarım, seni üzmektense…<br>
      Gözlerim dolar, kalbim ağlar,<br>
      Çünkü senin sevginle hayat var… ❤️
    </div>

    <div class="video">
      <iframe width="315" height="560"
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
      heart.style.fontSize = Math.random() * 20 + 15 + "px";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 6000);
    }
    setInterval(createHeart, 500);
  </script>
</body>
</html>
