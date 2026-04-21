# Curriculum-Vitae
web 
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Donbosco Silvester Taa — Portfolio</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }
:root { --cream: #F5F0E8; --dark: #1A1A18; --gold: #C9A84C; --gold-light: #E8D5A3; --text-muted: #6B6B62; --border: rgba(201,168,76,0.25); }
body { font-family: "DM Sans", sans-serif; background: var(--cream); color: var(--dark); overflow-x: hidden; }
nav { position: fixed; top: 0; width: 100%; z-index: 100; padding: 18px 48px; display: flex; justify-content: space-between; align-items: center; background: rgba(245,240,232,0.93); backdrop-filter: blur(12px); border-bottom: 1px solid var(--border); }
.nav-logo { font-family: "Playfair Display", serif; font-size: 18px; font-weight: 700; }
.nav-links { display: flex; gap: 32px; list-style: none; }
.nav-links a { text-decoration: none; font-size: 13px; letter-spacing: 1px; text-transform: uppercase; color: var(--text-muted); font-weight: 500; transition: color 0.2s; }
.nav-links a:hover { color: var(--gold); }
.hero { min-height: 100vh; display: grid; grid-template-columns: 1fr 1fr; align-items: center; padding: 100px 48px 60px; gap: 60px; }
.hero-text .eyebrow { font-size: 11px; letter-spacing: 3px; text-transform: uppercase; color: var(--gold); font-weight: 500; margin-bottom: 20px; display: flex; align-items: center; gap: 12px; }
.hero-text .eyebrow::before { content: ""; width: 32px; height: 1px; background: var(--gold); }
.hero-name { font-family: "Playfair Display", serif; font-size: clamp(42px,5vw,64px); font-weight: 900; line-height: 1.05; margin-bottom: 12px; }
.hero-name span { color: var(--gold); }
.hero-title { font-size: 15px; color: var(--text-muted); margin-bottom: 32px; line-height: 1.7; max-width: 460px; }
.hero-tags { display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 40px; }
.tag { padding: 6px 14px; border: 1px solid var(--border); border-radius: 20px; font-size: 12px; color: var(--text-muted); }
.hero-cta { display: flex; gap: 16px; }
.btn-primary { padding: 14px 32px; background: var(--dark); color: var(--cream); font-size: 13px; font-weight: 500; letter-spacing: 1px; text-transform: uppercase; border: none; border-radius: 2px; cursor: pointer; text-decoration: none; display: inline-block; transition: background 0.2s; }
.btn-primary:hover { background: var(--gold); color: var(--dark); }
.btn-outline { padding: 14px 32px; background: transparent; color: var(--dark); font-size: 13px; font-weight: 500; letter-spacing: 1px; text-transform: uppercase; border: 1px solid var(--dark); border-radius: 2px; cursor: pointer; text-decoration: none; display: inline-block; transition: all 0.2s; }
.btn-outline:hover { border-color: var(--gold); color: var(--gold); }
.hero-photo-wrap { display: flex; justify-content: center; align-items: center; }
.photo-frame { position: relative; width: 340px; height: 460px; }
.photo-bg { position: absolute; top: 20px; right: -20px; width: 100%; height: 100%; background: var(--gold-light); border-radius: 4px; }
.photo-img { position: absolute; top: 0; left: -20px; width: 100%; height: 100%; object-fit: cover; object-position: center top; border-radius: 4px; display: block; }
.photo-badge { position: absolute; bottom: -16px; right: -8px; background: var(--dark); color: var(--cream); padding: 14px 18px; border-radius: 4px; text-align: center; z-index: 2; }
.photo-badge .num { font-family: "Playfair Display", serif; font-size: 26px; font-weight: 900; color: var(--gold); line-height: 1; }
.photo-badge .label { font-size: 9px; letter-spacing: 1.5px; text-transform: uppercase; color: rgba(245,240,232,0.55); margin-top: 4px; }
section { padding: 80px 48px; }
.section-header { display: flex; align-items: center; gap: 16px; margin-bottom: 48px; }
.section-num { font-family: "Playfair Display", serif; font-size: 48px; font-weight: 900; color: var(--gold-light); line-height: 1; }
.section-title { font-family: "Playfair Display", serif; font-size: 28px; font-weight: 700; }
.section-line { flex: 1; height: 1px; background: var(--border); }
.about-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: start; }
.about-lead { font-family: "Playfair Display", serif; font-size: 19px; font-weight: 400; line-height: 1.6; margin-bottom: 20px; }
.about-body { font-size: 14px; line-height: 1.8; color: var(--text-muted); }
.stats-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
.stat-card { padding: 24px; border: 1px solid var(--border); border-radius: 4px; }
.stat-num { font-family: "Playfair Display", serif; font-size: 36px; font-weight: 900; color: var(--gold); line-height: 1; }
.stat-label { font-size: 11px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px; margin-top: 6px; }
.lang-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 28px; }
.lang-card { display: flex; justify-content: space-between; align-items: center; padding: 14px 18px; border: 1px solid var(--border); border-radius: 4px; }
.lang-name { font-size: 13px; font-weight: 500; }
.lang-level { font-size: 11px; color: var(--gold); background: rgba(201,168,76,0.1); padding: 3px 10px; border-radius: 10px; }
.award-card { padding: 18px 22px; border: 1px solid var(--border); border-radius: 4px; margin-top: 14px; display: flex; align-items: center; gap: 14px; }
.award-text .atitle { font-size: 13px; font-weight: 500; }
.award-text .ayear { font-size: 11px; color: var(--text-muted); margin-top: 2px; }
.exp-bg { background: var(--dark); }
.exp-bg .section-title { color: var(--cream); }
.exp-bg .section-num { color: rgba(201,168,76,0.3); }
.exp-bg .section-line { background: rgba(201,168,76,0.2); }
.exp-list { display: grid; gap: 2px; }
.exp-item { border: 1px solid rgba(201,168,76,0.15); border-radius: 4px; overflow: hidden; }
.exp-header { padding: 22px 28px; display: flex; justify-content: space-between; align-items: center; cursor: pointer; transition: background 0.2s; }
.exp-header:hover { background: rgba(201,168,76,0.08); }
.exp-left .exp-role { font-family: "Playfair Display", serif; font-size: 17px; font-weight: 700; color: var(--cream); }
.exp-left .exp-company { font-size: 12px; color: var(--gold); font-weight: 500; margin-top: 4px; }
.exp-right { text-align: right; flex-shrink: 0; margin-left: 16px; }
.exp-period { font-size: 11px; color: rgba(245,240,232,0.4); letter-spacing: 1px; text-transform: uppercase; }
.exp-type { font-size: 10px; background: rgba(201,168,76,0.15); color: var(--gold); padding: 3px 10px; border-radius: 10px; margin-top: 5px; display: inline-block; }
.exp-body { padding: 0 28px; max-height: 0; overflow: hidden; transition: max-height 0.35s ease, padding 0.2s; }
.exp-body.open { max-height: 400px; padding: 0 28px 24px; }
.exp-points { list-style: none; }
.exp-points li { font-size: 13px; color: rgba(245,240,232,0.65); line-height: 1.7; padding: 5px 0 5px 16px; position: relative; }
.exp-points li::before { content: "—"; position: absolute; left: 0; color: var(--gold); }
.chevron { width: 18px; height: 18px; color: var(--gold); transition: transform 0.3s; flex-shrink: 0; margin-left: 12px; }
.chevron.open { transform: rotate(180deg); }
.skills-grid { display: grid; grid-template-columns: repeat(3,1fr); gap: 20px; }
.skill-card { padding: 24px; border: 1px solid var(--border); border-radius: 4px; transition: border-color 0.2s; }
.skill-card:hover { border-color: var(--gold); }
.skill-icon { width: 36px; height: 36px; background: var(--gold-light); border-radius: 4px; display: flex; align-items: center; justify-content: center; margin-bottom: 14px; }
.skill-icon svg { width: 18px; height: 18px; }
.skill-card-title { font-family: "Playfair Display", serif; font-size: 15px; font-weight: 700; margin-bottom: 10px; }
.skill-tags { display: flex; flex-wrap: wrap; gap: 5px; }
.skill-tag { padding: 3px 9px; background: rgba(201,168,76,0.1); border-radius: 2px; font-size: 11px; color: var(--text-muted); }
.edu-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
.edu-card { padding: 28px; border: 1px solid var(--border); border-radius: 4px; position: relative; overflow: hidden; }
.edu-card::before { content: ""; position: absolute; top: 0; left: 0; width: 4px; height: 100%; background: var(--gold); }
.edu-degree { font-family: "Playfair Display", serif; font-size: 17px; font-weight: 700; margin-bottom: 8px; }
.edu-school { font-size: 13px; color: var(--gold); font-weight: 500; margin-bottom: 4px; }
.edu-year { font-size: 11px; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px; }
.edu-gpa { margin-top: 14px; display: inline-flex; align-items: center; gap: 8px; background: rgba(201,168,76,0.1); padding: 5px 12px; border-radius: 2px; }
.edu-gpa span { font-size: 11px; color: var(--text-muted); }
.edu-gpa strong { font-size: 13px; color: var(--gold); }
.contact-bg { background: var(--dark); }
.contact-bg .section-title { color: var(--cream); }
.contact-bg .section-num { color: rgba(201,168,76,0.3); }
.contact-bg .section-line { background: rgba(201,168,76,0.2); }
.contact-inner { display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: center; }
.contact-lead { font-family: "Playfair Display", serif; font-size: 21px; color: var(--cream); line-height: 1.5; }
.contact-sub { font-size: 13px; color: rgba(245,240,232,0.5); margin-top: 14px; line-height: 1.7; }
.contact-list { list-style: none; display: flex; flex-direction: column; gap: 14px; }
.contact-item { display: flex; align-items: center; gap: 14px; }
.contact-icon { width: 38px; height: 38px; border: 1px solid rgba(201,168,76,0.3); border-radius: 4px; display: flex; align-items: center; justify-content: center; flex-shrink: 0; }
.contact-icon svg { width: 17px; height: 17px; stroke: var(--gold); }
.contact-detail .clabel { font-size: 10px; color: rgba(245,240,232,0.35); text-transform: uppercase; letter-spacing: 1px; }
.contact-detail .cval { font-size: 13px; color: var(--cream); margin-top: 2px; }
.contact-detail a { color: var(--gold); text-decoration: none; }
footer { background: var(--dark); border-top: 1px solid rgba(201,168,76,0.15); padding: 22px 48px; display: flex; justify-content: space-between; align-items: center; }
.footer-copy { font-size: 11px; color: rgba(245,240,232,0.3); }
.footer-logo { font-family: "Playfair Display", serif; font-size: 15px; color: var(--gold); }
@media (max-width: 900px) {
  .hero { grid-template-columns: 1fr; padding: 80px 24px 40px; }
  .hero-photo-wrap { display: none; }
  section { padding: 60px 24px; }
  nav { padding: 16px 24px; }
  .about-grid, .contact-inner, .edu-grid { grid-template-columns: 1fr; }
  .skills-grid { grid-template-columns: 1fr 1fr; }
}
</style>
</head>
<body>
<nav>
  <div class="nav-logo">D. S. Taa</div>
  <ul class="nav-links">
    <li><a href="#about">Profil</a></li>
    <li><a href="#experience">Pengalaman</a></li>
    <li><a href="#skills">Keahlian</a></li>
    <li><a href="#contact">Kontak</a></li>
  </ul>
