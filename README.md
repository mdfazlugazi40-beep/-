
<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport"
        content="width=device-width, initial-scale=1">
  <title>PRIME MINI APP</title>
  <script src="https://telegram.org/js/telegram-web-app.js"></script>
  <style>
    body {
      margin: 0;
      padding: 20px;
      background: #101827;
      color: white;
      font-family: Arial, sans-serif;
    }
    .card {
      background: #1e293b;
      padding: 22px;
      border-radius: 16px;
      text-align: center;
    }
    h2 { color: #45e0a8; }
    button {
      width: 100%;
      padding: 14px;
      margin-top: 12px;
      border: 0;
      border-radius: 10px;
      background: #16a879;
      color: white;
      font-size: 16px;
    }
  </style>
</head>
<body>
  <div class="card">
    <h2>PRIME MINI APP</h2>
    <p>Welcome to our Mini App!</p>
    <button onclick="showMessage('Account')">
      👤 Account
    </button>
    <button onclick="showMessage('Referral')">
      ⚡ Referral
    </button>
    <button onclick="showMessage('Wallet')">
      💳 Wallet
    </button>
    <button onclick="showMessage('Support')">
      📞 Support
    </button>
  </div>

  <script>
    const tg = window.Telegram.WebApp;
    tg.ready();
    tg.expand();

    function showMessage(name) {
      tg.showAlert(name + ' পেজ পরে যুক্ত করা হবে।');
    }
  </script>
</body>
</html>
