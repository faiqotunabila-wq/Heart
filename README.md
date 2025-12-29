<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Keep Our Streak</title>

  <style>
    body{
      background: #0d0d0d;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: Arial, Helvetica, sans-serif;
    }

    .box{
      text-align: center;
      padding: 30px 40px;
      border-radius: 20px;
      background: linear-gradient(45deg, #ff4d79, #ff2a95);
      box-shadow: 0 0 25px rgba(255,0,102,0.6);
    }

    h1{
      margin-bottom: 10px;
    }

    .streak{
      font-size: 45px;
      font-weight: bold;
    }

    button{
      margin-top: 20px;
      padding: 10px 20px;
      border-radius: 10px;
      border:none;
      font-size: 16px;
      background:#fff;
    }
  </style>

</head>

<body>

  <div class="box">
    <h1>Keep Our Streak ❤️</h1>
    <div class="streak">
      🔥 <span id="count">1</span> Days
    </div>

    <button onclick="addStreak()">Tambah Streak</button>
  </div>


  <script>
    let streak = 1;

    function addStreak(){
      streak++;
      document.getElementById("count").innerText = streak;
    }
  </script>

</body>
</html>