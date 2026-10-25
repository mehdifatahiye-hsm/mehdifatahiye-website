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