</nav>

<section class="hero" id="home">
  <div class="hero-text">
    <div class="eyebrow">Portfolio Profesional</div>
    <h1 class="hero-name">Donbosco<br><span>Silvester</span> Taa</h1>
    <p class="hero-title">Lulusan Bisnis Internasional Universitas Padjadjaran dengan pengalaman di bidang digital marketing, ekspor-impor, dan analisis bisnis. Siap membawa kontribusi nyata bagi perusahaan Anda.</p>
    <div class="hero-tags">
      <span class="tag">Digital Marketing</span>
      <span class="tag">Ekspor-Impor</span>
      <span class="tag">Analisis Bisnis</span>
      <span class="tag">SEO &amp; Ads</span>
      <span class="tag">Bisnis Internasional</span>
    </div>
    <div class="hero-cta">
      <a href="#experience" class="btn-primary">Lihat Pengalaman</a>
      <a href="#contact" class="btn-outline">Hubungi Saya</a>
    </div>
  </div>
  <div class="hero-photo-wrap">
    <div class="photo-frame">
      <div class="photo-bg"></div>
      <img class="photo-img" src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAYEBAUEBAYFBQUGBgYHCQ4JCQgICRINDQoOFRIWFhUSFBQXGiEcFxgfGRQUHScdHyIjJSUlFhwpLCgkKyEkJST/2wBDAQYGBgkICREJCREkGBQYJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCQkJCT/wAARCAGQAlgDASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDu6aRTj0pprnEFJS0CkMBTgKTFOFMBcUhFKelJQAop4FNAp4oAMUMccClNRk80CAcmlxSiloGNxRS4oxQAmKcBRiloABTgKQU8CgAApwFAFOoEJil7UtIaYBjFO7UlLQAYpe1ApDQAooxQKKAENNp56U3FAABS0oFBoAa3AoFB5pR0oGKKcKBS0CCjFLS4oABS0YooAKUUUUwCilooAKKWigAApaKWkAUYoooAKWilFMAoxRS0AJRS0lACUGlpKQCUtFFACUUtGKAEopaSgAxSUtFACUUtFADaKWigBtFLRQA2ilNFAGLTT1pxpvepAKcBSCnCgYlOFJ3pRTAWgCigUAKKeBikAoNAAxpg5NKaAKAHAUtAooEGKMUUUDDFFAp2KAAU8U1RUgFACgUGgUvegQAUUUUwCnAUgpaAFPSkpTSUAKOaKAKKAENAFKetAoAO1IaWg0AMFOFJThSGOFFAo70wFpRSCnAUAKBSkUCg0CEFLQKKYAKMUUtABS0UUAGKWgUtAAKKKKQBSiiloAKKKKYBRRRQAlFFFIAopaSgApKWigBKKWkoADSUtGKAEopaSgBKKWigBKSlooAQ0UGigDEPSm06mipAcKWkFOFMYlLjiilFACc0qilpQKAFFITSnimZyaBCmlFJSigY6jvS0negQtFApaAEFOxQKUUDFAp4popwoELiilFJ3oAUUlKKKAFFLSUUwA0UtJQA6igUtACUlKaKAEooooASlFJThQAopaSloAWnCkApyigBaDS000AFLRRQAUdqSloAWk70UCgBwpaQUo6UAFLRS4oAKBRRigAopaSmAUUtJSAKKKMUAFFFFABSYpaKAEooooASilxRQAlJS0lABRRRQAlFFBoASilooAw80nelxSYqRiinU0U6gBKUUClApiFFOFNoBoAG9KB0pSO4pKAFpRTRxTs0ALRQKKAHCiiigBwpaQU4igAFOFNFOoAcKSgHFB60ALQKSg0ALS0i06mAlKKSlFACilpKKADvRQaKAEpTRSUAIKcKSlpAOpabThTAcKUUClFABSUtFAAKWkFBoAKKKSgBaUUlKKAHClFIBThTAMUppcUhpAGKKWigBDRRS0AJRilFFACdqKXFJQAUlLSUAFFLSYoAKKKKAEopaSgBKKKKACkpTSUAJRS0lABRRRQBhmgUMcCkBB6VIx/agUdqSmIXvS9aQU4UAFAo604DigBRTSMGnCg0AMpaKBQAtAPNFAoAfQKTPFOFADhSmkFOoAMUopKWgBaQ0vekNAB2paQdKKAHLTxTB1pwoASgUppBQA7tRSZpRTAMUlLRSAKKSigA70tJSigBwpy00U5aAHClFJS0wCiiigApaKKACkoooABSiilFADhS02njpQAoopKKAFopKM8UAApaQdKUUAFFFFABSUtJQAUUUUAFFFFACUUUUAFIaWkoAQ0UtJQAUlLSYoAKSlooAaaKWigDDIpoGDTjwKZnmpGPzSim5JpwoELThTaUUwHClrDuPGmg21y1s2oI8q8MI1ZwD6ZAxmprLxVo19ci2gv4zMRwjgoT9MgZpXRXLK17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" alt="Donbosco Silvester Taa">
      <div class="photo-badge">
        <div class="num">3.51</div>
        <div class="label">IPK UNPAD</div>
      </div>
    </div>
  </div>
