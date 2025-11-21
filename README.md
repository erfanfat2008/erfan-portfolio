<!doctype html>

<html lang="fa" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>عرفان فتحعلی‌زاده — Developer Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <meta name="description" content="پورتفولیو عرفان فتحعلی‌زاده — توسعه‌دهنده فرانت‌اند. پروژه‌ها، خدمات و تماس." />
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#06b6d4; --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.02);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;padding:0;font-family:Inter,system-ui, -apple-system,"Segoe UI", Roboto, "Helvetica Neue", Arial; background:linear-gradient(180deg,#071026 0%, #081227 50%, #0b1220 100%); color:#e6eef6; -webkit-font-smoothing:antialiased;}.container{max-width:1100px;margin:32px auto;padding:24px}
header{display:flex;align-items:center;justify-content:space-between;gap:16px}
.brand{display:flex;align-items:center;gap:12px}
.logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:700;color:#062023}
.brand h1{margin:0;font-size:18px}
nav{display:flex;gap:14px;align-items:center}
nav a{color:var(--muted);text-decoration:none;font-weight:600}
.btn{background:var(--accent);color:#062023;padding:10px 14px;border-radius:10px;font-weight:700;text-decoration:none}

/* hero */
.hero{display:grid;grid-template-columns:1fr 420px;gap:32px;align-items:center;margin-top:28px}
.intro h2{margin:0;font-size:28px;line-height:1.05}
.intro p{color:var(--muted);margin-top:10px}
.kpis{display:flex;gap:12px;margin-top:18px}
.kpi{background:var(--glass);padding:12px;border-radius:12px;text-align:center;min-width:110px}
.kpi h3{margin:0;font-size:18px}
.kpi p{margin:6px 0 0;color:var(--muted);font-size:13px}

.card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.03);padding:18px;border-radius:14px;backdrop-filter: blur(6px)}

/* project preview */
.preview{height:320px;border-radius:10px;overflow:hidden;display:flex;flex-direction:column}
.preview .mock{flex:1;background:linear-gradient(180deg,#071a24,#05202b);display:flex;flex-direction:column;padding:18px}
.mock .title{font-weight:700}
.mock .meta{margin-top:auto;color:var(--muted);font-size:13px}

/* projects */
.projects{display:grid;grid-template-columns:repeat(2,1fr);gap:16px;margin-top:28px}
.project{padding:14px;border-radius:12px;background:var(--glass-2);border:1px solid rgba(255,255,255,0.02)}
.project h4{margin:0}
.project p{color:var(--muted);font-size:13px}
.actions{display:flex;gap:8px;margin-top:12px}
.link{padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.03);color:var(--muted);text-decoration:none;font-weight:600}

footer{margin-top:40px;padding:18px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.01));display:flex;justify-content:space-between;align-items:center}

/* responsive */
@media (max-width:900px){.hero{grid-template-columns:1fr;}.projects{grid-template-columns:1fr}.preview{height:260px}.logo{width:48px;height:48px}}

/* simple animations */
.fade-up{opacity:0;transform:translateY(10px);animation:fadeUp .7s ease forwards}
.fade-delay{animation-delay:.12s}
.pop{transform-origin:center;animation:pop .7s ease forwards}
@keyframes fadeUp{to{opacity:1;transform:none}}
@keyframes pop{0%{transform:scale(.95);opacity:0}100%{transform:none;opacity:1}}

/* mobile nav */
.mobile-toggle{display:none}
@media (max-width:700px){nav{display:none}.mobile-toggle{display:inline-flex}}

/* theme toggle */
.theme-toggle{background:transparent;border:1px solid rgba(255,255,255,0.04);padding:8px;border-radius:10px;color:var(--muted);font-weight:700}

/* little code block */
pre{background:rgba(0,0,0,0.25);padding:8px;border-radius:8px;color:var(--muted);overflow:auto}

  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">E</div>
        <div>
          <h1>عرفان فتحعلی‌زاده</h1>
          <div style="color:var(--muted);font-size:13px">Front‑End Developer &amp; Web Enthusiast</div>
        </div>
      </div>
      <div style="display:flex;align-items:center;gap:12px">
        <nav>
          <a href="#projects">پروژه‌ها</a>
          <a href="#services">خدمات</a>
          <a href="#contact">تماس</a>
        </nav>
        <button class="theme-toggle" id="themeToggle">حالت</button>
        <a class="btn" href="#contact">استخدام</a>
        <button class="mobile-toggle" aria-label="menu" id="menuBtn">☰</button>
      </div>
    </header><main class="hero">
  <section class="intro card fade-up">
    <h2>سلام — من عرفان هستم، توسعه‌دهنده فرانت‌اند</h2>
    <p>من صفحات وب واکنش‌گرا، لندینگ پیج‌های جذاب و اپلیکیشن‌های کوچک وب می‌سازم. آماده‌ام پروژه شما را با کیفیت بالا و تحویل سریع انجام دهم.</p>

    <div class="kpis">
      <div class="kpi pop">
        <h3>10+</h3>
        <p>نمونه‌کار</p>
      </div>
      <div class="kpi pop fade-delay">
        <h3>3</h3>
        <p>ماه تجربهٔ جدی</p>
      </div>
      <div class="kpi pop" style="animation-delay:.24s">
        <h3>100%</h3>
        <p>رضایت مشتری</p>
      </div>
    </div>

    <div style="margin-top:18px;display:flex;gap:10px">
      <a class="btn" href="#contact">درخواست قیمت</a>
      <a class="link" href="#projects">مشاهده پروژه‌ها</a>
    </div>
  </section>

  <aside class="card preview fade-up" style="animation-delay:.06s">
    <div class="mock">
      <div style="display:flex;justify-content:space-between;align-items:center">
        <div>
          <div class="title">Portfolio Landing — عرفان</div>
          <div style="color:var(--muted);font-size:13px;margin-top:6px">HTML • CSS • JavaScript • Responsive</div>
        </div>
        <div style="font-size:12px;color:var(--muted)">Live Preview</div>
      </div>

      <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='600' height='200'><rect width='100%' height='100%' fill='%23061b26'/><text x='50%' y='50%' dominant-baseline='middle' text-anchor='middle' font-size='18' fill='%23bfeaf3'>Live demo inside repository</text></svg>" alt="mock" style="width:100%;border-radius:8px;margin-top:12px;object-fit:cover"/>

      <div class="meta">قابلیت واکنش‌پذیری، انیمیشن سبک و نمونه‌کارهای آماده برای کارفرما</div>
    </div>
  </aside>
