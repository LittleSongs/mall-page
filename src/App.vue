<template>
  <main class="launch-page">
    <section class="hero" aria-labelledby="page-title">
      <nav class="topbar" aria-label="Main navigation">
        <a class="brand" href="https://itswellbiotech.com" aria-label="Itswell Biotech home">
          <span class="brand-mark">IB</span>
          <span>
            <strong>Itswell Biotech</strong>
            <small>itswellbiotech.com</small>
          </span>
        </a>

        <div class="status-pill">
          <span class="status-dot" aria-hidden="true"></span>
          Preparing for launch
        </div>
      </nav>

      <div class="hero-grid">
        <div class="hero-copy">
          <p class="eyebrow">Product showcase website</p>
          <h1 id="page-title">敬请期待</h1>
          <p class="headline">Itswell Biotech 全新产品展示网站即将上线。</p>
          <p class="intro">
            我们正在完善产品信息、展示体验与服务入口。网站上线后，将在这里呈现更清晰的产品能力、应用场景与品牌资讯。
          </p>

          <div class="actions" aria-label="Launch information">
            <a class="primary-action" href="mailto:contact@itswellbiotech.com">联系团队</a>
            <span class="secondary-note">Coming Soon</span>
          </div>
        </div>

        <div class="showcase" aria-label="Biotech product preview">
          <div class="glass-panel panel-large">
            <span class="panel-label">R&D Pipeline</span>
            <strong>Biotech Solutions</strong>
            <div class="signal-bars" aria-hidden="true">
              <span></span>
              <span></span>
              <span></span>
              <span></span>
            </div>
          </div>

          <div class="orbital-card card-top">
            <span>Quality</span>
            <strong>99.8%</strong>
          </div>

          <div class="orbital-card card-bottom">
            <span>Status</span>
            <strong>Online Soon</strong>
          </div>
        </div>
      </div>

      <footer class="footer">
        <span>© 2026 Itswell Biotech</span>
        <span>Innovating with care, launching soon.</span>
      </footer>
    </section>
  </main>
</template>