</section>

<section id="about">
  <div class="section-header">
    <div class="section-num">01</div>
    <h2 class="section-title">Profil Saya</h2>
    <div class="section-line"></div>
  </div>
  <div class="about-grid">
    <div>
      <p class="about-lead">"Profesional muda yang menggabungkan pemahaman bisnis internasional dengan kemampuan eksekusi digital yang kuat."</p>
      <p class="about-body">Sarjana Terapan (D4) Bisnis Internasional dari Universitas Padjadjaran (IPK 3.51/4.00) dengan rekam jejak melalui dua pengalaman magang — konsultasi ekspor di FTA Center Kementerian Perdagangan dan digital marketing di startup edukasi Satukelas.id. Memiliki kemampuan lintas fungsi: dari perencanaan strategi ekspor-impor, kampanye iklan digital (Meta Ads & Google Ads), analisis pasar, hingga pembuatan konten kreatif.</p>
      <div class="lang-grid">
        <div class="lang-card"><span class="lang-name">Bahasa Indonesia</span><span class="lang-level">Pembicara Asli</span></div>
        <div class="lang-card"><span class="lang-name">Bahasa Inggris</span><span class="lang-level">Advanced</span></div>
      </div>
      <div class="award-card">
        <div style="font-size:22px">&#127891;</div>
        <div class="award-text">
          <div class="atitle">Beasiswa Afirmasi/ADik — Pemerintah Pusat &amp; Kab. Nabire</div>
          <div class="ayear">2020 – Sekarang</div>
        </div>
      </div>
    </div>
    <div class="stats-grid">
      <div class="stat-card"><div class="stat-num">2</div><div class="stat-label">Pengalaman Magang</div></div>
      <div class="stat-card"><div class="stat-num">4+</div><div class="stat-label">Tahun Aktif Organisasi</div></div>
      <div class="stat-card"><div class="stat-num">1K+</div><div class="stat-label">Data Klien Dikelola</div></div>
      <div class="stat-card"><div class="stat-num">45+</div><div class="stat-label">Konten Sosmed Dibuat</div></div>
    </div>
  </div>
