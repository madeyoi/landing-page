
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>AI Merchant | التاجر الإلكتروني الذكي</title>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;800&display=swap" rel="stylesheet">
<meta name="description" content="AI Merchant منصة تاجر إلكتروني ذكي تعتمد على الذكاء الاصطناعي لأتمتة التجارة الإلكترونية بالكامل.">
<style>
/* ================= Base ================= */
*{box-sizing:border-box;}
:root{--bg:#0b1020;--bg-alt:#101733;--card:#121a3d;--text:#e8ecff;--muted:#a9b1d6;--primary:#6c9cff;--primary-ink:#0a0f24;--ring:rgba(108,156,255,0.35);--success:#22c55e;}
html,body{margin:0;padding:0;background:linear-gradient(180deg,var(--bg) 0%,#0c1124 100%);color:var(--text);font-family:"Cairo",system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;line-height:1.7;}
img{max-width:100%;display:block;}
a{color:var(--text);text-decoration:none;}
.container{width:min(1100px,92%);margin:0 auto;}
/* ================= Navbar ================= */
.navbar{position:sticky;top:0;z-index:50;background:rgba(10,15,36,0.6);backdrop-filter:blur(10px);border-bottom:1px solid rgba(255,255,255,0.06);}
.nav-wrap{display:flex;align-items:center;justify-content:space-between;padding:12px 0;}
.brand{display:inline-flex;gap:8px;align-items:center;font-weight:800;letter-spacing:.2px;}
.brand .logo{font-size:20px;}
.nav-links{display:flex;gap:16px;align-items:center;}
.nav-links a{opacity:.9;}
.burger{display:none;flex-direction:column;gap:4px;background:none;border:0;cursor:pointer;}
.burger span{width:22px;height:2px;background:var(--text);display:block;}
/* ================= Buttons, Badges ================= */
.btn{display:inline-block;padding:10px 16px;border-radius:14px;border:1px solid transparent;font-weight:700;transition:transform .08s ease,box-shadow .2s ease,background .2s ease;box-shadow:0 8px 24px rgba(108,156,255,0.2);}
.btn:hover{transform:translateY(-1px);}
.btn:active{transform:translateY(0);}
.btn--primary{background:var(--primary);color:var(--primary-ink);}
.btn--ghost{background:transparent;border-color:rgba(255,255,255,0.12);}
.badge{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(108,156,255,0.16);color:var(--text);font-weight:700;font-size:12px;border:1px solid rgba(108,156,255,0.25);}
/* ================= Hero ================= */
.hero{padding:64px 0 32px;}
.hero-grid{display:grid;grid-template-columns:1.2fr .8fr;align-items:center;gap:28px;}
.hero-text h1{font-size:38px;line-height:1.2;margin:0 0 10px;}
.muted{color:var(--muted);}
.hero-cta{display:flex;gap:12px;margin-top:16px;}
.badges{display:flex;gap:8px;margin-top:14px;flex-wrap:wrap;}
.card{background:linear-gradient(180deg,var(--card),#0f1840);border:1px solid rgba(255,255,255,0.06);border-radius:18px;padding:18px;box-shadow:inset 0 1px 0 rgba(255,255,255,0.06),0 20px 40px rgba(0,0,0,0.25);}
.hero-card .card h3{margin-top:0;}
.checklist{padding:0;margin:10px 0 0;list-style:none;}
.checklist li{padding:8px 0;border-bottom:1px dashed rgba(255,255,255,0.08);}
.checklist li:last-child{border-bottom:none;}
/* ================= Sections ================= */
.section{padding:64px 0;}
.section.alt{background:linear-gradient(180deg,var(--bg-alt),rgba(16,23,51,0.7));}
.section-title{font-size:28px;margin:0 0 24px;}
.grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;}
.feature{padding:16px;border:1px solid rgba(255,255,255,0.06);border-radius:16px;background:rgba(18,26,61,0.6);}
.feature-icon{font-size:22px;margin-bottom:8px;}
.steps{counter-reset:step;padding:0;margin:0;list-style:none;display:grid;gap:10px;}
.steps li{display:flex;gap:10px;align-items:center;background:rgba(18,26,61,0.6);border:1px solid rgba(255,255,255,0.06);border-radius:14px;padding:12px 14px;}
.steps li span{width:30px;height:30px;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;background:var(--primary);color:var(--primary-ink);font-weight:800;}
.price-card{position:relative;}
.price-card--featured{outline:2px solid var(--primary);}
.ribbon{position:absolute;top:-10px;left:12px;background:var(--primary);color:var(--primary-ink);font-weight:800;padding:4px 10px;border-radius:999px;font-size:12px;}
.price{font-size:36px;font-weight:800;margin:8px 0 12px;}
.price small{font-size:12px;color:var(--muted);}
.list{list-style:none;padding:0;margin:0 0 12px;}
.list li{padding:6px 0;border-bottom:1px dashed rgba(255,255,255,0.08);}
.list li:last-child{border-bottom:0;}
.toggle{position:relative;display:inline-flex;align-items:center;cursor:pointer;user-select:none;}
.toggle input{display:none;}
.toggle-track{position:relative;width:120px;height:36px;border-radius:999px;border:1px solid rgba(255,255,255,0.12);display:inline-flex;align-items:center;justify-content:space-between;padding:0 12px;font-weight:700;}
.toggle-track::before{content:attr(data-monthly);position:absolute;right:14px;opacity:.9;}
.toggle-track::after{content:"";position:absolute;top:4px;left:4px;width:28px;height:28px;border-radius:50%;background:var(--primary);transition:transform .25s ease;}
.toggle input:checked + .toggle-track::before{content:attr(data-yearly);right:auto;left:14px;}
.toggle input:checked + .toggle-track::after{transform:translateX(84px);}
.accordion{display:grid;gap:10px;}
.accordion-item{border:1px solid rgba(255,255,255,0.08);border-radius:14px;overflow:hidden;background:rgba(18,26,61,0.6);}
.accordion-header{width:100%;text-align:start;background:transparent;color:var(--text);font-weight:700;border:0;padding:14px;cursor:pointer;}
.accordion-body{padding:0 14px 14px;display:none;color:var(--muted);}
.accordion-item.open .accordion-body{display:block;}
.cta{padding-top:20px;}
.cta-card{text-align:center;}
.signup-form{margin-top:12px;display:flex;gap:8px;align-items:center;justify-content:center;flex-wrap:wrap;}
.signup-form input{padding:10px 12px;border-radius:12px;border:1px solid rgba(255,255,255,0.12);background:rgba(255,255,255,0.02);color:var(--text);min-width:260px;}
.form-msg{display:block;margin-top:6px;min-height:20px;}
.sr-only{position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0);white-space:nowrap;}
.footer{padding:24px 0 56px;border-top:1px solid rgba(255,255,255,0.06);}
.footer-grid{display:flex;align-items:center;justify-content:space-between;}
.socials a{opacity:.8;margin-inline-start:10px;}
@media(max-width:940px){.hero-grid{grid-template-columns:1fr;}}
@media(max-width:720px){.grid-3{grid-template-columns:1fr 1fr;}}
@media(max-width:520px){.nav-links{display:none;position:absolute;inset-inline:0;top:56px;background:rgba(12,17,36,0.98);padding:12px 16px;flex-direction:column;gap:10px;}.nav-links.open{display:flex;}.burger{display:inline-flex;}.grid-3{grid-template-columns:1fr;}.hero-text h1{font-size:30px;}}
</style>
</head>
<body>
<!-- Navbar -->
<header class="navbar">
<div class="container nav-wrap">
<a class="brand" href="#"><span class="logo">🤖</span><span>AI Merchant</span></a>
<nav class="nav-links" id="navLinks">
<a href="#features">المزايا</a>
<a href="#how">كيف يعمل</a>
<a href="#pricing">الأسعار</a>
<a href="#faq">الأسئلة الشائعة</a>
<a href="#cta" class="btn btn--ghost">جرّبه الآن</a>
</nav>
<button class="burger" id="burger" aria-label="قائمة"><span></span><span></span><span></span></button>
</div>
</header>
<!-- Hero -->
<section class="hero">
<div class="container hero-grid">
<div class="hero-text">
<h1>التاجر الإلكتروني الذكي المدعوم بالذكاء الاصطناعي</h1>
<p class="muted">أتمتة كاملة لدورة التجارة الإلكترونية: اختيار المنتجات، إدارة المخزون، التسعير الديناميكي، التسويق، خدمة العملاء، والشحن — كل ذلك في منصة واحدة.</p>
<div class="hero-cta"><a href="#cta" class="btn btn--primary">ابدأ النسخة التجريبية</a><a href="#features" class="btn btn--ghost">اكتشف المزايا</a></div>
<div class="badges"><span class="badge">اشتراك شهري (SaaS)</span><span class="badge">عمولة على المبيعات</span><span class="badge">خدمات إضافية مدفوعة</span></div>
</div>
<div class="hero-card"><div class="card">
<h3>لوحة تاجر ذكية</h3>
<ul class="checklist">
<li>🔍 اختيار المنتجات المربحة تلقائيًا</li>
<li>📦 مزامنة المخزون مع الموردين</li>
<li>💲 تسعير ديناميكي حسب السوق</li>
<li>📢 حملات تسويق مُدارة بالذكاء الاصطناعي</li>
<li>🤖 شات بوت لخدمة العملاء 24/7</li>
<li>🚚 تكامل شركات الشحن</li>
</ul></div></div>
</div>
</section>
<!-- Features -->
<section id="features" class="section">
<div class="container"><h2 class="section-title">المزايا الأساسية</h2>
<div class="grid-3">
<div class="feature"><div class="feature-icon">🔎</div><h3>اختيار المنتجات</h3><p>تحليل السوق والاتجاهات لاكتشاف فرص منتجات مربحة بأقل منافسة.</p></div>
<div class="feature"><div class="feature-icon">📦</div><h3>إدارة المخزون</h3><p>تحديثات تلقائية ومزامنة مع الموردين لتجنّب نفاد المخزون.</p></div>
<div class="feature"><div class="feature-icon">💲</div><h3>تسعير ذكي</h3><p>تعديل الأسعار تلقائيًا بناءً على الطلب والمنافسة والهوامش.</p></div>
<div class="feature"><div class="feature-icon">📢</div><h3>تسويق آلي</h3><p>إعلانات مستهدفة وإدارة القنوات من مكان واحد مع تقارير واضحة.</p></div>
<div class="feature"><div class="feature-icon">🤖</div><h3>خدمة عملاء</h3><p>شات بوت متعدد اللغات يجيب 24/7 ويحوّل الحالات المعقدة للبشر.</p></div>
<div class="feature"><div class="feature-icon">🚚</div><h3>لوجستيات سلسة</h3><p>تنسيق الشحن والتوصيل مع شركاء موثوقين وتتبع الطلبات.</p></div>
</div>
</div>
</section>
<!-- How it works -->
<section id="how" class="section alt">
<div class="container"><h2 class="section-title">كيف يعمل</h2>
<ol class="steps">
<li><span>1</span> أنشئ حسابك وحدّد السوق الذي تستهدفه.</li>
<li><span>2</span> دع الذكاء الاصطناعي يقترح منتجات مربحة.</li>
<li><span>3</span> أطلق متجرك تلقائيًا خلال دقائق.</li>
<li><span>4</span> فعّل التسويق وخدمة العملاء والشحن بنقرة واحدة.</li>
</ol>
</div>
</section>
<!-- Pricing -->
<section id="pricing" class="section">
<div class="container">
<div class="pricing-head">
<h2 class="section-title">الأسعار</h2>
<label class="toggle"><input type="checkbox" id="priceToggle" aria-label="تبديل سنوي / شهري"><span class="toggle-track" data-monthly="شهري" data-yearly="سنوي"></span></label>
</div>
<div class="grid-3">
<div class="card price-card">
<h3>Starter</h3>
<div class="price"><span id="p1">99</span><small>$/<span id="term1">شهر</span></small></div>
<ul class="list"><li>MVP: اختيار المنتجات + إطلاق متجر</li><li>مكوّنات أساسية</li><li>دعم عبر البريد</li></ul>
<a href="#cta" class="btn btn--primary">ابدأ الآن</a>
</div>
<div class="card price-card price-card--featured"><div class="ribbon">الأكثر شيوعًا</div>
<h3>Growth</h3>
<div class="price"><span id="p2">199</span><small>$/<span id="term2">شهر</span></small></div>
<ul class="list"><li>كل ما في Starter</li><li>تسويق آلي وتقارير</li><li>شات بوت 24/7</li></ul>
<a href="#cta" class="btn btn--primary">جرّبه مجانًا</a>
</div>
<div class="card price-card">
<h3>Scale</h3>
<div class="price"><span id="p3">499</span><small>$/<span id="term3">شهر</span></small></div>
<ul class="list"><li>كل ما في Growth</li><li>تكاملات لوجستية متقدمة</li><li>مدير نجاح مخصص</li></ul>
<a href="#cta" class="btn btn--ghost">تحدث مع المبيعات</a>
</div>
</div>
</div>
</section>
<!-- FAQ -->
<section id="faq" class="section alt">
<div class="container">
<h2 class="section-title">الأسئلة الشائعة</h2>
<div class="accordion" id="faqList">
<div class="accordion-item">
<button class="accordion-header">ما الذي يميز AI Merchant؟</button>
<div class="accordion-body">يقلل الأخطاء ويختصر الوقت عبر أتمتة دورة التجارة بالكامل ويتيح دخولًا سريعًا للسوق.</div>
</div>
<div class="accordion-item">
<button class="accordion-header">هل أحتاج خبرة مسبقة؟</button>
<div class="accordion-body">لا، المنصة ترشدك خطوة بخطوة وتبدأ بـ MVP جاهز.</div>
</div>
<div class="accordion-item">
<button class="accordion-header">هل يمكن ربط المنصة مع متجري الحالي؟</button>
<div class="accordion-body">نعم، نوفر تكاملات شائعة عبر واجهات برمجة التطبيقات (API) والإضافات.</div>
</div>
</div>
</div>
</section>
<!-- CTA / Signup -->
<section id="cta" class="section cta">
<div class="container">
<div class="card cta-card">
<h2>ابدأ نسختك التجريبية الآن</h2>
<p class="muted">سجّل بريدك الإلكتروني لنبلغك عند الإطلاق الأولي.</p>
<form id="signupForm" class="signup-form" novalidate>
<label class="sr-only" for="email">البريد الإلكتروني</label>
<input type="email" id="email" placeholder="you@example.com" required>
<button type="submit" class="btn btn--primary">تسجيل</button>
<small id="formMsg" class="form-msg" role="status" aria-live="polite"></small>
</form>
</div>
</div>
</section>
<footer class="footer">
<div class="container footer-grid">
<p>© <span id="year"></span> AI Merchant. جميع الحقوق محفوظة.</p>
<div class="socials">
<a href="#" aria-label="X">X</a>
<a href="#" aria-label="LinkedIn">LinkedIn</a>
<a href="#" aria-label="YouTube">YouTube</a>
</div>
</div>
</footer>
<script>
// Burger menu toggle
const burger=document.getElementById("burger"),navLinks=document.getElementById("navLinks");
burger.addEventListener("click",()=>{navLinks.classList.toggle("open");});
// Pricing toggle
const priceToggle=document.getElementById("priceToggle"),prices=[{monthly:99,yearly:990},{monthly:199,yearly:1990},{monthly:499,yearly:4990}],p1=document.getElementById("p1"),p2=document.getElementById("p2"),p3=document.getElementById("p3"),term1=document.getElementById("term1"),term2=document.getElementById("term2"),term3=document.getElementById("term3");
priceToggle.addEventListener("change",()=>{if(priceToggle.checked){p1.textContent=prices[0].yearly;p2.textContent=prices[1].yearly;p3.textContent=prices[2].yearly;term1.textContent="سنة";term2.textContent="سنة";term3.textContent="سنة";}else{p1.textContent=prices[0].monthly;p2.textContent=prices[1].monthly;p3.textContent=prices[2].monthly;term1.textContent="شهر";term2.textContent="شهر";term3.textContent="شهر";}});
// FAQ accordion
document.querySelectorAll(".accordion-item").forEach(item=>{item.querySelector(".accordion-header").addEventListener("click",()=>{item.classList.toggle("open");});});
// Footer year
document.getElementById("year").textContent=new Date().getFullYear();
// Signup form
const form=document.getElementById("signupForm"),formMsg=document.getElementById("formMsg");
form.addEventListener("submit",(e)=>{e.preventDefault();const email=form.email.value.trim();if(!email||!/\S+@\S+\.\S+/.test(email)){formMsg.textContent="الرجاء إدخال بريد إلكتروني صالح.";formMsg.style.color="var(--primary)";return;}formMsg.textContent="تم التسجيل بنجاح! شكرًا لك.";formMsg.style.color="var(--success)";form.reset();});
</script>
</body>
</html>
