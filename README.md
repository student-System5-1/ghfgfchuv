
<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>หัวใจแห่งความรัก</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      background: linear-gradient(135deg, #180b2e, #421044, #180b2e);
      font-family: Arial, sans-serif;
      overflow: hidden;
    }

    .heart {
      width: 120px;
      height: 120px;
      position: relative;
      background: linear-gradient(135deg, #ff8ac7, #ff176b);
      transform: rotate(-45deg);
      animation: beat 1s infinite;
      box-shadow: 0 0 40px #ff398b;
    }

    .heart::before,
    .heart::after {
      content: "";
      position: absolute;
      width: 120px;
      height: 120px;
      background: inherit;
      border-radius: 50%;
    }

    .heart::before {
      top: -60px;
      left: 0;
    }

    .heart::after {
      top: 0;
      left: 60px;
    }

    @keyframes beat {
      0%, 100% {
        transform: rotate(-45deg) scale(1);
      }
      50% {
        transform: rotate(-45deg) scale(1.2);
      }
    }

    h1 {
      margin-top: 100px;
      color: #ffb5d8;
      font-size: 28px;
      text-shadow: 0 0 15px #ff398b;
    }

    p {
      color: white;
      margin-top: 12px;
      font-size: 16px;
    }

    .sparkle {
      position: absolute;
      color: #ffb5d8;
      animation: float 3s infinite ease-in-out;
    }

    @keyframes float {
      0%, 100% {
        transform: translateY(0);
        opacity: 0.4;
      }
      50% {
        transform: translateY(-25px);
        opacity: 1;
      }
    }
  </style>
</head>

<body>
  <div class="sparkle" style="top:15%;left:20%;font-size:30px;">♥</div>
  <div class="sparkle" style="top:25%;right:20%;font-size:20px;">✦</div>
  <div class="sparkle" style="bottom:20%;left:25%;font-size:24px;">♡</div>
  <div class="sparkle" style="bottom:15%;right:25%;font-size:30px;">✧</div>

  <div class="heart"></div>

  <h1>Made with Love ❤️</h1>
  <p>หัวใจดวงนี้มอบให้เธอ</p>
</body>
</html>
