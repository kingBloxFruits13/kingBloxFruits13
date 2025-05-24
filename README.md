<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>BloxFruitStore 🍍💰</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
      color: #fff;
      text-align: center;
      padding: 60px 20px;
    }

    .container {
      background: rgba(0, 0, 0, 0.6);
      padding: 40px;
      border-radius: 16px;
      box-shadow: 0 0 20px rgba(0, 255, 170, 0.2);
      max-width: 500px;
      margin: auto;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.2em;
      margin: 20px 0;
      white-space: pre-line;
    }

    button {
      padding: 12px 24px;
      background-color: #00cc88;
      border: none;
      border-radius: 10px;
      color: white;
      font-size: 18px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #00b377;
    }

    .whatsapp-btn {
      display: inline-block;
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #25D366;
      color: white;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s;
    }

    .whatsapp-btn:hover {
      background-color: #1ebe5d;
    }

    .support {
      position: fixed;
      top: 15px;
      right: 15px;
      background-color: #ffc107;
      color: #000;
      padding: 10px 15px;
      border-radius: 8px;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>BloxFruitStore 🍍💰</h1>
    <p id="output">اضغط الزر للحصول على حساب وفاكهة 🎲</p>
    <button onclick="generate()">🎁 احصل على حساب</button>
    <a id="whatsappLink" href="#" target="_blank" class="whatsapp-btn" style="display:none;">📱 اطلب عبر واتساب</a>
  </div>

  <div class="support">
    💰 للمساعدة المالية
  </div>

  <script>
    const fruits = [
      { name: "Gravity 🍇", price: 30 },
      { name: "Control ⚡", price: 15 },
      { name: "Rumble ⚡", price: 15 }
    ];

    const accounts = [
      "fruitboss99:pass123",
      "legendx:control007",
      "rumblegod:powerup",
      "pineapple_kid:fruity!",
      "shadowfruit:rumblex"
    ];

    function generate() {
      const fruit = fruits[Math.floor(Math.random() * fruits.length)];
      const account = accounts[Math.floor(Math.random() * accounts.length)];
      const msg = `👤 حساب Blox Fruits:\n${account}\n🍍 الفاكهة: ${fruit.name}\n💵 السعر: ${fruit.price} درهم`;

      document.getElementById("output").innerText = msg;

      // رقم واتساب - بدله برقمك الفعلي مع رمز الدولة
      const phone = "971500000000"; // مثال رقم إماراتي
      const whatsappURL = `https://wa.me/${phone}?text=${encodeURIComponent(msg)}`;

      const link = document.getElementById("whatsappLink");
      link.href = whatsappURL;
      link.style.display = "inline-block";
    }
  </script>

</body>
</html>

kingBloxFruits13/kingBloxFruits13 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
