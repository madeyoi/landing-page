
<html lang="ar">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AI Merchant</title>
<style>
/* === Reset === */
* { box-sizing: border-box; margin: 0; padding: 0; font-family: Arial, sans-serif; }
body { direction: rtl; background-color: #f4f4f4; }

/* === Header === */
.header { display: flex; justify-content: space-between; align-items: center; background-color: #1e90ff; color: white; padding: 15px 30px; }
.header .logo { font-size: 24px; font-weight: bold; }
.header nav a { color: white; margin-left: 20px; text-decoration: none; cursor: pointer; }
.header nav a:hover { text-decoration: underline; }

/* === Hero / Landing === */
.hero { text-align: center; padding: 60px 20px; background-color: #e6f2ff; }
.hero h1 { font-size: 36px; margin-bottom: 20px; }
.hero p { font-size: 18px; margin-bottom: 30px; }
.btn { background-color: #1e90ff; color: white; padding: 12px 25px; border: none; border-radius: 6px; cursor: pointer; text-decoration: none; }
.btn:hover { background-color: #0f78d4; }

/* === Features === */
.features { padding: 40px 20px; text-align: center; }
.feature-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); gap: 20px; margin-top: 30px; }
.feature { background-color: white; padding: 25px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); font-size: 18px; }

/* === Signup/Login === */
.signup { background-color: #fff; max-width: 400px; margin: 30px auto; padding: 30px; border-radius: 10px; box-shadow: 0 0 15px rgba(0,0,0,0.1); text-align: center; }
.signup input { width: 90%; padding: 10px; margin: 10px 0; border-radius: 6px; border: 1px solid #ccc; }
.signup button { width: 95%; padding: 12px; margin-top: 10px; }

/* === Dashboard Layout === */
.dashboard-container { display: flex; min-height: 80vh; margin-top: 20px; }
.sidebar { width: 220px; background-color: #1e90ff; color: white; padding: 20px; }
.sidebar h2 { margin-bottom: 30px; }
.sidebar nav a { display: block; color: white; text-decoration: none; padding: 10px 0; margin-bottom: 10px; border-radius: 5px; cursor: pointer; }
.sidebar nav a:hover { background-color: #0f78d4; }

/* === Main Panel === */
.main-panel { flex: 1; padding: 30px; background-color: #f4f4f4; display: none; }
.main-panel.active { display: block; }
.stats-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin-bottom: 20px; }
.stat-card { background-color: white; padding: 25px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); font-size: 18px; text-align: center; }

/* === Product Scout === */
.product-card { background-color: white; padding: 15px; border-radius: 10px; box-shadow: 0 0 5px rgba(0,0,0,0.1); margin-bottom: 15px; }
.product-card button { margin-top: 10px; padding: 8px 15px; border: none; border-radius: 5px; background-color: #1e90ff; color: white; cursor: pointer; }
.product-card button:hover { background-color: #0f78d4; }

/* === Inventory Table === */
table { width: 100%; border-collapse: collapse; margin-top: 20px; }
table th, table td { padding: 12px; border: 1px solid #ccc; text-align: center; }
table th { background-color: #1e90ff; color: white; }
</style>
</head>
<body>

<!-- Header -->
<header class="header">
  <div class="logo">AI Merchant</div>
  <nav>
    <a onclick="showPanel('landing')">Landing</a>
    <a onclick="showPanel('dashboard')">Dashboard</a>
  </nav>
</header>

<!-- Landing Page -->
<div id="landing" class="main-panel active">
  <section class="hero">
    <h1>تاجر إلكتروني ذكي يعتمد على الذكاء الاصطناعي</h1>
    <p>اختر المنتجات المربحة، أدِر المخزون، وابدأ التسويق الذكي بكل سهولة</p>
    <a class="btn" onclick="showPanel('dashboard')">ابدأ الآن</a>
  </section>

  <section class="features">
    <h2>مزايا المنصة</h2>
    <div class="feature-grid">
      <div class="feature">🔍 اختيار المنتجات</div>
      <div class="feature">📦 إدارة المخزون</div>
      <div class="feature">💲 التسعير الديناميكي</div>
      <div class="feature">📢 التسويق الذكي</div>
    </div>
  </section>

  <section class="signup">
    <h2>إنشاء حساب جديد</h2>
    <input type="email" placeholder="البريد الإلكتروني">
    <input type="password" placeholder="كلمة المرور">
    <input type="password" placeholder="تأكيد كلمة المرور">
    <button>إنشاء حساب</button>
  </section>
</div>

<!-- Dashboard -->
<div id="dashboard" class="main-panel">
  <div class="dashboard-container">
    <aside class="sidebar">
      <h2>AI Merchant</h2>
      <nav>
        <a onclick="switchTab('dashboardMain')">Dashboard</a>
        <a onclick="switchTab('productScout')">Product Scout</a>
        <a onclick="switchTab('inventory')">Inventory</a>
        <a onclick="switchTab('marketing')">Marketing AI</a>
        <a onclick="switchTab('chatbot')">Chatbot</a>
        <a onclick="switchTab('analytics')">Analytics</a>
      </nav>
    </aside>

    <div class="main-content">
      <!-- Dashboard Main -->
      <div id="dashboardMain" class="tab-content active">
        <h1>لوحة التحكم</h1>
        <div class="stats-grid">
          <div class="stat-card">المبيعات اليوم: 150$</div>
          <div class="stat-card">المنتجات الأكثر ربحًا: 5</div>
          <div class="stat-card">الطلبات الجديدة: 12</div>
        </div>
      </div>

      <!-- Product Scout -->
      <div id="productScout" class="tab-content">
        <h2>Product Scout</h2>
        <button class="btn" onclick="suggestProduct()">اقتراح منتج</button>
        <div id="productList"></div>
      </div>

      <!-- Inventory -->
      <div id="inventory" class="tab-content">
        <h2>Inventory</h2>
        <table>
          <thead>
            <tr><th>اسم المنتج</th><th>الفئة</th><th>السعر</th><th>الكمية</th></tr>
          </thead>
          <tbody id="inventoryTable">
            <tr><td>هاتف ذكي</td><td>الكترونيات</td><td>299.99</td><td>10</td></tr>
            <tr><td>ساعة ذكية</td><td>الكترونيات</td><td>199.99</td><td>5</td></tr>
          </tbody>
        </table>
      </div>

      <!-- Marketing AI -->
      <div id="marketing" class="tab-content">
        <h2>Marketing AI</h2>
        <p>إحصائيات الحملات وإدارة الإعلانات الذكية.</p>
      </div>

      <!-- Chatbot -->
      <div id="chatbot" class="tab-content">
        <h2>Chatbot</h2>
        <p>نافذة المحادثة مع العملاء.</p>
      </div>

      <!-- Analytics -->
      <div id="analytics" class="tab-content">
        <h2>Analytics</h2>
        <p>تحليل المبيعات والأداء.</p>
      </div>
    </div>
  </div>
</div>

<script>
// Switch between Landing and Dashboard
function showPanel(panelId) {
  document.querySelectorAll('.main-panel').forEach(p => p.classList.remove('active'));
  document.getElementById(panelId).classList.add('active');
}

// Switch Dashboard Tabs
function switchTab(tabId) {
  document.querySelectorAll('.tab-content').forEach(t => t.classList.remove('active'));
  document.getElementById(tabId).classList.add('active');
}

// Mock Product Suggestion
function suggestProduct() {
  const products = [
    {name:"هاتف ذكي",price:299.99,category:"الكترونيات"},
    {name:"ساعة ذكية",price:199.99,category:"الكترونيات"},
    {name:"حقيبة ظهر",price:49.99,category:"أزياء"},
    {name:"سماعات لاسلكية",price:89.99,category:"الكترونيات"}
  ];
  const prod = products[Math.floor(Math.random()*products.length)];
  const div = document.createElement('div');
  div.className = 'product-card';
  div.innerHTML = `<h3>${prod.name}</h3><p>السعر: $${prod.price}</p><p>الفئة: ${prod.category}</p><button>إضافة للمتجر</button>`;
  document.getElementById('productList').prepend(div);
}
</script>
</body>
</html>