<style scoped>
.launch-page {
  min-height: 100vh;
  overflow: hidden;
  color: #10221f;
  background:
    radial-gradient(circle at 18% 18%, rgba(70, 181, 143, 0.3), transparent 28rem),
    radial-gradient(circle at 88% 12%, rgba(79, 124, 201, 0.22), transparent 24rem),
    linear-gradient(135deg, #f7fbf8 0%, #eef7f4 42%, #f8fafc 100%);
}

.hero {
  position: relative;
  display: flex;
  min-height: 100vh;
  width: min(1180px, calc(100% - 40px));
  margin: 0 auto;
  padding: 32px 0 24px;
  flex-direction: column;
}

.hero::before {
  position: absolute;
  inset: 108px auto auto 52%;
  width: 420px;
  height: 420px;
  border: 1px solid rgba(42, 90, 78, 0.16);
  border-radius: 999px;
  background:
    linear-gradient(rgba(29, 92, 78, 0.1), rgba(29, 92, 78, 0.02)),
    repeating-linear-gradient(
      90deg,
      rgba(24, 80, 69, 0.08) 0 1px,
      transparent 1px 32px
    );
  content: '';
  mask-image: radial-gradient(circle, #000 44%, transparent 68%);
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
  gap: 14px;
  color: inherit;
  text-decoration: none;
}

.brand-mark {
  display: grid;
  width: 46px;
  height: 46px;
  place-items: center;
  border-radius: 14px;
  color: #ffffff;
  background: linear-gradient(135deg, #1d8c72, #2457a6);
  box-shadow: 0 14px 34px rgba(29, 99, 91, 0.25);
  font-size: 0.9rem;
  font-weight: 800;
  letter-spacing: 0;
}

.brand strong,
.brand small {
  display: block;
}

.brand strong {
  font-size: 1rem;
  font-weight: 750;
}

.brand small {
  color: #5e716b;
  font-size: 0.78rem;
}

.status-pill {
  display: inline-flex;
  min-height: 40px;
  align-items: center;
  gap: 10px;
  border: 1px solid rgba(20, 79, 66, 0.13);
  border-radius: 999px;
  padding: 8px 16px;
  color: #244840;
  background: rgba(255, 255, 255, 0.66);
  box-shadow: 0 12px 30px rgba(32, 82, 74, 0.08);
  backdrop-filter: blur(16px);
  font-size: 0.86rem;
  font-weight: 650;
}

.status-dot {
  width: 8px;
  height: 8px;
  border-radius: 999px;
  background: #22a17f;
  box-shadow: 0 0 0 6px rgba(34, 161, 127, 0.14);
}

.hero-grid {
  position: relative;
  z-index: 1;
  display: grid;
  flex: 1;
  grid-template-columns: minmax(0, 1.02fr) minmax(320px, 0.78fr);
  align-items: center;
  gap: clamp(36px, 7vw, 92px);
  padding: 68px 0 44px;
}

.hero-copy {
  max-width: 680px;
}

.eyebrow {
  margin-bottom: 18px;
  color: #1a7464;
  font-size: 0.83rem;
  font-weight: 800;
  letter-spacing: 0.16em;
  text-transform: uppercase;
}

h1 {
  color: #10221f;
  font-size: clamp(4.2rem, 12vw, 9.6rem);
  font-weight: 850;
  line-height: 0.95;
}

.headline {
  max-width: 620px;
  margin-top: 28px;
  color: #183d37;
  font-size: clamp(1.45rem, 3vw, 2.35rem);
  font-weight: 720;
  line-height: 1.22;
}

.intro {
  max-width: 610px;
  margin-top: 22px;
  color: #50655f;
  font-size: 1.04rem;
  line-height: 1.9;
}

.actions {
  display: flex;
  align-items: center;
  gap: 18px;
  margin-top: 38px;
  flex-wrap: wrap;
}

.primary-action {
  display: inline-flex;
  min-height: 50px;
  align-items: center;
  justify-content: center;
  border-radius: 999px;
  padding: 0 24px;
  color: #ffffff;
  background: #10221f;
  box-shadow: 0 18px 36px rgba(16, 34, 31, 0.2);
  font-weight: 760;
  text-decoration: none;
}

.secondary-note {
  color: #1c6f60;
  font-size: 0.92rem;
  font-weight: 800;
  letter-spacing: 0.14em;
  text-transform: uppercase;
}

.showcase {
  position: relative;
  display: grid;
  min-height: 520px;
  place-items: center;
}

.glass-panel {
  position: relative;
  overflow: hidden;
  border: 1px solid rgba(255, 255, 255, 0.72);
  border-radius: 28px;
  background:
    linear-gradient(160deg, rgba(255, 255, 255, 0.92), rgba(245, 252, 249, 0.56)),
    linear-gradient(135deg, rgba(37, 133, 112, 0.2), rgba(34, 73, 142, 0.14));
  box-shadow: 0 34px 86px rgba(36, 81, 76, 0.18);
  backdrop-filter: blur(24px);
}

.panel-large {
  display: flex;
  width: min(100%, 430px);
  min-height: 360px;
  padding: 34px;
  flex-direction: column;
  justify-content: space-between;
}

.panel-large::before,
.panel-large::after {
  position: absolute;
  border-radius: 999px;
  content: '';
}

.panel-large::before {
  right: -86px;
  bottom: -70px;
  width: 240px;
  height: 240px;
  background: rgba(35, 142, 114, 0.14);
}

.panel-large::after {
  top: 84px;
  left: 58px;
  width: 126px;
  height: 126px;
  border: 20px solid rgba(36, 87, 166, 0.12);
}

.panel-label {
  position: relative;
  z-index: 1;
  color: #59706a;
  font-size: 0.82rem;
  font-weight: 800;
  letter-spacing: 0.14em;
  text-transform: uppercase;
}

.panel-large strong {
  position: relative;
  z-index: 1;
  max-width: 260px;
  color: #10221f;
  font-size: 2.6rem;
  font-weight: 820;
  line-height: 1.04;
}

.signal-bars {
  position: relative;
  z-index: 1;
  display: grid;
  height: 96px;
  align-items: end;
  grid-template-columns: repeat(4, 1fr);
  gap: 12px;
}

.signal-bars span {
  border-radius: 999px 999px 12px 12px;
  background: linear-gradient(180deg, #2457a6, #22a17f);
  opacity: 0.9;
}

.signal-bars span:nth-child(1) {
  height: 44%;
}

.signal-bars span:nth-child(2) {
  height: 72%;
}

.signal-bars span:nth-child(3) {
  height: 58%;
}

.signal-bars span:nth-child(4) {
  height: 92%;
}

.orbital-card {
  position: absolute;
  display: grid;
  min-width: 148px;
  gap: 6px;
  border: 1px solid rgba(255, 255, 255, 0.7);
  border-radius: 18px;
  padding: 18px 20px;
  background: rgba(255, 255, 255, 0.74);
  box-shadow: 0 24px 54px rgba(27, 80, 72, 0.14);
  backdrop-filter: blur(18px);
}

.orbital-card span {
  color: #687b75;
  font-size: 0.78rem;
  font-weight: 760;
  text-transform: uppercase;
}

.orbital-card strong {
  color: #10221f;
  font-size: 1.15rem;
  font-weight: 820;
}

.card-top {
  top: 70px;
  right: 0;
}

.card-bottom {
  bottom: 72px;
  left: 0;
}

.footer {
  position: relative;
  z-index: 2;
  display: flex;
  justify-content: space-between;
  gap: 18px;
  border-top: 1px solid rgba(31, 82, 73, 0.12);
  padding-top: 20px;
  color: #657a74;
  font-size: 0.88rem;
}

@media (max-width: 820px) {
  .hero {
    width: min(100% - 28px, 640px);
    padding-top: 22px;
  }

  .topbar,
  .footer {
    align-items: flex-start;
    flex-direction: column;
  }

  .hero-grid {
    grid-template-columns: 1fr;
    padding-top: 58px;
  }

  .showcase {
    min-height: 420px;
  }

  .card-top {
    top: 40px;
    right: 4px;
  }

  .card-bottom {
    bottom: 38px;
    left: 4px;
  }
}

@media (max-width: 520px) {
  .status-pill {
    width: 100%;
    justify-content: center;
  }

  .hero-grid {
    gap: 22px;
    padding-bottom: 32px;
  }

  h1 {
    font-size: clamp(3.7rem, 19vw, 5.4rem);
  }

  .intro {
    font-size: 0.98rem;
  }

  .panel-large {
    min-height: 310px;
    padding: 26px;
  }

  .panel-large strong {
    font-size: 2.1rem;
  }

  .orbital-card {
    min-width: 128px;
    padding: 14px 16px;
  }
}
</style>