</section>

<section id="experience" class="exp-bg">
  <div class="section-header">
    <div class="section-num">02</div>
    <h2 class="section-title">Pengalaman</h2>
    <div class="section-line"></div>
  </div>
  <div class="exp-list">
    <div class="exp-item">
      <div class="exp-header" onclick="toggleExp(this)">
        <div class="exp-left"><div class="exp-role">Staf Marketing</div><div class="exp-company">Satukelas.id</div></div>
        <div class="exp-right"><div class="exp-period">Okt 2024 – Jan 2025</div><div class="exp-type">Magang · Digital Marketing</div></div>
        <svg class="chevron" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
      </div>
      <div class="exp-body">
        <ul class="exp-points">
          <li>Menjalankan kampanye iklan berbayar Meta Ads &amp; Google Ads untuk promosi produk Satukelas</li>
          <li>Membuat 45+ konten media sosial (TikTok &amp; Instagram) dengan teknik copywriting IDCA, HSO, dan PAS</li>
          <li>Membangun dan mengoptimalkan website dengan SEO berdasarkan riset Google Trends &amp; Keyword Planner</li>
          <li>Melakukan analisis bisnis: Business Model Canvas, SWOT, Customer Journey, dan analisis kompetitor</li>
          <li>Berhasil merealisasikan minimal satu penjualan produk secara mandiri</li>
        </ul>
      </div>
    </div>
    <div class="exp-item">
      <div class="exp-header" onclick="toggleExp(this)">
        <div class="exp-left"><div class="exp-role">Konsultan Junior</div><div class="exp-company">FTA Center — Kementerian Perdagangan RI</div></div>
        <div class="exp-right"><div class="exp-period">Agu – Des 2023</div><div class="exp-type">Magang · Ekspor-Impor</div></div>
        <svg class="chevron" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
      </div>
      <div class="exp-body">
        <ul class="exp-points">
          <li>Memberikan layanan konsultasi proses ekspor: business matching, sales contract, logistik, dan pembayaran internasional</li>
          <li>Mengelola dan merekap lebih dari 1.000 data konsultasi klien dari tahun 2019–2023</li>
          <li>Menentukan HS Code via insw.go.id dan menganalisis regulasi ekspor-impor via macmap.org</li>
          <li>Analisis pasar ekspor menggunakan trademap.org dan menangani pengisian e-SKA</li>
        </ul>
      </div>
    </div>
    <div class="exp-item">
      <div class="exp-header" onclick="toggleExp(this)">
        <div class="exp-left"><div class="exp-role">Wakil Ketua</div><div class="exp-company">Himpunan Mahasiswa Papua — Universitas Padjadjaran</div></div>
        <div class="exp-right"><div class="exp-period">Feb 2021 – Feb 2022</div><div class="exp-type">Organisasi · Kepemimpinan</div></div>
        <svg class="chevron" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
      </div>
      <div class="exp-body">
        <ul class="exp-points">
          <li>Mendampingi ketua dalam koordinasi kegiatan dan memastikan program kerja berjalan efektif</li>
          <li>Mengelola komunikasi antar anggota mahasiswa Papua di Universitas Padjadjaran</li>
          <li>Berperan aktif dalam perencanaan kegiatan akademik dan sosial serta pengambilan keputusan strategis</li>
        </ul>
      </div>
    </div>
    <div class="exp-item">
      <div class="exp-header" onclick="toggleExp(this)">
        <div class="exp-left"><div class="exp-role">Kepala Divisi Dokumentasi &amp; Dekorasi</div><div class="exp-company">Virtual Porseni Kabim — Universitas Padjadjaran</div></div>
        <div class="exp-right"><div class="exp-period">Okt – Nov 2021</div><div class="exp-type">Kepanitiaan · Event</div></div>
        <svg class="chevron" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
      </div>
      <div class="exp-body">
        <ul class="exp-points">
          <li>Memimpin divisi desain dan dokumentasi: konten sosmed, sertifikat, dan piagam acara</li>
          <li>Memantau dan mendokumentasikan teknis acara virtual melalui Zoom</li>
          <li>Memberikan rekomendasi strategis kepada ketua panitia</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="section-header">
    <div class="section-num">03</div>
    <h2 class="section-title">Keahlian</h2>
    <div class="section-line"></div>
  </div>
  <div class="skills-grid">
    <div class="skill-card">
      <div class="skill-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 12h-4l-3 9L9 3l-3 9H2"/></svg></div>
      <div class="skill-card-title">Digital Marketing</div>
      <div class="skill-tags"><span class="skill-tag">Meta Ads</span><span class="skill-tag">Google Ads</span><span class="skill-tag">TikTok Ads</span><span class="skill-tag">SEO</span><span class="skill-tag">Copywriting</span><span class="skill-tag">Marketing Funnel</span></div>
    </div>
    <div class="skill-card">
      <div class="skill-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg></div>
      <div class="skill-card-title">Ekspor-Impor</div>
      <div class="skill-tags"><span class="skill-tag">LC &amp; Bill of Lading</span><span class="skill-tag">HS Code</span><span class="skill-tag">e-SKA</span><span class="skill-tag">Trademap</span><span class="skill-tag">Macmap</span><span class="skill-tag">PIB &amp; PEB</span></div>
    </div>
    <div class="skill-card">
      <div class="skill-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="3" width="20" height="14" rx="2"/><line x1="8" y1="21" x2="16" y2="21"/><line x1="12" y1="17" x2="12" y2="21"/></svg></div>
      <div class="skill-card-title">Konten &amp; Desain</div>
      <div class="skill-tags"><span class="skill-tag">Canva</span><span class="skill-tag">CapCut</span><span class="skill-tag">Adobe Premiere</span><span class="skill-tag">TikTok Live</span><span class="skill-tag">Color Grading</span></div>
    </div>
    <div class="skill-card">
      <div class="skill-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg></div>
      <div class="skill-card-title">Analisis Bisnis</div>
      <div class="skill-tags"><span class="skill-tag">SWOT</span><span class="skill-tag">BMC</span><span class="skill-tag">Design Thinking</span><span class="skill-tag">Google Analytics</span><span class="skill-tag">Tableau</span><span class="skill-tag">NVivo</span></div>
    </div>
    <div class="skill-card">
      <div class="skill-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/></svg></div>
      <div class="skill-card-title">Produktivitas &amp; Teknis</div>
      <div class="skill-tags"><span class="skill-tag">Ms. Excel</span><span class="skill-tag">Ms. Word</span><span class="skill-tag">Google Suite</span><span class="skill-tag">Wix Builder</span><span class="skill-tag">AI Tools</span></div>
    </div>
    <div class="skill-card">
      <div class="skill-icon"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/></svg></div>
      <div class="skill-card-title">Soft Skills</div>
      <div class="skill-tags"><span class="skill-tag">Presentasi Publik</span><span class="skill-tag">Komunikasi Bisnis</span><span class="skill-tag">Kepemimpinan</span><span class="skill-tag">Problem Solving</span></div>
    </div>
  </div>
