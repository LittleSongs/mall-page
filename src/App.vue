<template>
  <main class="launch-page">
    <section class="hero" aria-labelledby="page-title">
      <header class="topbar">
        <a class="brand" href="https://itswellbiotech.com" aria-label="Itswell Biotech home">
          <span class="brand-text">Itswell Biotech</span>
        </a>

        <a class="domain-link" href="https://itswellbiotech.com">itswellbiotech.com</a>
      </header>

      <div class="hero-content">
        <p class="eyebrow">Product showcase website</p>
        <h1 id="page-title">Coming Soon</h1>
        <p class="headline">A new digital home for Itswell Biotech is on the way.</p>
        <p class="intro">
          We are preparing a refined product experience for global partners, customers, and
          collaborators.
        </p>

        <a class="contact-link" href="mailto:sales@itswellbiotech.com">sales@itswellbiotech.com</a>
      </div>

      <div class="visual" aria-hidden="true">
        <span class="ring"></span>
        <span class="core"></span>
      </div>
    </section>
  </main>
</template>

<style scoped>
.launch-page {
  min-height: 100vh;
  color: #10221f;
  background:
    radial-gradient(circle at 74% 42%, rgba(59, 164, 130, 0.18), transparent 25rem),
    radial-gradient(circle at 18% 18%, rgba(103, 194, 163, 0.24), transparent 28rem),
    linear-gradient(135deg, #f7fbf8 0%, #eff8f4 46%, #f8fafc 100%);
}

.hero {
  position: relative;
  display: flex;
  min-height: 100vh;
  width: min(1120px, calc(100% - 40px));
  margin: 0 auto;
  padding: 34px 0;
  flex-direction: column;
  justify-content: space-between;
  overflow: hidden;
}

.topbar {
  position: relative;
  z-index: 2;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 24px;
}

.brand {
  display: inline-flex;
  align-items: center;
  color: inherit;
  text-decoration: none;
}

.brand-text {
  color: #10221f;
  font-family:
    Georgia,
    'Times New Roman',
    Times,
    serif;
  font-size: clamp(1.34rem, 2vw, 1.74rem);
  font-weight: 700;
  letter-spacing: 0.01em;
  line-height: 1;
}

.brand-text::after {
  display: block;
  width: 58%;
  height: 2px;
  margin-top: 8px;
  border-radius: 999px;
  background: linear-gradient(90deg, #1d8c72, rgba(29, 140, 114, 0));
  content: '';
}

.domain-link {
  color: #4f6861;
  font-size: 0.92rem;
  font-weight: 650;
  text-decoration: none;
}

.hero-content {
  position: relative;
  z-index: 2;
  max-width: 760px;
  padding: 96px 0 104px;
}

.eyebrow {
  margin-bottom: 20px;
  color: #1b7867;
  font-size: 0.82rem;
  font-weight: 800;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

h1 {
  max-width: 880px;
  color: #10221f;
  font-size: clamp(4.6rem, 12vw, 9.8rem);
  font-weight: 850;
  line-height: 0.95;
}

.headline {
  max-width: 620px;
  margin-top: 30px;
  color: #173d36;
  font-size: clamp(1.42rem, 3vw, 2.25rem);
  font-weight: 720;
  line-height: 1.22;
}

.intro {
  max-width: 560px;
  margin-top: 20px;
  color: #526961;
  font-size: 1.06rem;
  line-height: 1.8;
}

.contact-link {
  display: inline-flex;
  margin-top: 40px;
  color: #145f52;
  font-size: 1rem;
  font-weight: 760;
  text-decoration-color: rgba(20, 95, 82, 0.24);
  text-underline-offset: 8px;
}

.visual {
  position: absolute;
  right: -90px;
  bottom: 36px;
  width: min(44vw, 520px);
  aspect-ratio: 1;
  opacity: 0.88;
}

.ring,
.core {
  position: absolute;
  border-radius: 999px;
}

.ring {
  inset: 0;
  border: 1px solid rgba(29, 120, 103, 0.16);
  background:
    linear-gradient(rgba(29, 120, 103, 0.06), rgba(29, 120, 103, 0.01)),
    repeating-linear-gradient(
      90deg,
      rgba(24, 88, 74, 0.07) 0 1px,
      transparent 1px 34px
    );
  mask-image: radial-gradient(circle, transparent 37%, #000 38%, #000 61%, transparent 62%);
}

.core {
  inset: 27%;
  background:
    radial-gradient(circle at 34% 28%, rgba(255, 255, 255, 0.9), transparent 34%),
    linear-gradient(135deg, rgba(29, 140, 114, 0.32), rgba(36, 95, 131, 0.18));
  box-shadow:
    0 34px 80px rgba(37, 103, 91, 0.17),
    inset 0 0 0 1px rgba(255, 255, 255, 0.74);
}

@media (max-width: 760px) {
  .hero {
    width: min(100% - 28px, 620px);
    padding: 24px 0 28px;
    justify-content: flex-start;
  }

  .topbar {
    align-items: flex-start;
    flex-direction: column;
    gap: 14px;
  }

  .hero-content {
    padding: 44px 0 58px;
  }

  h1 {
    font-size: clamp(3.8rem, 17vw, 6.6rem);
  }

  .visual {
    right: -140px;
    bottom: 12px;
    width: 430px;
    opacity: 0.36;
  }
}

@media (max-width: 440px) {
  .hero {
    width: min(100% - 24px, 420px);
  }

  .brand-text {
    font-size: 1.28rem;
  }

  .domain-link {
    font-size: 0.86rem;
  }

  .eyebrow {
    margin-bottom: 16px;
    font-size: 0.75rem;
    letter-spacing: 0.13em;
  }

  h1 {
    font-size: clamp(3.42rem, 16vw, 4.3rem);
  }

  .headline {
    font-size: 1.32rem;
  }

  .intro {
    font-size: 0.98rem;
  }

  .contact-link {
    overflow-wrap: anywhere;
  }
}
</style>
