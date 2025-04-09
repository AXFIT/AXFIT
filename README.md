- 👋 Hi, I’m @AXFIT
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
AXFIT/AXFIT is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AXFIT - ملابس رياضية رجالية</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
  <style>
    html {
      scroll-behavior: smooth;
    }
    body {
      margin: 0;
      font-family: 'Cairo', sans-serif;
      background-color: #fff;
      color: #000;
    }
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background-color: #000;
      color: #fff;
    }
    .logo {
      font-size: 1.8rem;
      font-weight: bold;
    }
    nav a {
      margin: 0 1rem;
      color: #fff;
      text-decoration: none;
    }
    .language-switcher {
      display: inline-block;
      margin-right: 1rem;
    }
    .language-switcher select {
      padding: 0.4rem;
      font-size: 1rem;
      border-radius: 5px;
      border: none;
    }
    .hero {
      background: url('your-banner.jpg') no-repeat center center/cover;
      height: 80vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: #fff;
      position: relative;
    }
    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; width: 100%; height: 100%;
      background: rgba(0,0,0,0.5);
    }
    .hero-content {
      position: relative;
      z-index: 2;
    }
    .hero h1 {
      font-size: 3rem;
      margin-bottom: 1rem;
    }
    .hero button {
      background: #fff;
      color: #000;
      border: none;
      padding: 0.75rem 1.5rem;
      font-size: 1rem;
      cursor: pointer;
      border-radius: 5px;
    }
    .filters {
      padding: 2rem;
      background: #f5f5f5;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
    }
    .filters select {
      padding: 0.5rem;
      font-size: 1rem;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 1.5rem;
      padding: 2rem;
    }
    .product {
      border: 1px solid #ddd;
      border-radius: 10px;
      overflow: hidden;
      text-align: center;
      padding: 1rem;
    }
    .product img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 8px;
    }
    .product h3 {
      margin: 0.5rem 0;
    }
    .product button {
      margin-top: 0.5rem;
      background: #000;
      color: #fff;
      border: none;
      padding: 0.5rem 1rem;
      cursor: pointer;
      border-radius: 5px;
    }
    .auth {
      max-width: 400px;
      margin: 2rem auto;
      padding: 2rem;
      border: 1px solid #ddd;
      border-radius: 10px;
      text-align: center;
    }
    .auth input {
      display: block;
      width: 100%;
      padding: 0.75rem;
      margin: 1rem 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .auth button {
      background: #000;
      color: #fff;
      border: none;
      padding: 0.75rem 1.5rem;
      cursor: pointer;
      border-radius: 5px;
      width: 100%;
    }
    .contact {
      max-width: 600px;
      margin: 2rem auto;
      padding: 2rem;
      border: 1px solid #ddd;
      border-radius: 10px;
    }
    .contact h2 {
      text-align: center;
      margin-bottom: 1rem;
    }
    .contact input, .contact textarea {
      display: block;
      width: 100%;
      padding: 0.75rem;
      margin: 1rem 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .contact button {
      background: #000;
      color: #fff;
      border: none;
      padding: 0.75rem 1.5rem;
      cursor: pointer;
      border-radius: 5px;
      width: 100%;
    }
    footer {
      background: #000;
      color: #fff;
      padding: 2rem;
      text-align: center;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">AXFIT</div>
    <nav>
      <a href="#filters">المنتجات</a>
      <a href="#auth">حسابي</a>
      <a href="#contact">تواصل معنا</a>
      <div class="language-switcher">
        <select onchange="changeLanguage(this.value)">
          <option value="ar" selected>العربية 🇸🇦</option>
          <option value="fr">Français 🇫🇷</option>
          <option value="en">English 🇬🇧</option>
        </select>
      </div>
    </nav>
  </header>

  <section class="hero">
    <div class="hero-content">
      <h1>أطلق طاقتك مع AXFIT</h1>
      <p>ملابس رياضية رجالية تجمع بين الأناقة والأداء</p>
      <button onclick="document.getElementById('filters').scrollIntoView({behavior: 'smooth'})">تسوق الآن</button>
    </div>
  </section>

  <section id="filters" class="filters">
    <select>
      <option>اختر المقاس</option>
      <option>M</option>
      <option>L</option>
      <option>XL</option>
    </select>
    <select>
      <option>اختر اللون</option>
      <option>أسود</option>
      <option>أبيض</option>
      <option>أحمر</option>
    </select>
    <select>
      <option>اختر النوع</option>
      <option>تيشيرت</option>
      <option>بنطال</option>
      <option>جاكيت</option>
    </select>
  </section>

  <section class="products">
    <div class="product">
      <img src="product1.jpg" alt="منتج 1">
      <h3>تيشيرت رياضي</h3>
      <p>3500 دج</p>
      <button>أضف إلى السلة</button>
    </div>
    <div class="product">
      <img src="product2.jpg" alt="منتج 2">
      <h3>بنطال رياضي</h3>
      <p>4500 دج</p>
      <button>أضف إلى السلة</button>
    </div>
    <div class="product">
      <img src="product3.jpg" alt="منتج 3">
      <h3>جاكيت رياضي</h3>
      <p>6500 دج</p>
      <button>أضف إلى السلة</button>
    </div>
  </section>

  <section id="auth" class="auth">
    <h2>تسجيل الدخول</h2>
    <input type="email" placeholder="البريد الإلكتروني">
    <input type="password" placeholder="كلمة المرور">
    <button>تسجيل الدخول</button>
    <hr>
    <h2>إنشاء حساب جديد</h2>
    <input type="text" placeholder="الاسم الكامل">
    <input type="email" placeholder="البريد الإلكتروني">
    <input type="password" placeholder="كلمة المرور">
    <button>إنشاء الحساب</button>
  </section>

  <section id="contact" class="contact">
    <h2>تواصل معنا</h2>
    <input type="text" placeholder="الاسم الكامل">
    <input type="email" placeholder="البريد الإلكتروني">
    <textarea rows="5" placeholder="اكتب رسالتك هنا..."></textarea>
    <button>إرسال</button>
  </section>

  <footer>
    <p>© 2025 AXFIT. جميع الحقوق محفوظة.</p>
  </footer>

  <script>
    function changeLanguage(lang) {
      alert('تم اختيار اللغة: ' + lang);
    }
  </script>
</body>
</html>
