<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Middle Finger World</title>
  <style>
    body {
      margin: 0;
      background: #111;
      overflow: hidden;
    }

    .main-middle {
      position: absolute;
      top: 50%;
      left: 50%;
      width: 120px;
      transform: translate(-50%, -50%);
      animation: pulse 2s infinite ease-in-out;
      z-index: 10;
      cursor: pointer;
    }

    @keyframes pulse {
      0%, 100% { transform: translate(-50%, -50%) scale(1); }
      50% { transform: translate(-50%, -50%) scale(1.1); }
    }

    .mini-finger {
      position: absolute;
      width: 20px;
      opacity: 0.4;
      animation: floatUp linear infinite;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(100vh) scale(1) rotate(0deg);
        opacity: 0;
      }
      10% { opacity: 0.5; }
      100% {
        transform: translateY(-10vh) scale(1.2) rotate(360deg);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <!-- Main Middle Finger SVG (center) -->
  <svg class="main-middle" viewBox="0 0 512 512" fill="white" xmlns="http://www.w3.org/2000/svg">
    <path d="M256 0c17.7 0 32 14.3 32 32v208h16c17.7 0 32 14.3 32 32v80h16c17.7 0 32 14.3 32 32v48h16c17.7 0 32 14.3 32 32v16c0 17.7-14.3 32-32 32H112c-17.7 0-32-14.3-32-32v-16c0-17.7 14.3-32 32-32h16v-96c0-17.7 14.3-32 32-32h16V208c0-17.7 14.3-32 32-32h16V32c0-17.7 14.3-32 32-32z"/>
  </svg>

  <!-- Floating Background Middle Fingers -->
  <script>
    const COUNT = 50;

    for (let i = 0; i < COUNT; i++) {
      const svg = document.createElementNS("http://www.w3.org/2000/svg", "svg");
      svg.setAttribute("viewBox", "0 0 512 512");
      svg.setAttribute("fill", "white");
      svg.setAttribute("class", "mini-finger");

      svg.style.left = Math.random() * 100 + 'vw';
      svg.style.top = Math.random() * 100 + 'vh';
      svg.style.width = (Math.random() * 20 + 10) + "px";
      svg.style.animationDuration = (Math.random() * 10 + 5) + "s";
      svg.style.animationDelay = Math.random() * 5 + "s";

      const path = document.createElementNS("http://www.w3.org/2000/svg", "path");
      path.setAttribute("d", "M256 0c17.7 0 32 14.3 32 32v208h16c17.7 0 32 14.3 32 32v80h16c17.7 0 32 14.3 32 32v48h16c17.7 0 32 14.3 32 32v16c0 17.7-14.3 32-32 32H112c-17.7 0-32-14.3-32-32v-16c0-17.7 14.3-32 32-32h16v-96c0-17.7 14.3-32 32-32h16V208c0-17.7 14.3-32 32-32h16V32c0-17.7 14.3-32 32-32z");

      svg.appendChild(path);
      document.body.appendChild(svg);
    }
  </script>

</body>
</html>
