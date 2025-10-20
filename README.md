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
      font-size: 2em;
      color: #d6336c;
      margin: 10px 0;
    }

    .content {
      max-width: 90%;
      margin: 30px auto;
      background-color: rgba(255, 255, 255, 0.85);
      padding: 25px;
      border-radius: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
      position: relative;
      z-index: 10;
    }

    .content p {
      font-size: 1.1em;
      line-height: 1.6;
      margin: 15px 0;
    }

    .signature {
      margin-top: 20px;
      font-style: italic;
      color: #444;
    }

    footer {
      margin-top: 30px;
      padding: 10px;
      background-color: rgba(255,255,255,0.3);
      color: #555;
      z-index: 10;
      position: relative;
      font-size: 0.9em;
    }

    img {
      width: 150px;
      border-radius: 50%;
      margin-top: 10px;
    }

    .btn {
      display: inline-block;
      margin-top: 15px;
      background-color: #ff6b81;
      color: white;
      padding: 10px 25px;
      border-radius: 30px;
      text-decoration: none;
      transition: 0.3s;
      cursor: pointer;
      font-size: 1em;
    }

    .btn:hover {
      background-color: #ff4757;
    }

    /* 🌸 Ảnh overlay chính giữa */
    .overlay {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: rgba(255, 240, 245, 0.96);
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      pointer-events: none;
      transition: opacity 1s ease;
      z-index: 100;
    }

    .overlay.show {
      opacity: 1;
      pointer-events: auto;
      animation: fadeInBg 1.2s ease forwards;
    }

    .overlay img {
      width: 0;
      border-radius: 20px;
      box-shadow: 0 8px 25px rgba(0,0,0,0.3);
      opacity: 0;
      transform: scale(0.5);
      transition: all 1.5s ease;
      max-width: 80%;
      height: auto;
    }

    .overlay.show img {
      width: 280px;
      opacity: 1;
      transform: scale(1);
    }

    @keyframes fadeInBg {
      0% { background-color: rgba(255, 240, 245, 0); }
      100% { background-color: rgba(255, 240, 245, 0.96); }
    }

    /* 🌸 Hoa rơi */
    .flower {
      position: fixed;
      top: -10px;
      font-size: 18px;
      opacity: 0.8;
      animation: fall linear forwards;
      z-index: 1;
      pointer-events: none;
    }

    @keyframes fall {
      0% { transform: translateY(0) rotate(0deg); opacity: 1; }
      100% { transform: translateY(100vh) rotate(360deg); opacity: 0; }
    }

  </style>
</head>
<body>

  <!-- 🌸 Ảnh overlay chính giữa -->
  <div class="overlay" id="overlay">
    <img src="me1.jpg" alt="Mẹ yêu nhất đời">
  </div>

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
    Con biết hiện tại con chưa làm được gì nhiều chỉ có thể tạo trang web này để gửi lời cảm ơn mẹ.</p>

    <p>Con mong mẹ luôn mạnh khỏe, luôn cười thật tươi, và mãi hạnh phúc bên gia đình nhỏ của mình.  
    Con yêu mẹ rất nhiều! ❤️</p>

    <div class="signature">— Con của mẹ, Vỹ —</div>

    <a class="btn" id="revealBtn">💌 Gửi mẹ</a>
  </div>

  <!-- 🌸 Footer -->
  <footer>
    <p>© 2025 - Trang web nhỏ dành tặng mẹ Thắm nhân ngày Phụ nữ Việt Nam 20/10 🌸</p>
  </footer>

  <!-- 🌸 Hiệu ứng hoa rơi -->
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
      setTimeout(() => flower.remove(), 9000);
    }
    setInterval(createFlower, 300);

    // Khi ấn nút -> hiện overlay ảnh giữa màn hình
    const btn = document.getElementById("revealBtn");
    const overlay = document.getElementById("overlay");

    btn.addEventListener("click", () => {
      overlay.classList.add("show");
      btn.innerText = "🌷 Cảm ơn mẹ 🌷";
      btn.style.backgroundColor = "#ff85a2";
      btn.style.cursor = "default";
      btn.disabled = true;
    });
  </script>

</body>
</html>
