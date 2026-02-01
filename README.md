<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine?</title>
  <style>
  body {
  background: #f6c1cc;
  font-family: 'Poppins', sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

    .card {
      background: white;
      padding: 40px;
      border-radius: 16px;
      text-align: center;
      width: 400px;
    }

    h2 {
      margin-bottom: 30px;
    }

    button {
      padding: 10px 24px;
      border-radius: 20px;
      border: none;
      cursor: pointer;
      font-size: 16px;
      position: relative;
    }

    #yes {
      background: #ff4d6d;
      color: white;
    }

    #no {
      background: #ddd;
      margin-left: 20px;
      position: absolute;
    }
  </style>
</head>
<body>

  <div class="card">
    <h2>Hey Gyal will you be my valentine?</h2>
    <button id="yes" onclick="alert('Yay ❤️')">Yes</button>
    <button id="no">No</button>
  </div>

  <script>
    const noBtn = document.getElementById("no");

    noBtn.addEventListener("mouseover", () => {
      const x = Math.random() * 300 - 150;
      const y = Math.random() * 200 - 100;

      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    });
  </script>

</body>
</html>
