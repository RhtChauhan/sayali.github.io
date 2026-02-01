# sayali.github.io

<!DOCTYPE html>
<html lang="en">
<head>s
  <meta charset="UTF-8">
  <title>Valentine Proposal 💖</title>
  <style>
    body {
      height: 100vh;
      margin: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff758c, #ff7eb3);
      font-family: 'Poppins', sans-serif;
      overflow: hidden;
    }

    .card {
      background: white;
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 20px 40px rgba(0,0,0,0.2);
      width: 320px;
      position: relative;
    }

    h1 {
      color: #ff4d6d;
      margin-bottom: 10px;
    }

    p {
      font-size: 18px;
      margin-bottom: 30px;
    }

    button {
      padding: 12px 24px;
      font-size: 16px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: 0.3s;
      position: relative;
    }

    #yesBtn {
      background-color: #ff4d6d;
      color: white;
      margin-right: 10px;
    }

    #yesBtn:hover {
      transform: scale(1.1);
    }

    #noBtn {
      background-color: #ccc;
      color: #333;
      position: absolute;
    }

    #gif {
      display: none;
      margin-top: 20px;
      width: 100%;
      border-radius: 15px;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>Sayali 💕</h1>
    <p>Will you be my Valentine?</p>

    <button id="yesBtn" onclick="yesClicked()">Yes 💖</button>
    <button id="noBtn" onmouseover="moveNo()">No 🙃</button>

    <img id="gif" src="https://media.giphy.com/media/l0MYt5jPR6QX5pnqM/giphy.gif" alt="Love Gif">
  </div>

  <script>
    const noBtn = document.getElementById("noBtn");

    function moveNo() {
      const x = Math.random() * 200 - 100;
      const y = Math.random() * 200 - 100;
      noBtn.style.transform = `translate(${x}px, ${y}px)`;
    }

    function yesClicked() {
      document.querySelector("p").innerText = "Yayyy!!! 💘 I knew it 😍";
      document.getElementById("gif").style.display = "block";
      noBtn.style.display = "none";
    }
  </script>

</body>
</html>
