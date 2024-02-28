<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Snake Animation</title>
  <style>
    /* Style for the snake */
    #snake {
      width: 50px;
      height: 50px;
      fill: red;
      animation: snakeMove 5s linear infinite;
    }

    /* Keyframe animation for the snake */
    @keyframes snakeMove {
      0% {
        transform: translateX(0);
      }
      50% {
        transform: translateX(200px);
      }
      100% {
        transform: translateX(0);
      }
    }
  </style>
</head>
<body>
  <!-- SVG container for the snake -->
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100">
    <path id="snake" d="M10,50 Q30,25 50,50 Q70,75 90,50" />
  </svg>
</body>
</html>

