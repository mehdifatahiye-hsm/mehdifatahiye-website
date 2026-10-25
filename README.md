<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#f5f2eb">
  <title>Mehdi Fatahiye | Architect</title>
  <meta name="description" content="Mehdi Fatahiye — Architect. Architecture, interior design, renovation and construction management.">
 ```css
/* ===== FULLSCREEN ARCHITECTURE GALLERY ===== */

.lightbox {
  position: fixed;
  inset: 0;
  z-index: 9999;
  display: none;
  align-items: center;
  justify-content: center;
  padding: 0;
  background: #e9e5db;
  overflow: hidden;
}

.lightbox.open {
  display: flex;
}

/* Main image area */
.lightbox-content {
  position: relative;
  width: 100vw;
  height: 100vh;
  height: 100dvh;
  max-width: none;
  min-height: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

/* Show the complete image without cropping */
.lightbox-image {
  display: block;
  width: 100%;
  height: 100%;
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
  border: 0;
  box-shadow: none;
}

/* Warm background instead of black */
.lightbox {
  background: #e9e5db;
}

/* Close button */
.lightbox-close {
  position: absolute;
  z-index: 5;
  top: 20px;
  right: 22px;
  width: 44px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #344033;
  background: rgba(248, 246, 239, 0.88);
  border: 1px solid rgba(70, 80, 62, 0.25);
  border-radius: 50%;
  font-size: 26px;
  cursor: pointer;
}

/* Previous and next buttons */
.lightbox-nav {
  position: absolute;
  z-index: 5;
  top: 50%;
  transform: translateY(-50%);
  width: 48px;
  height: 48px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #344033;
  background: rgba(248, 246, 239, 0.88);
  border: 1px solid rgba(70, 80, 62, 0.25);
  border-radius: 50%;
  font-size: 28px;
  cursor: pointer;
  transition: background 0.2s ease, transform 0.2s ease;
}

.lightbox-nav:hover {
  background: #fffdf7;
}

.lightbox-prev {
  left: 20px;
}

.lightbox-next {
  right: 20px;
}

/* Project title and image counter */
.lightbox-caption {
  position: absolute;
  z-index: 5;
  left: 50%;
  bottom: 20px;
  transform: translateX(-50%);
  padding: 9px 16px;
  color: #344033;
  background: rgba(248, 246, 239, 0.88);
  border: 1px solid rgba(70, 80, 62, 0.15);
  border-radius: 2px;
  font-size: 11px;
  letter-spacing: 1.5px;
  text-align: center;
  white-space: nowrap;
}

/* Subtle watermark over the image */
.lightbox-content::after {
  content: "MEHDI FATAHIYE  ·  ARCHITECTURE";
  position: absolute;
  z-index: 3;
  right: 28px;
  bottom: 28px;
  padding: 7px 10px;
  color: rgba(255, 255, 255, 0.82);
  background: rgba(42, 47, 38, 0.24);
  border: 1px solid rgba(255, 255, 255, 0.22);
  font-size: 9px;
  letter-spacing: 2px;
  pointer-events: none;
  text-shadow: 0 1px 3px rgba(0, 0, 0, 0.35);
}

/* Keyboard-focus accessibility */
.lightbox-close:focus-visible,
.lightbox-nav:focus-visible {
  outline: 2px solid #68775a;
  outline-offset: 4px;
}

/* Mobile adjustments */
@media (max-width: 680px) {
  .lightbox-close {
    top: 12px;
    right: 12px;
    width: 40px;
    height: 40px;
  }

  .lightbox-nav {
    width: 40px;
    height: 40px;
    font-size: 23px;
  }

  .lightbox-prev {
    left: 10px;
  }

  .lightbox-next {
    right: 10px;
  }

  .lightbox-caption {
    bottom: 12px;
    max-width: 75vw;
    white-space: normal;
    font-size: 10px;
  }

  .lightbox-content::after {
    right: 12px;
    bottom: 58px;
    font-size: 8px;
    letter-spacing: 1px;
  }
}
```
 <style>
    :root{--paper:#f5f2eb;--ink:#292a27;--muted:#77766f;--green:#405b31;--line:#dedbd2;--white:#fbfaf6}
    *{box-sizing:border-box}
    html{scroll-behavior:smooth;scroll-padding-top:90px}
    body{margin:0;background:var(--paper);color:var(--ink);font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Arial,sans-serif;-webkit-font-smoothing:antialiased}
    a{color:inherit;text-decoration:none}
    button{font:inherit}
    .topbar{position:absolute;top:0;left:0;width:100%;padding:28px 5%;display:flex;align-items:center;justify-content:space-between;z-index:5}
    .brand{display:flex;align-items:center;gap:15px}.brand-mark{width:48px;height:48px;flex-shrink:0}
    .brand-name{font-size:15px;letter-spacing:4px;font-weight:500}.brand-subtitle{margin-top:5px;font-size:10px;letter-spacing:5px;color:var(--muted)}
    .navigation{display:flex;align-items:center;gap:25px;font-size:11px;letter-spacing:1px}.navigation a{transition:color .2s}.navigation a:hover{color:var(--green)}
    .language{padding-left:18px;border-left:1px solid var(--line);white-space:nowrap}.language button{border:0;background:none;padding:0 2px;color:var(--muted);cursor:pointer;font-size:11px}.language button.active{color:var(--green);font-weight:700}
    .hero{min-height:100svh;position:relative;display:grid;grid-template-columns:34% 66%;align-items:center;padding:120px 5% 65px;overflow:hidden}
    .hero-copy{position:relative;z-index:2;align-self:center;padding-bottom:20px}
    h1{margin:0;font-size:clamp(40px,5vw,72px);line-height:1.12;font-weight:400;letter-spacing:-2px}
    .role{margin:12px 0 0;font-size:clamp(19px,2vw,27px);font-weight:300;letter-spacing:7px;color:var(--muted)}
    .small-line{width:45px;height:1px;margin:32px 0 24px;background:var(--green)}
    .tagline{max-width:310px;margin:0;font-size:clamp(17px,1.7vw,23px);line-height:1.6;font-weight:300;color:#66655f}
    .scroll-link{display:inline-flex;align-items:center;gap:15px;margin-top:55px;color:var(--muted);font-size:10px;letter-spacing:2px}
    .scroll-arrow{color:var(--green);font-size:25px;font-weight:300}
    .hero-art{width:100%;align-self:center;margin-left:-3%}.hero-art svg{display:block;width:100%;height:auto;overflow:visible}
    .sketch-line{fill:none;stroke:#817c70;stroke-width:1.1;stroke-linecap:round;stroke-linejoin:round;opacity:.72}
    .sketch-light{fill:none;stroke:#b4a58e;stroke-width:1;stroke-linecap:round;opacity:.6}
    .sketch-dark{fill:none;stroke:#4b4a43;stroke-width:2;stroke-linecap:round;opacity:.7}
    .section{padding:100px 7%;border-top:1px solid var(--line)}
    .section-label{color:var(--green);font-size:10px;letter-spacing:3px;text-transform:uppercase}
    .section-heading{display:flex;justify-content:space-between;align-items:end;gap:24px;margin-bottom:42px}
    h2{margin:15px 0 0;font-size:clamp(34px,4vw,52px);font-weight:400;letter-spacing:-1px}
    .intro{max-width:370px;color:var(--muted);font-size:14px;line-height:1.8}
    .project-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}
    .project-card{min-width:0;border:1px solid var(--line);background:rgba(255,255,255,.18);transition:transform .25s,border-color .25s}
    .project-card:hover{transform:translateY(-4px);border-color:#b8b5a9}.project-card{cursor:pointer}.project-card:focus-visible{outline:2px solid var(--green);outline-offset:3px}
    .project-visual{aspect-ratio:4/3;display:grid;place-items:center;background:#e9e5db;color:#817c70;overflow:hidden}
    .project-visual img{width:100%;height:100%;object-fit:cover;display:block}
    .visual-mark{font-size:11px;letter-spacing:2px;text-transform:uppercase}
    .project-info{padding:20px}.project-number{font-size:10px;letter-spacing:2px;color:var(--green)}
    .project-info h3{font-size:21px;font-weight:400;margin:10px 0 8px}
    .project-info p{font-size:13px;line-height:1.7;color:var(--muted);margin:0}
    .about-layout{display:grid;grid-template-columns:1fr 1fr;gap:9%;align-items:start}
    .about-copy{font-size:16px;line-height:1.9;color:#66655f;max-width:600px}
    .about-copy p:first-child{margin-top:0}
    .facts{border-top:1px solid var(--line)}
    .fact{display:flex;justify-content:space-between;gap:20px;padding:17px 0;border-bottom:1px solid var(--line);font-size:13px}
    .fact span:first-child{color:var(--muted)}.fact span:last-child{text-align:right}
    .service-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:18px}
    .service{border-top:1px solid var(--green);padding:23px 5px 0}
    .service-index{font-size:11px;color:var(--green);letter-spacing:2px}
    .service h3{font-size:22px;font-weight:400;margin:18px 0 10px}
    .service p{font-size:14px;line-height:1.8;color:var(--muted);margin:0}
    .contact-panel{display:flex;align-items:flex-end;justify-content:space-between;gap:28px}
    .contact-panel h2{max-width:600px}
    .contact-details{font-size:14px;line-height:2;color:var(--muted)}
    .contact-details a{color:var(--green);border-bottom:1px solid var(--line)}
    footer{padding:25px 7%;border-top:1px solid var(--line);color:var(--muted);font-size:11px;letter-spacing:1px;display:flex;justify-content:space-between;gap:15px}
    .lightbox{display:none;position:fixed;inset:0;z-index:50;background:rgba(20,21,18,.94);align-items:center;justify-content:center;padding:24px}
    .lightbox.open{display:flex}.lightbox-content{position:relative;width:min(100%,1100px);display:flex;align-items:center;justify-content:center;min-height:60vh}
    .lightbox-image{max-width:100%;max-height:78vh;object-fit:contain;display:block}.lightbox-close,.lightbox-nav{position:absolute;border:1px solid rgba(255,255,255,.35);background:rgba(0,0,0,.2);color:#fff;cursor:pointer;display:grid;place-items:center}
    .lightbox-close{top:-42px;right:0;width:38px;height:38px;font-size:22px}.lightbox-nav{top:50%;transform:translateY(-50%);width:44px;height:44px;font-size:30px}.lightbox-prev{left:0}.lightbox-next{right:0}
    .lightbox-caption{position:absolute;bottom:-38px;left:0;right:0;text-align:center;color:#eee;font-size:12px;letter-spacing:1px}
    @media(max-width:680px){.lightbox{padding:15px}.lightbox-content{min-height:45vh}.lightbox-image{max-height:72vh}.lightbox-prev{left:0}.lightbox-next{right:0}.lightbox-nav{width:36px;height:36px;background:rgba(0,0,0,.55)}}
    [dir="rtl"] body{font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Tahoma,Arial,sans-serif}
    [dir="rtl"] .navigation{letter-spacing:0}[dir="rtl"] .brand-subtitle{letter-spacing:2px}
    [dir="rtl"] .section-label{letter-spacing:1px}[dir="rtl"] .fact span:last-child{text-align:left}
    @media(max-width:900px){.topbar{padding:22px 5%}.navigation{gap:14px}.project-grid{grid-template-columns:repeat(2,minmax(0,1fr))}.hero{grid-template-columns:40% 60%}.about-layout{gap:5%}}
    @media(max-width:680px){
      html{scroll-padding-top:70px}.topbar{padding:18px 6%}.brand{gap:0}.brand-mark{width:43px;height:43px}.brand-name{display:none}
      .navigation{gap:0}.navigation .nav-link{display:none}.navigation .language{padding-left:0;border:0;font-size:10px}
      .hero{min-height:100svh;grid-template-columns:1fr;grid-template-rows:auto 1fr;padding:105px 7% 24px;align-content:center}
      .hero-copy{padding:15px 0 0}h1{font-size:clamp(38px,11vw,58px);letter-spacing:-1.5px}.role{font-size:18px;letter-spacing:6px}
      .small-line{margin:22px 0 16px}.tagline{font-size:17px}.scroll-link{margin-top:24px}
      .hero-art{width:112%;margin:5px 0 0 -6%;align-self:center}
      .section{padding:72px 7%}.section-heading{display:block;margin-bottom:28px}.intro{margin-top:17px}
      .project-grid,.service-grid{grid-template-columns:1fr}.project-visual{aspect-ratio:5/3}
      .about-layout{grid-template-columns:1fr;gap:28px}.contact-panel{display:block}.contact-details{margin-top:28px}
      footer{padding:22px 7%;flex-direction:column}
    }
    @media(prefers-reduced-motion:reduce){html{scroll-behavior:auto}.project-card{transition:none}}
  ```css
/* ===== REFINED ARCHITECTURE PROJECT GALLERY ===== */

#projects {
  padding-top: 110px;
  padding-bottom: 110px;
}

#projects .section-heading {
  margin-bottom: 50px;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 28px;
}

.project-card {
  position: relative;
  overflow: hidden;
  border: 1px solid #e2ded4;
  background: #efebe2;
  cursor: pointer;
  transition: transform .45s ease, box-shadow .45s ease;
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 18px 38px rgba(49, 47, 39, .10);
}

.project-visual {
  position: relative;
  display: block;
  aspect-ratio: 4 / 3;
  overflow: hidden;
  background: #e6e0d4;
}

.project-visual img {
  display: block !important;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform .8s cubic-bezier(.2, .65, .3, 1),
              filter .5s ease;
}

.project-card:hover .project-visual img {
  transform: scale(1.045);
}

/* Project title overlay */

.project-visual::after {
  content: "";
  position: absolute;
  inset: 35% 0 0;
  background: linear-gradient(
    to bottom,
    transparent,
    rgba(27, 29, 24, .72)
  );
  pointer-events: none;
}

.project-visual .visual-mark {
  position: absolute;
  z-index: 2;
  left: 24px;
  bottom: 22px;
  color: #fff;
  font-size: 20px;
  font-weight: 400;
  letter-spacing: 2px;
  text-transform: uppercase;
  text-shadow: 0 1px 8px rgba(0, 0, 0, .15);
}

.project-info {
  padding: 22px 24px 24px;
  background: #f8f5ee;
}

.project-number {
  font-size: 10px;
  letter-spacing: 2px;
  color: #68775a;
}

.project-info h3 {
  margin: 10px 0 7px;
  font-size: 23px;
  font-weight: 400;
  letter-spacing: -.3px;
}

.project-info p {
  margin: 0;
  color: #77766f;
  font-size: 13px;
  line-height: 1.8;
}

/* ===== LARGE, SOFT PROJECT SLIDESHOW ===== */

.lightbox {
  background: rgba(27, 28, 25, .96);
  padding: 55px 30px;
  backdrop-filter: blur(8px);
}

.lightbox-content {
  width: min(100%, 1180px);
  min-height: 65vh;
}

.lightbox-image {
  max-width: 100%;
  max-height: 76vh;
  object-fit: contain;
  border: 1px solid rgba(255, 255, 255, .10);
  box-shadow: 0 20px 65px rgba(0, 0, 0, .25);
}

.lightbox-close,
.lightbox-nav {
  border: 1px solid rgba(255, 255, 255, .28);
  border-radius: 50%;
  background: rgba(255, 255, 255, .07);
  transition: background .25s ease, border-color .25s ease;
}

.lightbox-close:hover,
.lightbox-nav:hover {
  background: rgba(255, 255, 255, .19);
  border-color: rgba(255, 255, 255, .7);
}

.lightbox-close {
  top: -48px;
  right: 0;
}

.lightbox-nav {
  width: 46px;
  height: 46px;
}

.lightbox-caption {
  bottom: -38px;
  color: #e7e2d8;
  font-size: 11px;
  letter-spacing: 2px;
}

@media (max-width: 680px) {
  #projects {
    padding-top: 75px;
    padding-bottom: 75px;
  }

  .project-grid {
    grid-template-columns: 1fr;
    gap: 22px;
  }

  .project-visual {
    aspect-ratio: 4 / 3;
  }

  .project-info {
    padding: 18px;
  }

  .project-visual .visual-mark {
    left: 18px;
    bottom: 18px;
    font-size: 17px;
  }

  .lightbox {
    padding: 45px 12px;
  }

  .lightbox-image {
    max-height: 70vh;
  }
}
```
</style>
</head>
<body>
<header class="topbar">
  <a class="brand" href="#home" aria-label="Mehdi Fatahiye home">
    <svg class="brand-mark" viewBox="0 0 100 100" role="img" aria-label="Architect logo">
      <path d="M12 12 H86 V70 H37 L18 91 L27 70 H12 Z" fill="none" stroke="#405b31" stroke-width="7" stroke-linejoin="miter"/>
      <path d="M28 70 L52 42" fill="none" stroke="#405b31" stroke-width="7"/>
    </svg>
    <div><div class="brand-name">MEHDI FATAHIYE</div><div class="brand-subtitle">ARCHITECT</div></div>
  </a>
  <nav class="navigation" aria-label="Main navigation">
    <a class="nav-link" href="#home" data-en="HOME" data-fa="خانه">HOME</a>
    <a class="nav-link" href="#projects" data-en="PROJECTS" data-fa="پروژه‌ها">PROJECTS</a>
    <a class="nav-link" href="#services" data-en="SERVICES" data-fa="خدمات">SERVICES</a>
    <a class="nav-link" href="#about" data-en="ABOUT" data-fa="درباره من">ABOUT</a>
    <a class="nav-link" href="#contact" data-en="CONTACT" data-fa="تماس">CONTACT</a>
    <span class="language"><button type="button" class="active" data-lang="en">EN</button> | <button type="button" data-lang="fa">FA</button></span>
  </nav>
</header>

<main>
<section class="hero" id="home">
  <div class="hero-copy">
    <h1>Mehdi<br>Fatahiye</h1>
    <p class="role" data-en="ARCHITECT" data-fa="معمار">ARCHITECT</p>
    <div class="small-line"></div>
    <p class="tagline" data-en="From idea to reality.<br>Spaces for a better life." data-fa="از ایده تا واقعیت.<br>فضاهایی برای زندگی بهتر.">From idea to reality.<br>Spaces for a better life.</p>
    <a class="scroll-link" href="#projects"><span class="scroll-arrow">↓</span><span data-en="SCROLL<br>TO EXPLORE" data-fa="برای دیدن<br>پروژه‌ها پایین بروید">SCROLL<br>TO EXPLORE</span></a>
  </div>
  <div class="hero-art" aria-label="Minimalist interior architectural sketch">
    <svg viewBox="0 0 900 650" role="img" aria-label="Hand-drawn sketch of a minimalist living room">
      <g class="sketch-light">
        <path d="M65 190 L435 35 L855 105"/><path d="M65 190 L65 470 L435 610"/><path d="M65 190 L435 260 L855 105"/>
        <path d="M120 168 L435 80 L810 125"/><path d="M190 145 L435 118 L780 145"/><path d="M270 118 L435 155 L735 165"/>
        <path d="M435 35 L435 610"/><path d="M530 50 L530 580"/><path d="M650 72 L650 540"/><path d="M755 90 L755 485"/>
      </g>
      <g class="sketch-dark"><path d="M95 185 L95 450"/><path d="M265 145 L265 515"/><path d="M95 185 L265 145"/><path d="M95 450 L265 515"/><path d="M185 164 L185 480"/><path d="M95 310 L265 290"/></g>
      <g class="sketch-line">
        <path d="M265 145 L600 170 L600 360"/><path d="M265 515 L600 455"/><path d="M340 240 L570 250 L570 345"/><path d="M340 240 L340 355 L570 345"/><path d="M340 355 L410 370 L570 345"/><path d="M355 270 L555 275"/><path d="M355 300 L555 305"/><path d="M375 325 L540 330"/><path d="M365 355 L365 405"/><path d="M550 345 L550 390"/><path d="M340 405 L550 390"/>
      </g>
      <g class="sketch-dark"><path d="M330 390 L500 400 L585 375 L420 365 Z"/><path d="M350 395 L350 430"/><path d="M480 402 L480 430"/><path d="M565 380 L565 410"/><path d="M350 430 L480 430 L565 410"/></g>
      <g class="sketch-line"><path d="M460 135 L460 205"/><path d="M425 205 L495 205"/><path d="M435 210 L485 210"/></g>
      <g class="sketch-line"><path d="M515 385 L800 350 L855 390 L855 475 L570 525 L515 485 Z"/><path d="M515 385 L570 425 L855 390"/><path d="M570 425 L570 525"/><path d="M665 413 L665 508"/><path d="M765 400 L765 490"/><path d="M530 405 L555 435"/><path d="M580 430 L645 420"/><path d="M680 415 L745 405"/><path d="M785 402 L835 395"/><path d="M570 525 L570 545"/><path d="M830 480 L830 500"/></g>
      <g class="sketch-dark"><path d="M450 475 L610 455 L710 485 L550 510 Z"/><path d="M470 480 L470 510"/><path d="M680 485 L680 505"/></g>
      <g class="sketch-light"><path d="M230 490 L550 545 L855 490"/><path d="M170 520 L550 590 L880 520"/><path d="M110 550 L550 630 L890 550"/><path d="M300 490 L250 590"/><path d="M390 505 L365 610"/><path d="M490 520 L480 620"/><path d="M590 520 L610 610"/><path d="M700 505 L750 585"/><path d="M800 490 L850 555"/></g>
      <g class="sketch-line"><path d="M145 430 L150 310 L130 275"/><path d="M150 350 L180 300"/><path d="M150 380 L115 340"/><path d="M130 275 Q95 250 110 230 Q140 220 145 260"/><path d="M145 260 Q165 215 190 240 Q195 265 160 280"/><path d="M130 310 Q95 285 85 305 Q90 330 135 330"/><path d="M180 300 Q205 275 220 295 Q215 320 165 330"/><path d="M120 430 L180 440 L195 420 L135 410 Z"/></g>
      <g class="sketch-light"><path d="M35 200 L430 18 L875 90"/><path d="M40 465 L435 625 L885 535"/><path d="M250 135 L610 155 L860 90"/><path d="M95 185 L280 125"/><path d="M270 145 L615 175"/><path d="M445 255 L850 170"/><path d="M450 260 L865 115"/><path d="M505 480 L805 450"/></g>
    </svg>
  </div>
</section>

<section class="section" id="projects">
  <div class="section-heading">
    <div><div class="section-label" data-en="SELECTED WORK" data-fa="نمونه کارها">SELECTED WORK</div><h2 data-en="Projects" data-fa="پروژه‌ها">Projects</h2></div>
    <p class="intro" data-en="A selection of architectural and interior projects, from concept to completion." data-fa="گزیده‌ای از پروژه‌های معماری و طراحی داخلی؛ از ایده‌پردازی تا اجرا.">A selection of architectural and interior projects, from concept to completion.</p>
  </div>
  <div class="project-grid">
    <article class="project-card" role="button" tabindex="0" data-gallery="atisaz" aria-label="Open Atisaz project gallery">
      <div class="project-visual"><img src="https://raw.githubusercontent.com/mehdifatahiye-hsm/mehdifatahiye-website/main/images/atisaz/1.jpg" alt="Atisaz architectural project" loading="lazy" onerror="this.style.display='none';this.nextElementSibling.style.display='block'"><span class="visual-mark" style="display:none">ATISAZ</span></div>
      <div class="project-info"><span class="project-number">01 / RESIDENTIAL</span><h3 data-en="Atisaz" data-fa="آتی‌ساز">Atisaz</h3><p data-en="Residential architecture and interior project." data-fa="پروژه معماری مسکونی و طراحی داخلی.">Residential architecture and interior project.</p></div>
    </article>
    <article class="project-card" role="button" tabindex="0" data-gallery="ekbatan" aria-label="Open Ekbatan project gallery">
      <div class="project-visual"><img src="https://raw.githubusercontent.com/mehdifatahiye-hsm/mehdifatahiye-website/main/images/ekbatan/Ekbatan%20(1).jpg" alt="Ekbatan architectural project" loading="lazy" onerror="this.style.display='none';this.nextElementSibling.style.display='block'"><span class="visual-mark" style="display:none">EKBATAN</span></div>
      <div class="project-info"><span class="project-number">02 / RESIDENTIAL</span><h3 data-en="Ekbatan" data-fa="اکباتان">Ekbatan</h3><p data-en="A residential project with a focus on practical planning." data-fa="پروژه مسکونی با تمرکز بر برنامه‌ریزی کاربردی فضا.">A residential project with a focus on practical planning.</p></div>
    </article>
    <article class="project-card" role="button" tabindex="0" data-gallery="parkway" aria-label="Open Parkway project gallery">
      <div class="project-visual"><img src="https://raw.githubusercontent.com/mehdifatahiye-hsm/mehdifatahiye-website/main/images/parkway/Parkway%20(1).jpg" alt="Parkway architectural project" loading="lazy" onerror="this.style.display='none';this.nextElementSibling.style.display='block'"><span class="visual-mark" style="display:none">PARKWAY</span></div>
      <div class="project-info"><span class="project-number">03 / INTERIORS</span><h3 data-en="Parkway" data-fa="پارک‌وی">Parkway</h3><p data-en="Interior architecture and carefully coordinated details." data-fa="معماری داخلی و هماهنگی دقیق جزئیات اجرایی.">Interior architecture and carefully coordinated details.</p></div>
    </article>
    <article class="project-card" role="button" tabindex="0" data-gallery="ava" aria-label="Open Ava General project gallery">
      <div class="project-visual"><img src="https://raw.githubusercontent.com/mehdifatahiye-hsm/mehdifatahiye-website/main/images/avageneral/Avageneral%20(1).jpg" alt="Ava General project" loading="lazy" onerror="this.style.display='none';this.nextElementSibling.style.display='block'"><span class="visual-mark" style="display:none">AVA GENERAL</span></div>
      <div class="project-info"><span class="project-number">04 / COMMERCIAL</span><h3 data-en="Ava General" data-fa="آوا جنرال">Ava General</h3><p data-en="Commercial project focused on function and user experience." data-fa="پروژه تجاری با تمرکز بر عملکرد و تجربه کاربران.">Commercial project focused on function and user experience.</p></div>
    </article>
    <article class="project-card" role="button" tabindex="0" data-gallery="daroos" aria-label="Open Daroos project gallery">
      <div class="project-visual"><img src="https://raw.githubusercontent.com/mehdifatahiye-hsm/mehdifatahiye-website/main/images/daroos/IMG_5858.jpg" alt="Daroos residential project" loading="lazy" onerror="this.style.display='none';this.nextElementSibling.style.display='block'"><span class="visual-mark" style="display:none">DAROOS</span></div>
      <div class="project-info"><span class="project-number">05 / RESIDENTIAL</span><h3 data-en="Daroos" data-fa="دروس">Daroos</h3><p data-en="Residential design and renovation work." data-fa="طراحی مسکونی و عملیات بازسازی.">Residential design and renovation work.</p></div>
    </article>
  </div>
</section>

<section class="section" id="about">
  <div class="about-layout">
    <div><div class="section-label" data-en="ABOUT" data-fa="درباره من">ABOUT</div><h2 data-en="Mehdi Fatahiye" data-fa="مهدی فتاحیه">Mehdi Fatahiye</h2></div>
    <div class="about-copy">
      <p data-en="I am a licensed architect and independent project consultant with 20 years of experience across architecture, interior design, renovation and construction management." data-fa="من معمار دارای پروانه و مشاور مستقل پروژه با ۲۰ سال تجربه در معماری، طراحی داخلی، بازسازی و مدیریت ساخت هستم.">I am a licensed architect and independent project consultant with 20 years of experience across architecture, interior design, renovation and construction management.</p>
      <p data-en="My approach brings design intent and on-site execution together. I value clear geometry, natural light, considered materials and practical decisions that make spaces work better." data-fa="رویکرد من پیوند دادن ایده طراحی با اجرای دقیق در محل است. به هندسه روشن، نور طبیعی، متریال سنجیده و تصمیم‌های کاربردی برای بهتر شدن فضا اهمیت می‌دهم.">My approach brings design intent and on-site execution together. I value clear geometry, natural light, considered materials and practical decisions that make spaces work better.</p>
      <div class="facts">
        <div class="fact"><span data-en="Experience" data-fa="سابقه">Experience</span><span data-en="20 years" data-fa="۲۰ سال">20 years</span></div>
        <div class="fact"><span data-en="Focus" data-fa="حوزه فعالیت">Focus</span><span data-en="Architecture · Interiors · Execution" data-fa="معماری · طراحی داخلی · اجرا">Architecture · Interiors · Execution</span></div>
        <div class="fact"><span data-en="Working style" data-fa="شیوه همکاری">Working style</span><span data-en="Independent project consultant" data-fa="مشاور مستقل پروژه">Independent project consultant</span></div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="services">
  <div class="section-heading">
    <div><div class="section-label" data-en="WHAT I DO" data-fa="خدمات">WHAT I DO</div><h2 data-en="Design. Build. Manage." data-fa="طراحی، اجرا، مدیریت">Design. Build. Manage.</h2></div>
    <p class="intro" data-en="Support throughout the project lifecycle, from the first idea to the finished space." data-fa="همراهی در تمام مراحل پروژه؛ از ایده اولیه تا فضای آماده بهره‌برداری.">Support throughout the project lifecycle, from the first idea to the finished space.</p>
  </div>
  <div class="service-grid">
    <article class="service"><span class="service-index">01</span><h3 data-en="Architectural Design" data-fa="طراحی معماری">Architectural Design</h3><p data-en="Concept development, spatial planning and architectural solutions tailored to the brief." data-fa="توسعه ایده، برنامه‌ریزی فضایی و ارائه راهکارهای معماری متناسب با نیاز پروژه.">Concept development, spatial planning and architectural solutions tailored to the brief.</p></article>
    <article class="service"><span class="service-index">02</span><h3 data-en="Interior Design" data-fa="طراحی داخلی">Interior Design</h3><p data-en="Interior layouts, material selection, lighting and detail coordination." data-fa="طراحی چیدمان داخلی، انتخاب متریال، نورپردازی و هماهنگی جزئیات اجرایی.">Interior layouts, material selection, lighting and detail coordination.</p></article>
    <article class="service"><span class="service-index">03</span><h3 data-en="Renovation & Execution" data-fa="بازسازی و اجرا">Renovation & Execution</h3><p data-en="Planning, site coordination, cost awareness, quality checks and construction management." data-fa="برنامه‌ریزی، هماهنگی کارگاه، کنترل هزینه، بررسی کیفیت و مدیریت عملیات اجرایی.">Planning, site coordination, cost awareness, quality checks and construction management.</p></article>
  </div>
</section>

<section class="section" id="contact">
  <div class="contact-panel">
    <div><div class="section-label" data-en="CONTACT" data-fa="تماس">CONTACT</div><h2 data-en="Let’s discuss your project." data-fa="درباره پروژه‌تان گفت‌وگو کنیم.">Let’s discuss your project.</h2><p class="intro" data-en="For selected projects, collaborations and consulting inquiries, get in touch." data-fa="برای پروژه‌های منتخب، همکاری و درخواست مشاوره با من در تماس باشید.">For selected projects, collaborations and consulting inquiries, get in touch.</p></div>
    <div class="contact-details"><div data-en="Email" data-fa="ایمیل">Email</div><a href="mailto:mehdi.fatahiye@outlook.com">mehdi.fatahiye@outlook.com</a></div>
  </div>
</section>
</main>
<div class="lightbox" id="lightbox" role="dialog" aria-modal="true" aria-label="Project photo gallery" onclick="if(event.target===this)closeGallery()">
  <div class="lightbox-content">
    <button class="lightbox-close" type="button" aria-label="Close gallery" onclick="closeGallery()">×</button>
    <button class="lightbox-nav lightbox-prev" type="button" aria-label="Previous image" onclick="changeGalleryImage(-1)">‹</button>
    <img class="lightbox-image" id="lightboxImage" src="" alt="Project photograph">
    <button class="lightbox-nav lightbox-next" type="button" aria-label="Next image" onclick="changeGalleryImage(1)">›</button>
    <div class="lightbox-caption" id="lightboxCaption"></div>
  </div>
</div>
<footer><span>© Mehdi Fatahiye — Architect</span><span data-en="Architecture · Interiors · Construction" data-fa="معماری · طراحی داخلی · اجرا">Architecture · Interiors · Construction</span></footer>
<script>
  const imageBase = 'https://raw.githubusercontent.com/mehdifatahiye-hsm/mehdifatahiye-website/main/';
  const imageUrl = path => imageBase + path.split('/').map(part => encodeURIComponent(part)).join('/');
  const projectGalleries = {
    atisaz: { en: 'Atisaz', fa: 'آتی‌ساز', images: Array.from({length:13}, (_,i) => `images/atisaz/${i+1}.jpg`) },
    ekbatan: { en: 'Ekbatan', fa: 'اکباتان', images: Array.from({length:16}, (_,i) => `images/ekbatan/Ekbatan (${i+1}).jpg`) },
    parkway: { en: 'Parkway', fa: 'پارک‌وی', images: Array.from({length:22}, (_,i) => `images/parkway/Parkway (${i+1}).jpg`) },
    ava: { en: 'Ava General', fa: 'آوا جنرال', images: Array.from({length:26}, (_,i) => `images/avageneral/Avageneral (${i+1}).jpg`) },
    daroos: { en: 'Daroos', fa: 'دروس', images: ['IMG_5858.jpg','IMG_6104.jpg','IMG_6109.jpg','IMG_6179.jpg','IMG_6182.jpg','IMG_6185.jpg','IMG_6207.jpg','IMG_6223.jpg','IMG_6243.jpg','IMG_6268.jpg','IMG_6275.jpg','IMG_6276.jpg','IMG_6282.jpg','IMG_6299.jpg','IMG_6318.jpg','IMG_6324.jpg','IMG_6330.jpg'].map(name => `images/daroos/${name}`) }
  };
  let activeGallery = null, activeImageIndex = 0;
  const lightbox = document.getElementById('lightbox');
  const lightboxImage = document.getElementById('lightboxImage');
  const lightboxCaption = document.getElementById('lightboxCaption');
  function openGallery(key) {
    if (!projectGalleries[key]) return;
    activeGallery = projectGalleries[key]; activeImageIndex = 0;
    lightbox.classList.add('open'); document.body.style.overflow = 'hidden'; showGalleryImage();
  }
  function showGalleryImage() {
    if (!activeGallery) return;
    const total = activeGallery.images.length;
    let attempts = 0;
    const tryImage = () => {
      if (attempts >= total) { lightboxImage.alt = 'Image not found in repository'; lightboxCaption.textContent = (document.documentElement.lang === 'fa' ? 'تصویر در مخزن پیدا نشد' : 'Image not found in repository'); return; }
      const path = imageUrl(activeGallery.images[activeImageIndex]);
      lightboxImage.onerror = () => { attempts++; activeImageIndex = (activeImageIndex + 1) % total; tryImage(); };
      lightboxImage.onload = () => { lightboxCaption.textContent = `${document.documentElement.lang === 'fa' ? activeGallery.fa : activeGallery.en} · ${activeImageIndex+1} / ${total}`; };
      lightboxImage.src = path;
    };
    tryImage();
  }
  function changeGalleryImage(direction) {
    if (!activeGallery) return;
    activeImageIndex = (activeImageIndex + direction + activeGallery.images.length) % activeGallery.images.length;
    showGalleryImage();
  }
  function closeGallery() { lightbox.classList.remove('open'); document.body.style.overflow = ''; activeGallery = null; lightboxImage.src = ''; }
  document.querySelectorAll('[data-gallery]').forEach(card => {
    card.addEventListener('click', () => openGallery(card.dataset.gallery));
    card.addEventListener('keydown', event => { if (event.key === 'Enter' || event.key === ' ') { event.preventDefault(); openGallery(card.dataset.gallery); } });
  });
  document.addEventListener('keydown', event => {
    if (!lightbox.classList.contains('open')) return;
    if (event.key === 'Escape') closeGallery();
    if (event.key === 'ArrowRight') changeGalleryImage(1);
    if (event.key === 'ArrowLeft') changeGalleryImage(-1);
  });
  const langButtons = document.querySelectorAll('[data-lang]');
  function setLanguage(lang) {
    document.documentElement.lang = lang;
    document.documentElement.dir = lang === 'fa' ? 'rtl' : 'ltr';
    langButtons.forEach(button => button.classList.toggle('active', button.dataset.lang === lang));
    document.querySelectorAll('[data-en][data-fa]').forEach(element => {
      element.innerHTML = element.dataset[lang];
    });
    if (activeGallery) showGalleryImage();
    try { localStorage.setItem('portfolio-language', lang); } catch (e) {}
  }
  langButtons.forEach(button => button.addEventListener('click', () => setLanguage(button.dataset.lang)));
  let savedLanguage = 'en';
  try { savedLanguage = localStorage.getItem('portfolio-language') || 'en'; } catch (e) {}
  setLanguage(savedLanguage);
</script>
</body>
</html>
