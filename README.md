<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>20/10 - Gửi Mẹ Thắm 💖</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      color: #333;
      text-align: center;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
      height: 100vh;
    }

    header {
      background-color: rgba(255, 255, 255, 0.3);
      padding: 30px 10px;
      border-bottom: 2px solid #fff;
    }

    h1 {
      font-size: 2.5em;
      color: #d6336c;
      margin: 10px 0;
    }

    .content {
      max-width: 700px;
      margin: 40px auto;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      position: relative;
      z-index: 10;
    }

    .content p {
      font-size: 1.2em;
      line-height: 1.8;
      margin: 20px 0;
    }

    .signature {
      margin-top: 30px;
      font-style: italic;
      color: #444;
    }

    footer {
      margin-top: 40px;
      padding: 10px;
      background-color: rgba(255,255,255,0.3);
      color: #555;
      z-index: 10;
      position: relative;
    }

    img {
      width: 200px;
      border-radius: 50%;
      margin-top: 20px;
    }

    .btn {
      display: inline-block;
      margin-top: 20px;
      background-color: #ff6b81;
      color: white;
      padding: 10px 20px;
      border-radius: 30px;
      text-decoration: none;
      transition: 0.3s;
    }

    .btn:hover {
      background-color: #ff4757;
    }

    /* Ảnh hai bên trang */
    .side-img {
      position: fixed;
      top: 50%;
      width: 180px;
      transform: translateY(-50%);
      border-radius: 15px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.2);
      opacity: 0.9;
      transition: transform 0.5s ease, opacity 0.5s ease;
      z-index: 5;
    }

    .side-img:hover {
      transform: translateY(-50%) scale(1.05);
      opacity: 1;
    }

    .left-img {
      left: 20px;
    }

    .right-img {
      right: 20px;
    }

    /* 🌸 Hiệu ứng hoa rơi */
    .flower {
      position: fixed;
      top: -10px;
      font-size: 20px;
      opacity: 0.8;
      animation: fall linear forwards;
      z-index: 1;
      pointer-events: none;
    }

    @keyframes fall {
      0% {
        transform: translateY(0) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh) rotate(360deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <!-- 🌸 Ảnh trang trí hai bên -->
  <img src="me1.jpg" alt="Mẹ bên trái" class="side-img left-img">
  <img src="me2.jpg" alt="Mẹ bên phải" class="side-img right-img">

  <!-- 🌸 Header -->
  <header>
    <h1>💐 Chúc mừng ngày mẹ Thắm 💐</h1>
    <h2>Gửi đến Mẹ người đẹp nhất trong lòng con</h2>
  </header>

  <!-- 🌸 Nội dung chính -->
  <div class="content">
    <img src="https://cdn.pixabay.com/photo/2016/11/21/15/54/woman-1848949_1280.jpg" alt="Mẹ yêu">
    <p>Mẹ ơi, nhân ngày 20/10, con muốn gửi đến mẹ lời chúc chân thành nhất!  
    Cảm ơn mẹ vì những năm tháng hi sinh, vì tình yêu thương bao la mẹ dành cho con.
    Con biết hiện tại con chưa làm được gì nhiều chỉ có thể tạo trang wed này để gửi lời cảm ơn me.</p>

    <p>Con mong mẹ luôn mạnh khỏe, luôn cười thật tươi, và mãi hạnh phúc bên gia đình nhỏ của mình.  
    Con yêu mẹ rất nhiều! ❤️</p>

    <div class="signature">— Con của mẹ, Vỹ —</div>

    <a class="btn" href="#">💌 Gửi mẹ</a>
  </div>

  <!-- 🌸 Footer -->
  <footer>
    <p>© 2025 - Trang web nhỏ dành tặng mẹ Thắm nhân ngày Phụ nữ Việt Nam 20/10 🌸</p>
  </footer>

  <!-- 🌸 Hiệu ứng hoa rơi bằng JavaScript -->
  <script>
    const flowers = ["🌸", "🌷", "💮", "🌺", "🌻", "🌼"];
    function createFlower() {
      const flower = document.createElement("div");
      flower.classList.add("flower");
      flower.innerText = flowers[Math.floor(Math.random() * flowers.length)];
      flower.style.left = Math.random() * 100 + "vw";
      flower.style.animationDuration = 4 + Math.random() * 5 + "s";
      flower.style.fontSize = 18 + Math.random() * 20 + "px";
      document.body.appendChild(flower);

      setTimeout(() => {
        flower.remove();
      }, 9000);
    }

    setInterval(createFlower, 300);
  </script>

</body>
</html>
