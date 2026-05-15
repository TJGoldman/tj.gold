<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>tj.gold</title>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      background: #0e0e0e;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
    }

    .mark {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .ring {
      position: absolute;
      border-radius: 50%;
      border: 1px solid rgba(184, 134, 11, 0.15);
      animation: pulse 4s ease-in-out infinite;
    }

    .ring:nth-child(1) { width: 160px; height: 160px; animation-delay: 0s; }
    .ring:nth-child(2) { width: 260px; height: 260px; animation-delay: 0.6s; }
    .ring:nth-child(3) { width: 360px; height: 360px; animation-delay: 1.2s; }

    @keyframes pulse {
      0%, 100% { opacity: 0.2; transform: scale(1); }
      50%       { opacity: 0.6; transform: scale(1.03); }
    }

    .wordmark {
      position: relative;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      font-size: 1.1rem;
      font-weight: 600;
      letter-spacing: 0.18em;
      text-transform: lowercase;
      color: #b8860b;
      opacity: 0;
      animation: fadein 1.8s ease forwards 0.4s;
    }

    @keyframes fadein {
      to { opacity: 1; }
    }
  </style>
</head>
<body>

  <div class="mark">
    <div class="ring"></div>
    <div class="ring"></div>
    <div class="ring"></div>
    <span class="wordmark">tj.gold</span>
  </div>

</body>
</html>
