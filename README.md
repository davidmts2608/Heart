# Heart

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>For You ❤️</title>

    <style>
      body {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background: #f2f2f2;
        font-family: Arial, sans-serif;
      }

      .heart {
        position: relative;
        width: 220px;
        height: 200px;
        transform: rotate(-45deg);
      }

      .heart-shape {
        position: absolute;
        width: 220px;
        height: 200px;
        background: #e63946;
        top: 0;
        left: 0;
      }

      .heart-shape::before,
      .heart-shape::after {
        content: "";
        position: absolute;
        width: 220px;
        height: 200px;
        background: #e63946;
        border-radius: 50%;
      }

      .heart-shape::before {
        top: -110px;
        left: 0;
      }

      .heart-shape::after {
        left: 110px;
        top: 0;
      }

      .text {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%) rotate(45deg);
        color: white;
        text-align: center;
        width: 150px;
        font-size: 18px;
        font-weight: bold;
        line-height: 1.4;
        z-index: 10; /* brings text to front */
        pointer-events: none;
      }
    </style>
  </head>
  <body>
    <div class="heart">
      <div class="heart-shape"></div>

      <div class="text">bruh<br /></div>
    </div>
  </body>
</html>
