<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <title>AI Merchant - Your Smart E-commerce Platform</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@600;400&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Cairo', sans-serif;
      margin: 0;
      background: linear-gradient(135deg, #f6d365 0%, #fda085 100%);
      color: #222;
    }
    .container {
      width: 90%;
      max-width: 1200px;
      margin: auto;
    }
    header {
      background: #fff8f0;
      border-radius: 0 0 36px 36px;
      padding: 40px 0 30px 0;
      box-shadow: 0 6px 24px #fdbb8433;
      text-align: center;
      position: relative;
      margin-bottom: 40px;
    }
    .logo-box {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      margin-bottom: 18px;
    }
    .logo-img {
      width: 110px;
      height: 110px;
      background: linear-gradient(135deg, #fff6e5 0%, #ffd6b0 100%);
      border-radius: 50%;
      box-shadow: 0 4px 18px #ffb36c33;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      margin-bottom: 12px;
      border: 3px solid #ff6f3c;
    }
    .logo-img img {
      width: 72px;
      height: 72px;
      object-fit: contain;
      display: block;
    }
    .logo-text {
      font-weight: 700;
      font-size: 1.35rem;
      color: #ff6f3c;
      letter-spacing: 2px;
      font-family: 'Cairo', sans-serif;
    }
    h1 {
      font-size: 2.4rem;
      color: #ff6f3c;
      margin-bottom: 12px;
    }
    h2 {
      color: #222;
      margin-top: 0;
    }
    .subtitle {
      font-size: 1.25rem;
      color: #555;
      margin-bottom: 20px;
    }
    .cta-btn {
      background: linear-gradient(90deg,#ff6f3c,#ffc93c);
      color: #fff;
      border: none;
      border-radius: 28px;
      padding: 15px 48px;
      font-size: 1.1rem;
      cursor: pointer;
      margin-top: 20px;
      font-weight: bold;
      letter-spacing: 1px;
      transition: background .2s;
      box-shadow: 0 2px 12px #ffbb3c44;
    }
    .cta-btn:hover {
      background: linear-gradient(90deg,#ffc93c,#ff6f3c);
    }
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(230px,1fr));
      gap: 32px;
      margin: 60px 0;
    }
    .feature {
      background: #fff;
      border-radius: 18px;
      box-shadow: 0 1px 8px #ffb36c2a;
      padding: 28px 20px 20px 20px;
      text-align: center;
      transition: transform .2s;
      position: relative;
    }
    .feature:hover {
      transform: translateY(-7px) scale(1.03);
    }
    .feature img {
      width: 54px;
      margin-bottom: 15px;
    }
    .feature-title {
      font-weight: bold;
      color: #ff6f3c;
      margin-bottom: 7px;
      font-size: 1.13rem;
    }
    .feature-desc {
      font-size: 1rem;
      color: #333;
      min-height: 52px;
    }
    .how-it-works {
      background: #fff8f0;
      border-radius: 22px;
      padding: 30px 16px 22px 16px;
      margin-bottom: 40px;
      box-shadow: 0 2px 12px #fdbb8422;
    }
    .steps {
      display: flex;
      flex-wrap: wrap;
      gap: 24px;
      justify-content: center;
      align-items: flex-start;
      margin-top: 16px;
      margin-bottom: 0;
      text-align: left;
    }
    .step {
      background: #fff;
      border-radius: 14px;
      box-shadow: 0 1px 7px #ffb36c1a;
      padding: 22px 16px;
      flex: 1 1 180px;
      max-width: 230px;
      min-width: 170px;
      margin-bottom: 8px;
    }
    .step-num {
      background: #ffc93c;
      color: #fff;
      width: 36px;
      height: 36px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      border-radius: 50%;
      font-size: 1.3rem;
      font-weight: bold;
      margin-right: 10px;
    }
    .subscribe {
      background: #fff;
      border-radius: 22px;
      box-shadow: 0 2px 14px #ffb36c36;
      padding: 36px 20px 26px 20px;
      text-align: center;
      margin: 60px auto 30px auto;
      max-width: 440px;
    }
    .subscribe h3 {
      color: #ff6f3c;
      font-size: 1.4rem;
      margin-bottom: 15px;
    }
    .form-group {
      margin-bottom: 13px;
      text-align: left;
    }
    .form-group label {
      display: block;
      font-size: 1rem;
      margin-bottom: 5px;
      color: #444;
    }
    .form-group input {
      width: 100%;
      padding: 11px 12px;
      border-radius: 9px;
      border: 1px solid #ffc93c;
      font-size: 1rem;
      box-sizing: border-box;
    }
    .sub-btn {
      background: linear-gradient(90deg,#ff6f3c,#ffc93c);
      color: #fff;
      border: none;
      border-radius: 22px;
      padding: 12px 38px;
      font-size: 1.07rem;
      cursor: pointer;
      font-weight: bold;
      margin-top: 7px;
      transition: background .2s;
    }
    .sub-btn:hover {
      background: linear-gradient(90deg,#ffc93c,#ff6f3c);
    }
    .testimonials {
      margin: 40px 0 20px 0;
      text-align: center;
    }
    .testimonial {
      background: #fff;
      display: inline-block;
      border-radius: 14px;
      box-shadow: 0 1px 7px #ffb36c2a;
      padding: 16px 22px;
      margin: 8px 12px;
      min-width: 240px;
      max-width: 350px;
      vertical-align: top;
      color: #444;
    }
    .testimonial .author {
      color: #ff6f3c;
      font-weight: bold;
      font-size: 1.03rem;
      margin-top: 7px;
    }
    .faq {
      margin: 42px auto 32px auto;
      max-width: 700px;
      background: #fff8f0;
      border-radius: 18px;
      box-shadow: 0 2px 12px #fdbb842a;
      padding: 28px 18px;
    }
    .faq h3 {
      color: #ff6f3c;
      margin-bottom: 19px;
      font-size: 1.2rem;
    }
    .faq-q {
      color: #222;
      font-weight: bold;
      margin-bottom: 3px;
      margin-top: 14px;
    }
    .faq-a {
      color: #444;
      font-size: 1rem;
      margin-bottom: 7px;
    }
    footer {
      background: #ff6f3c;
      color: #fff;
      text-align: center;
      border-radius: 26px 26px 0 0;
      padding: 18px 0 10px 0;
      margin-top: 38px;
      font-size: 1.08rem;
      letter-spacing: 0.5px;
    }
    .footer-links {
      margin: 7px 0;
      font-size: .99rem;
    }
    .footer-links a {
      color: #ffe1bb;
      margin: 0 10px;
      text-decoration: none;
      transition: color .2s;
    }
    .footer-links a:hover {
      color: #fff;
      text-decoration: underline;
    }
    @media (max-width: 700px){
      .features {grid-template-columns: 1fr;}
      .steps {flex-direction: column;}
      .testimonial {max-width: 90vw;}
      header {padding: 18px 0 18px 0;}
    }
  </style>
</head>
<body>
  <header>
    <div class="logo-box">
      <div class="logo-img">
        <!-- AI Merchant Logo: Modern, tech/ecommerce style -->
        <img src="https://cdn-icons-png.flaticon.com/512/3004/3004458.png" alt="AI Merchant Logo">
      </div>
      <div class="logo-text">AI Merchant</div>
    </div>
    <h1>Launch Your Smart Store with AI Merchant</h1>
    <div class="subtitle">
      AI manages your entire e-commerce business…<br>
      Focus on profits and let us handle the rest!
    </div>
    <button class="cta-btn" onclick="document.getElementById('subscribe').scrollIntoView({behavior:'smooth'})">Start Free Now</button>
  </header>

  <div class="container">
    <h2 style="text-align:center;margin-bottom:10px;">All Features in One Place</h2>
    <div class="features">
      <div class="feature">
        <img src="https://cdn-icons-png.flaticon.com/512/2332/2332670.png" alt="Product Selection">
        <div class="feature-title">Profitable Product Selection</div>
        <div class="feature-desc">AI analyzes your local market and recommends the most in-demand and profitable products.</div>
      </div>
      <div class="feature">
        <img src="https://cdn-icons-png.flaticon.com/512/2516/2516746.png" alt="Stock Management">
        <div class="feature-title">Automated Inventory Management</div>
        <div class="feature-desc">Alerts when stock is low and automatic integration with suppliers to restock directly.</div>
      </div>
      <div class="feature">
        <img src="https://cdn-icons-png.flaticon.com/512/2894/2894771.png" alt="Dynamic Pricing">
        <div class="feature-title">Smart Dynamic Pricing</div>
        <div class="feature-desc">The system automatically adjusts prices according to market demand and competition.</div>
      </div>
      <div class="feature">
        <img src="https://cdn-icons-png.flaticon.com/512/2922/2922676.png" alt="Smart Marketing">
        <div class="feature-title">AI-Powered Targeted Marketing</div>
        <div class="feature-desc">Facebook, Instagram, Google campaigns… everything managed automatically for the best results.</div>
      </div>
      <div class="feature">
        <img src="https://cdn-icons-png.flaticon.com/512/1250/1250620.png" alt="24/7 Support">
        <div class="feature-title">Smart 24/7 Customer Support</div>
        <div class="feature-desc">A chatbot responds to customers, tracks orders, and suggests related products any time.</div>
      </div>
      <div class="feature">
        <img src="https://cdn-icons-png.flaticon.com/512/1041/1041916.png" alt="Shipping Integration">
        <div class="feature-title">Integrated Shipping Solutions</div>
        <div class="feature-desc">The system automatically coordinates with local shipping companies for fast delivery.</div>
      </div>
    </div>

    <div class="how-it-works">
      <h2 style="text-align:center;">How Does It Work?</h2>
      <div class="steps">
        <div class="step">
          <span class="step-num">1</span>
          Create your account in minutes — no technical experience needed.
        </div>
        <div class="step">
          <span class="step-num">2</span>
          Get profitable product suggestions from AI.
        </div>
        <div class="step">
          <span class="step-num">3</span>
          Launch your online store automatically.
        </div>
        <div class="step">
          <span class="step-num">4</span>
          Receive orders and let the platform handle everything else!
        </div>
      </div>
    </div>

    <div class="subscribe" id="subscribe">
      <h3>Try AI Merchant for Free Now 👇</h3>
      <form>
        <div class="form-group">
          <label for="name">Full Name</label>
          <input type="text" id="name" name="name" placeholder="Enter your name" required>
        </div>
        <div class="form-group">
          <label for="email">Email Address</label>
          <input type="email" id="email" name="email" placeholder="example@email.com" required>
        </div>
        <button type="submit" class="sub-btn">Subscribe for Free</button>
      </form>
      <div style="font-size:.97rem;color:#888;margin-top:10px;">No credit card required for the free trial!</div>
    </div>

    <div class="testimonials">
      <div class="testimonial">
        <div>I launched my store in less than an hour! Everything is managed automatically.</div>
        <div class="author">Ahmed - Entrepreneur</div>
      </div>
      <div class="testimonial">
        <div>Fewer mistakes and more profits. Best decision I made!</div>
        <div class="author">Noura - Online Store Owner</div>
      </div>
    </div>

    <div class="faq">
      <h3>Frequently Asked Questions</h3>
      <div>
        <div class="faq-q">Do I need technical experience?</div>
        <div class="faq-a">Not at all! Our platform is designed for everyone at any technical level.</div>
        <div class="faq-q">What is the subscription cost?</div>
        <div class="faq-a">You can start for free, and our subscription plans start at an affordable monthly rate.</div>
        <div class="faq-q">How does the platform help me with marketing?</div>
        <div class="faq-a">AI manages marketing campaigns automatically to help you reach your best customers.</div>
        <div class="faq-q">Can I integrate with local suppliers or shipping companies?</div>
        <div class="faq-a">Yes, full integration with suppliers and shipping companies is provided.</div>
      </div>
    </div>
  </div>

  <footer>
    <div class="footer-links">
      <a href="#">About Us</a> |
      <a href="#">Terms & Conditions</a> |
      <a href="#">Support</a> |
      <a href="#">Contact Us</a>
    </div>
    All rights reserved © 2025 AI Merchant
  </footer>
</body>
</html>