</section>

<section id="education">
  <div class="section-header">
    <div class="section-num">04</div>
    <h2 class="section-title">Pendidikan</h2>
    <div class="section-line"></div>
  </div>
  <div class="edu-grid">
    <div class="edu-card">
      <div class="edu-degree">D4 Bisnis Internasional</div>
      <div class="edu-school">Universitas Padjadjaran</div>
      <div class="edu-year">2020 – 2025 · Fakultas Ekonomi dan Bisnis</div>
      <div class="edu-gpa"><span>IPK</span><strong>3.51 / 4.00</strong></div>
      <p style="font-size:13px;color:var(--text-muted);margin-top:14px;line-height:1.6;">Fokus pada perdagangan internasional, manajemen bisnis global, analisis pasar, dan kewirausahaan digital.</p>
    </div>
    <div class="edu-card">
      <div class="edu-degree">Sekolah Menengah Atas</div>
      <div class="edu-school">YPPK Adhi Luhur Kolese LE COCQ D'Armandville</div>
      <div class="edu-year">2017 – 2020</div>
      <p style="font-size:13px;color:var(--text-muted);margin-top:14px;line-height:1.6;">Lulusan dengan fondasi akademik kuat, mendapatkan Beasiswa Afirmasi/ADik untuk melanjutkan ke Universitas Padjadjaran.</p>
    </div>
  </div>
