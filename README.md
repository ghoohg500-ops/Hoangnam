<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Website VIP</title>
  <style>
    /* 🎥 Video nền toàn màn hình */
    #bg-video {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
    }

    /* 🌟 Nội dung nổi phía trên */
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      font-family: "Segoe UI", sans-serif;
      color: white;
      text-align: center;
      overflow: hidden;
    }

    h1 {
      font-size: 3rem;
      margin-bottom: 40px;
      text-shadow: 0 0 15px #ff00de, 0 0 25px #00c3ff;
      animation: glow 3s ease-in-out infinite alternate;
    }

    @keyframes glow {
      from { text-shadow: 0 0 15px #ff00de, 0 0 25px #00c3ff; }
      to { text-shadow: 0 0 30px #ff00de, 0 0 50px #00c3ff; }
    }

    /* ✨ Nút VIP */
    .btn {
      padding: 15px 40px;
      margin: 10px;
      font-size: 20px;
      font-weight: bold;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      color: #fff;
      background: rgba(0, 0, 0, 0.4);
      backdrop-filter: blur(10px);
      box-shadow: 0 0 15px rgba(255,255,255,0.8);
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .btn:hover {
      transform: scale(1.1);
      box-shadow: 0 0 25px #fff, 0 0 50px #ff00de, 0 0 75px #00c3ff;
    }

    /* 📜 Popup hiển thị code */
    .popup {
      display: none;
      position: fixed;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 80%;
      height: 70%;
      background: rgba(0,0,0,0.95);
      color: #00ffcc;
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 30px rgba(0,0,0,0.8);
      overflow-y: auto;
      z-index: 1000;
      font-family: monospace;
      white-space: pre;
      animation: zoomIn 0.5s ease forwards;
    }

    @keyframes zoomIn {
      from { opacity: 0; transform: translate(-50%, -50%) scale(0.5); }
      to { opacity: 1; transform: translate(-50%, -50%) scale(1); }
    }

    .close-btn {
      position: absolute;
      top: 10px;
      right: 20px;
      font-size: 20px;
      cursor: pointer;
      color: #ff5555;
    }
  </style>
</head>
<body>
  <!-- Video nền -->
  <video autoplay muted loop id="bg-video">
    <source src="snaptik_7539420105990540552_hd.mp4" type="video/mp4">
  </video>

  <!-- Nội dung trên nền -->
  <h1>🚀 Website VIP Cực Ngầu 🚀</h1>

  <button class="btn" id="btn1">Xem code wed</button>
  <button class="btn" id="btn2">Xem code wed</button>

  <!-- Popup hiển thị code -->
  <div class="popup" id="popup">
    <span class="close-btn" id="closeBtn">✖</span>
&lt;!-- Đây là toàn bộ code của web (HTML + CSS + JS) mà bạn đang xem --&gt;
  </div>

  <script>
    const btn2 = document.getElementById("btn2");
    const popup = document.getElementById("popup");
    const closeBtn = document.getElementById("closeBtn");

    btn2.addEventListener("click", () => {
      popup.style.display = "block";
    });

    closeBtn.addEventListener("click", () => {
      popup.style.display = "none";
    });
  </script>
</body>
</html>
