<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="موقع أسرة الكاروز - اجتماع الشباب والشابات بكنيسة العذراء مريم بالبداري">
  <meta name="keywords" content="أسرة الكاروز, كنيسة العذراء مريم, شباب, شابات, اجتماعات, مسيحية, أرثوذكسية">
  <meta name="author" content="أسرة الكاروز">
  <title>أسرة الكاروز</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700;900&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Cairo', sans-serif;
      background: linear-gradient(to bottom, #f3f4f6, #ffffff);
      color: #222;
      line-height: 1.8;
      transition: background 0.5s ease-in-out;
    }

    header {
      background: linear-gradient(to right, #003366, #0059b3);
      color: white;
      text-align: center;
      padding: 40px 20px;
      animation: fadeInDown 1s ease-out;
    }

    header img {
      width: 160px;
      margin-bottom: 15px;
      animation: zoomIn 1s ease-out;
    }

    header h1 {
      font-size: 3em;
      font-weight: 900;
    }

    header h2 {
      font-size: 1.5em;
      opacity: 0.9;
    }

    nav {
      background-color: #002b55;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.2);
    }

    nav a {
      color: white;
      text-decoration: none;
      padding: 15px 25px;
      font-weight: bold;
      font-size: 1.1em;
      transition: all 0.3s ease;
      border-radius: 10px;
    }

    nav a:hover,
    nav a.active-link {
      background-color: #0077cc;
      transform: scale(1.05);
      box-shadow: 0 4px 15px rgba(0, 119, 204, 0.4);
    }

    .section {
      display: none;
      padding: 60px 20px;
      text-align: center;
      animation: fadeIn 0.8s ease-out;
    }

    .section.active {
      display: block;
    }

    .section h2 {
      color: #004080;
      font-size: 2.8em;
      margin-bottom: 20px;
      font-weight: 900;
    }

    .section p {
      font-size: 1.2em;
      max-width: 750px;
      margin: auto;
      opacity: 0.95;
    }

    .btn-link {
      margin-top: 30px;
      display: inline-block;
      padding: 14px 30px;
      background: #004080;
      color: white;
      text-decoration: none;
      border-radius: 10px;
      font-size: 1.1em;
      font-weight: bold;
      transition: all 0.3s ease-in-out;
    }

    .btn-link:hover {
      background: #0066cc;
      transform: scale(1.05);
    }

    footer {
      background-color: #003366;
      color: white;
      text-align: center;
      padding: 20px 10px;
      margin-top: 60px;
      font-size: 0.9em;
    }

    footer a {
      color: #aee4ff;
      text-decoration: none;
    }

    .gallery img {
      width: 300px;
      height: 200px;
      border-radius: 12px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
      transition: transform 0.5s ease, box-shadow 0.3s ease;
    }

    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
    }

    @keyframes fadeInDown {
      from {
        transform: translateY(-50px);
        opacity: 0;
      }
      to {
        transform: translateY(0);
        opacity: 1;
      }
    }

    @keyframes zoomIn {
      from {
        transform: scale(0.8);
        opacity: 0;
      }
      to {
        transform: scale(1);
        opacity: 1;
      }
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    @media (max-width: 768px) {
      header h1 {
        font-size: 2.2em;
      }
      .section h2 {
        font-size: 2em;
      }
      nav a {
        padding: 10px 15px;
        font-size: 1em;
      }
      .gallery img {
        width: 90%;
        height: auto;
      }
    }
  </style>
</head>
<body>

  <header>
    <img src="https://i.postimg.cc/vTLYWwg4/487031869-529154986552598-2072131729727778558-n.png" alt="شعار أسرة الكاروز">
    <h1>أسرة الكاروز</h1>
    <h2>اجتماع الشباب والشابات بكنيسة العذراء مريم بالبداري</h2>
  </header>

  <nav>
    <a href="#about" onclick="showSection('about')">من نحن</a>
    <a href="#facebook" onclick="showSection('facebook')">فيسبوك</a>
    <a href="#whatsapp" onclick="showSection('whatsapp')">واتساب</a>
    <a href="#sarahah" onclick="showSection('sarahah')">الصراحة</a>
    <a href="#app" onclick="showSection('app')">برنامج الكاروز</a>
    <a href="#gallery" onclick="showSection('gallery')">صورنا</a>
  </nav>

  <div id="about" class="section active">
    <h2>من نحن</h2>
    <p>نحن أسرة مسيحية أرثوذكسية لاجتماع الشباب والشابات</p>
  </div>

  <div id="facebook" class="section">
    <h2>صفحتنا على فيسبوك</h2>
    <a class="btn-link" href="https://www.facebook.com/S.t.mark.family" target="_blank">الانتقال إلى الصفحة</a>
  </div>

  <div id="whatsapp" class="section">
    <h2>جروب الواتساب</h2>
    <a class="btn-link" href="https://chat.whatsapp.com/GIdtlyS1ykABhK74OCM09e" target="_blank">الانضمام للجروب</a>
  </div>

  <div id="sarahah" class="section">
    <h2>صارحني</h2>
    <a class="btn-link" href="https://sarhne.sarahah.pro/alkaroz" target="_blank">إرسال رأيك</a>
  </div>

  <div id="app" class="section">
    <h2>تحميل برنامج الكاروز</h2>
    <a class="btn-link" href="https://alkaroz.blogspot.com/2025/03/blog-post.html" target="_blank">تحميل الآن</a>
  </div>

  <div id="gallery" class="section">
    <h2>صور من اجتماعتنا</h2>
    <div class="gallery" style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center; margin-top: 30px;">
      <img src="https://i.postimg.cc/FsGZZPLq/496956452-122125685750735002-5455872153711139610-n.jpg" alt="صورة 1">
      <img src="https://i.postimg.cc/qMpw2fzy/496061475-122125685630735002-5854248544752354944-n.jpg" alt="صورة 2">
      <img src="https://i.postimg.cc/rwxpTHNZ/IMG.jpg" alt="صورة 3">
    </div>
  </div>

  <footer>
    &copy; 2025 أسرة الكاروز - جميع الحقوق محفوظة.<br>
    <a href="https://www.facebook.com/S.t.mark.family" target="_blank">تابعنا على فيسبوك</a>
  </footer>

  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(section => section.classList.remove('active'));

      const target = document.getElementById(id);
      if (target) {
        target.classList.add('active');
      }

      document.querySelectorAll("nav a").forEach(link => link.classList.remove("active-link"));
      const activeLink = document.querySelector(`nav a[href="#${id}"]`);
      if (activeLink) {
        activeLink.classList.add("active-link");
      }

      history.replaceState(null, null, "#" + id);
    }

    window.addEventListener('load', () => {
      const hash = window.location.hash.substring(1);
      if (hash) {
        showSection(hash);
      } else {
        document.querySelector("nav a[href='#about']").classList.add("active-link");
      }
    });
  </script>

</body>
</html>