</section>

<section id="contact" class="contact-bg">
  <div class="section-header">
    <div class="section-num">05</div>
    <h2 class="section-title">Kontak</h2>
    <div class="section-line"></div>
  </div>
  <div class="contact-inner">
    <div>
      <p class="contact-lead">Tertarik berkolaborasi atau mendiskusikan peluang karir?</p>
      <p class="contact-sub">Terbuka untuk peluang di bidang digital marketing, bisnis internasional, analisis bisnis, maupun posisi entry-level lainnya.</p>
    </div>
    <ul class="contact-list">
      <li class="contact-item">
        <div class="contact-icon"><svg viewBox="0 0 24 24" fill="none" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.99 12a19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 3.9 1.18h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L8.09 8.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7a2 2 0 0 1 1.72 2.03z"/></svg></div>
        <div class="contact-detail"><div class="clabel">Telepon</div><div class="cval">081388334752</div></div>
      </li>
      <li class="contact-item">
        <div class="contact-icon"><svg viewBox="0 0 24 24" fill="none" stroke-width="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg></div>
        <div class="contact-detail"><div class="clabel">Email</div><div class="cval"><a href="mailto:donboscosilvestertaa@gmail.com">donboscosilvestertaa@gmail.com</a></div></div>
      </li>
      <li class="contact-item">
        <div class="contact-icon"><svg viewBox="0 0 24 24" fill="none" stroke-width="2"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"/><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"/></svg></div>
        <div class="contact-detail"><div class="clabel">Profil Linktree</div><div class="cval"><a href="https://lynk.id/boscotaa" target="_blank">lynk.id/boscotaa</a></div></div>
      </li>
    </ul>
  </div>
</section>

<footer>
  <div class="footer-copy">&copy; 2025 Donbosco Silvester Taa. All rights reserved.</div>
  <div class="footer-logo">D. S. Taa</div>
</footer>

<script>
function toggleExp(header) {
  var body = header.nextElementSibling;
  var chevron = header.querySelector(".chevron");
  var isOpen = body.classList.contains("open");
  document.querySelectorAll(".exp-body.open").forEach(function(b) { b.classList.remove("open"); });
  document.querySelectorAll(".chevron.open").forEach(function(c) { c.classList.remove("open"); });
  if (!isOpen) { body.classList.add("open"); chevron.classList.add("open"); }
}
document.querySelectorAll("a[href^=\"#\"]").forEach(function(a) {
  a.addEventListener("click", function(e) {
    e.preventDefault();
    var t = document.querySelector(a.getAttribute("href"));
    if (t) t.scrollIntoView({ behavior: "smooth" });
  });
});
</script>
</body>
</html>
