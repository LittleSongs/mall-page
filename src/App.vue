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

    <section class="contact-section" aria-labelledby="contact-title">
      <div class="contact-copy">
        <p class="eyebrow">Contact us</p>
        <h2 id="contact-title">Send us a message</h2>
        <p>
          Leave your contact information and our team will get back to you as soon as possible.
        </p>
      </div>

      <form class="contact-form" action="https://api.web3forms.com/submit" method="POST">
        <input type="hidden" name="access_key" value="eb95beba-a677-4d5b-9bd4-7a562397e2fd" />

        <label>
          <span>Name</span>
          <input type="text" name="name" placeholder="Your name" required />
        </label>

        <label>
          <span>Email</span>
          <input type="email" name="email" placeholder="you@example.com" required />
        </label>

        <label>
          <span>Message</span>
          <textarea name="message" placeholder="Tell us how we can help" required></textarea>
        </label>

        <button type="submit">Submit</button>
      </form>
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

.contact-section {
  position: relative;
  z-index: 2;
  display: grid;
  width: min(1120px, calc(100% - 40px));
  margin: 0 auto;
  padding: 18px 0 78px;
  grid-template-columns: minmax(0, 0.85fr) minmax(320px, 0.9fr);
  gap: clamp(32px, 7vw, 92px);
  align-items: start;
}

.contact-copy {
  max-width: 440px;
}

.contact-copy h2 {
  color: #10221f;
  font-size: clamp(2rem, 4vw, 3.4rem);
  font-weight: 820;
  line-height: 1.02;
}

.contact-copy p:not(.eyebrow) {
  margin-top: 18px;
  color: #526961;
  font-size: 1rem;
  line-height: 1.8;
}

.contact-form {
  display: grid;
  gap: 16px;
  border: 1px solid rgba(29, 120, 103, 0.14);
  border-radius: 24px;
  padding: clamp(20px, 4vw, 30px);
  background: rgba(255, 255, 255, 0.62);
  box-shadow: 0 30px 70px rgba(37, 103, 91, 0.11);
  backdrop-filter: blur(18px);
}

.contact-form label {
  display: grid;
  gap: 8px;
}

.contact-form span {
  color: #214940;
  font-size: 0.86rem;
  font-weight: 760;
}

.contact-form input,
.contact-form textarea {
  width: 100%;
  border: 1px solid rgba(29, 120, 103, 0.18);
  border-radius: 14px;
  padding: 14px 15px;
  color: #10221f;
  background: rgba(255, 255, 255, 0.82);
  outline: none;
  transition:
    border-color 0.2s ease,
    box-shadow 0.2s ease,
    background 0.2s ease;
}

.contact-form textarea {
  min-height: 132px;
  resize: vertical;
}

.contact-form input::placeholder,
.contact-form textarea::placeholder {
  color: #82948e;
}

.contact-form input:focus,
.contact-form textarea:focus {
  border-color: rgba(29, 140, 114, 0.58);
  background: #ffffff;
  box-shadow: 0 0 0 4px rgba(29, 140, 114, 0.1);
}

.contact-form button {
  min-height: 50px;
  border: 0;
  border-radius: 999px;
  color: #ffffff;
  background: #10221f;
  cursor: pointer;
  font-weight: 780;
  transition:
    transform 0.2s ease,
    box-shadow 0.2s ease,
    background 0.2s ease;
}

.contact-form button:hover {
  background: #145f52;
  box-shadow: 0 18px 34px rgba(20, 95, 82, 0.2);
  transform: translateY(-1px);
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

  .contact-section {
    width: min(100% - 28px, 620px);
    padding: 4px 0 54px;
    grid-template-columns: 1fr;
    gap: 24px;
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

  .contact-section {
    width: min(100% - 24px, 420px);
    padding-bottom: 42px;
  }

  .contact-form {
    border-radius: 20px;
  }
}
</style>
