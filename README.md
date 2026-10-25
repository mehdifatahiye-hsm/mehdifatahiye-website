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
