<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Loading...</title>
  <style>
    body {
      background: #0d1117;
      color: #fff;
      font-family: Arial, sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      flex-direction: column;
      text-align: center;
    }
    .spinner {
      border: 6px solid #2c2f33;
      border-top: 6px solid #00ffcc;
      border-radius: 50%;
      width: 60px;
      height: 60px;
      animation: spin 1s linear infinite;
      margin-bottom: 20px;
    }
    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    .text {
      font-size: 18px;
    }
  </style>
</head>
<body>
  <div class="spinner"></div>
  <div class="text">Loading… please wait</div>

  <script>
    // Set the target date & time (year, month-1, day, hour, minute)
    const launchTime = new Date("2025-08-29T00:00:00").getTime(); 

    const checkTime = setInterval(() => {
      const now = new Date().getTime();

      if (now >= launchTime) {
        clearInterval(checkTime);
        // 🔗 Replace the link below with the PUBLIC URL of your PDF
        window.location.href = "https://www.canva.com/design/DAGw__IF8CU/FbCjPmSZzfGZFd5K0b6wQQ/edit?utm_content=DAGw__IF8CU&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton";
      }
    }, 1000);
  </script>
</body>
</html>
