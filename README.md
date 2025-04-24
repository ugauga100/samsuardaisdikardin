# samsuardaisdikardin
prabowo bodoh
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Slide Fadhlurrrah Man</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: black;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
    }

    .slide {
      display: none;
      font-size: 5em;
      text-align: center;
    }

    .active {
      display: block;
    }

    button {
      position: absolute;
      bottom: 40px;
      padding: 15px 30px;
      font-size: 1em;
      background: white;
      color: black;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <div id="slide1" class="slide active">OI</div>
  <div id="slide2" class="slide">LOL</div>
  <div id="slide3" class="slide">LEMPAR NMAX MAU</div>

  <button onclick="nextSlide()">Lanjut</button>

  <script>
    let current = 1;

    function nextSlide() {
      document.getElementById('slide' + current).classList.remove('active');
      current++;
      if (current > 3) current = 1;
      document.getElementById('slide' + current).classList.add('active');
    }
  </script>
</body>
</html>
