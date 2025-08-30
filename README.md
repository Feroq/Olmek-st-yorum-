<!DOCTYPE html>
<html lang="tr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Özür Dilerim ❤️</title>
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

  .container {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    height: 90%;
    padding: 10px;
  }

  h1 {
    font-size: 2em;
    color: #fff;
    text-shadow: 0 0 12px rgba(255,255,255,0.8);
    margin: 0;
  }

  p {
    font-size: 1em;
    color: #fff;
    margin: 5px 0;
  }

  .poem {
    font-size: 0.95em;
    color: #fff;
    font-style: italic;
    text-align: center;
    margin: 5px 0;
    line-height: 1.3em;
  }

  .video {
    width: 100%;
    max-width: 360px;
    height: 202px; /* 16:9 oranı */
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 0 15px rgba(0,0,0,0.5);
    margin-top: 10px;
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

  @media screen and (max-width: 400px) {
    h1 { font-size: 1.6em; }
    p { font-size: 0.9em; }
    .poem { font-size: 0.85em; }
    .video { max-width: 280px; height: 157px; }
  }
</style>
</head>
<body>

<div class="container">
  <h1>Özür Dilerim, Nehirim ❤️</h1>
  <p>Sensiz hayat eksik, kalbim boş…</p>
  <div class="poem">
    Canıma kıyarım, seni üzmektense…<br>
    Gözlerinle aydınlanır gecem,<br>
    Kalbim sadece senin için atıyor,<br>
    Affet beni, Nehirim… 💔<br>
    Her hatamı unut, birlikte olalım<br>
    Hayatımın anlamı sensin, sevgilim… ❤️
  </div>

  <div class="video">
    <iframe width="100%" height="100%" 
      src="https://www.youtube.com/embed/lk95g7LjZ6E" 
      frameborder="0" 
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
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
