---
layout: default
title: Home
---

<style>
/* ---------------------------------------
   STANFORD CS STYLE GLOBAL SETTINGS
--------------------------------------- */
body {
    font-family: "Helvetica", "Arial", sans-serif;
    font-size: 17px;
    line-height: 1.65;
    color: #222;
    margin: 0;
    padding: 0;
    background: #fafafa;
}

.page-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 40px;
    background: #fff;
    box-shadow: 0 0 40px rgba(0,0,0,0.05);
}

/* Typography */
h1 { font-family: Georgia, serif; font-size: 38px; color: #800000; margin: 0 0 10px 0; }
h2 { font-family: Georgia, serif; font-size: 26px; color: #800000; margin-top: 45px; margin-bottom: 15px; }

/* Header */
.header { display: flex; justify-content: space-between; align-items: flex-start; border-bottom: 1px solid #ddd; padding-bottom: 30px; margin-bottom: 40px; }
.header-left { flex: 1; padding-right: 40px; }
.header-meta span { display: block; font-size: 16px; color: #555; margin-bottom: 4px; }
.header p { margin: 15px 0; }
.header-right { width: 230px; text-align: center; }
.profile-img { width: 220px; height: 220px; object-fit: cover; border-radius: 4px; box-shadow: 0 3px 10px rgba(0,0,0,0.15); }

/* Social links */
.social-links { margin-top: 15px; }
.social-links a { margin-right: 15px; font-weight: 600; color: #800000; text-transform: uppercase; font-size: 14px; }
.social-links a:hover { text-decoration: underline; }

/* News */
.news-item { margin-bottom: 10px; }
.news-date { font-family: monospace; font-weight: bold; margin-right: 8px; }

/* Publications */
.pub-item { display: flex; gap: 25px; margin-bottom: 40px; }
.pub-teaser img { width: 240px; border-radius: 4px; box-shadow: 0 2px 6px rgba(0,0,0,0.15); }
.pub-title { font-size: 18px; font-weight: 700; color: #000; margin-bottom: 5px; }
.pub-links a { font-size: 13px; margin-right: 12px; text-transform: uppercase; color: #800000; font-weight: 600; }

/* Responsive */
@media (max-width: 900px) {
    .header { flex-direction: column-reverse; text-align: center; }
    .header-left { padding-right: 0; }
    .header-right { margin-bottom: 25px; width: 100%; }
    .pub-item { flex-direction: column; text-align: center; }
    .pub-teaser img { margin: 0 auto; }
}
</style>

<div class="page-container">

<!-- HEADER -->
<div class="header">
  <div class="header-left">
    <h1>{{ site.author.name }}</h1>
    <div class="header-meta">
      <span>{{ site.author.role }}</span>
      <span>{{ site.author.department }}</span>
      <span><a href="{{ site.author.university_url }}">{{ site.author.university }}</a></span>
      <span>📍 {{ site.author.location }}</span>
    </div>

    <p>
      I am a Ph.D. student at Georgia State University working on
      <strong>Generative AI</strong>, <strong>Vision-Language Models</strong>, and
      <strong>Diffusion-based image editing</strong>. I am advised by
      <a href="#">Dr. Hemanth Venkateswara</a>.
    </p>

    <p>
      My research focuses on instruction-driven image editing, dataset augmentation,
      multi-view generation, and building robust vision-language alignment.
    </p>

    <div class="social-links">
      <a href="mailto:{{ site.author.email }}">Email</a>
      <a href="https://github.com/{{ site.author.github }}">GitHub</a>
      <a href="{{ site.author.scholar }}">Scholar</a>
      <a href="assets/rahat_resume.pdf">CV</a>
    </div>
  </div>

  <div class="header-right">
    <img src="assets/profile.jpg" alt="{{ site.author.name }}" class="profile-img">
  </div>
</div>

<!-- NEWS -->
## News

<div class="news-item">
  <span class="news-date">[Dec 2024]</span>
  Paper accepted to **WACV 2025**.
</div>
<div class="news-item">
  <span class="news-date">[Aug 2021]</span>
  Started Ph.D. at Georgia State University.
</div>

<!-- PUBLICATIONS -->
## Selected Publications

<div class="pub-item">
  <div class="pub-teaser">
    <img src="assets/wacv_teaser.png" alt="WACV Paper">
  </div>
  <div class="pub-details">
    <div class="pub-title">
      Dataset Augmentation by Mixing Visual Concepts
    </div>
    <div><strong>Abdullah Al Rahat</strong>, Hemanth Venkateswara</div>
    <div><em>WACV 2025</em></div>
    <p>
      A concept-mixing based augmentation strategy that improves model robustness
      and generalization for image classification tasks.
    </p>
    <div class="pub-links">
      <a href="https://arxiv.org/abs/2412.15358">[arXiv]</a>
      <a href="#">[Code]</a>
    </div>
  </div>
</div>

<div class="pub-item">
  <div class="pub-teaser">
    <img src="https://via.placeholder.com/240x150?text=Secure+Payment" alt="Payment">
  </div>
  <div class="pub-details">
    <div class="pub-title">
      A Simplified Scheme for Secure Offline Electronic Payment Systems
    </div>
    <div><strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto<