</main>

<section id="projects" class="projects">
  <div class="project card fade-up">
    <h4>لندینگ پیج فروشگاهی</h4>
    <p>صفحه فرود تک‌صفحه‌ای با فرم تماس و بخش معرفی محصول.</p>
    <div class="actions">
      <a class="link" href="#" onclick="openDemo(event,'/demos/landing.html')">Live</a>
      <a class="link" href="#" onclick="openCode(event,'https://github.com/yourname/portfolio')">Code</a>
    </div>
  </div>

  <div class="project card fade-up" style="animation-delay:.06s">
    <h4>To‑Do App</h4>
    <p>اپ ساده مدیریت کارها با LocalStorage و رابط کاربری جمع‌وجور.</p>
    <div class="actions">
      <a class="link" href="#">Live</a>
      <a class="link" href="#">Code</a>
    </div>
  </div>

  <div class="project card fade-up" style="animation-delay:.12s">
    <h4>ماشین‌حساب</h4>
    <p>ماشین‌حساب پایه با طراحی لمسی و واکنش‌گرا.</p>
    <div class="actions">
      <a class="link" href="#">Live</a>
      <a class="link" href="#">Code</a>
    </div>
  </div>

  <div class="project card fade-up" style="animation-delay:.18s">
    <h4>وب‌اپ هواشناسی</h4>
    <p>نمایش دادهٔ آب‌وهوا از API (نمونهٔ آماده برای توسعه).</p>
    <div class="actions">
      <a class="link" href="#">Live</a>
      <a class="link" href="#">Code</a>
    </div>
  </div>
</section>

<section id="services" style="margin-top:28px">
  <div class="card fade-up">
    <h3>خدمات من</h3>
    <p style="color:var(--muted)">ساخت لندینگ پیج، طراحی صفحات فروشگاهی، پیاده‌سازی فرم‌ها، رفع باگ و بهینه‌سازی رابط کاربری.</p>

    <div style="display:flex;gap:12px;margin-top:12px;flex-wrap:wrap">
      <div class="kpi">لندینگ پیج حرفه‌ای</div>
      <div class="kpi">طراحی ریسپانسیو</div>
      <div class="kpi">ادیت و بهینه‌سازی</div>
    </div>
  </div>
</section>

<section id="contact" style="margin-top:28px">
  <div class="card">
    <h3>تماس با من</h3>
    <p style="color:var(--muted)">آماده‌ام در پروژه بعدی‌تان کمک کنم. فرم یا پیام مستقیم به من بفرستید.</p>

    <form id="contactForm" style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-top:12px">
      <input name="name" placeholder="نام شما" style="padding:12px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" required />
      <input name="email" placeholder="ایمیل یا شماره" style="padding:12px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" required />
      <input name="title" placeholder="عنوان پروژه" style="grid-column:1 / -1;padding:12px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" />
      <textarea name="message" placeholder="توضیحات پروژه" style="grid-column:1 / -1;padding:12px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:transparent;color:inherit" rows="4"></textarea>

      <div style="grid-column:1 / -1;display:flex;gap:10px;align-items:center">
        <button type="submit" class="btn">ارسال پیام</button>
        <div style="color:var(--muted);font-size:13px">یا مستقیم پیام در تلگرام: @erfan_dev</div>
      </div>
    </form>

  </div>
</section>

<footer>
  <div style="color:var(--muted);font-size:13px">© عرفان فتحعلی‌زاده — Front‑End Developer</div>
  <div style="display:flex;gap:10px">
    <a class="link" href="#">GitHub</a>
    <a class="link" href="#">LinkedIn</a>
  </div>
</footer>

  </div>  <script>
    // theme toggle (light/dark simple)
    const themeBtn = document.getElementById('themeToggle');
    themeBtn.addEventListener('click',()=>{
      if(document.documentElement.style.getPropertyValue('--bg')===''){
        document.documentElement.style.setProperty('--bg','#ffffff');
      }
      alert('حالت تیره/روشن در نسخه محلی شبیه‌سازی شد — برای انتشار نهایی می‌توان شکل‌دهی کرد.');
    });

    // fake open functions (for demo)
    function openDemo(e,link){e.preventDefault();alert('برای دیدن نسخهٔ آنلاین، این پروژه را در گیت‌هاب منتشر کنید یا از Netlify/Vercel استفاده کنید.');}
    function openCode(e,link){e.preventDefault();window.open('https://github.com/yourname/portfolio','_blank');}

    // contact form (local demo)
    document.getElementById('contactForm').addEventListener('submit',function(e){
      e.preventDefault();
      alert('پیام شما ثبت شد — در نسخهٔ واقعی باید فرم را به back-end یا سرویس ایمیل وصل کنید.');
      this.reset();
    });

    // reveal animations
    document.querySelectorAll('.fade-up').forEach((el,i)=>{el.style.animationDelay=(i*120)+'ms';el.classList.add('fade-up');});
  </script></body>
</html>
