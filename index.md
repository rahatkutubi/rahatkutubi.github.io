---
layout: default
title: Home
---

<div style="max-width:1200px; margin:0 auto; padding:60px 40px; background:#fff; box-shadow:0 0 40px rgba(0,0,0,0.05); font-family:'Helvetica', Arial, sans-serif; color:#222; line-height:1.65;">

<!-- HEADER -->
<div style="display:flex; justify-content:space-between; align-items:flex-start; border-bottom:1px solid #ddd; padding-bottom:30px; margin-bottom:40px;">
  
  <!-- Left: Bio -->
  <div style="flex:1; padding-right:40px;">
    <h1 style="font-family:Georgia, serif; font-size:38px; color:#800000; margin:0 0 10px 0;">{{ site.author.name }}</h1>
    <div style="font-size:16px; color:#555;">
      <span>{{ site.author.role }}</span>
      <span>{{ site.author.department }}</span>
      <span><a href="{{ site.author.university_url }}">{{ site.author.university }}</a></span>
      <span>📍 {{ site.author.location }}</span>
    </div>

    <p style="margin:15px 0;">
      I am a Ph.D. student at Georgia State University working on
      <strong>Generative AI</strong>, <strong>Vision-Language Models</strong>, and
      <strong>Diffusion-based image editing</strong>. I am advised by
      <a href="#">Dr. Hemanth Venkateswara</a>.
    </p>

    <p>
      My research focuses on instruction-driven image editing, dataset augmentation,
      multi-view generation, and building robust vision-language alignment.
    </p>

    <div style="margin-top:15px;">
      <a href="mailto:{{ site.author.email }}" style="margin-right:15px; font-weight:600; color:#800000; text-transform:uppercase; font-size:14px;">Email</a>
      <a href="https://github.com/{{ site.author.github }}" style="margin-right:15px; font-weight:600; color:#800000; text-transform:uppercase; font-size:14px;">GitHub</a>
      <a href="{{ site.author.scholar }}" style="margin-right:15px; font-weight:600; color:#800000; text-transform:uppercase; font-size:14px;">Scholar</a>
      <a href="assets/rahat_resume.pdf" style="margin-right:15px; font-weight:600; color:#800000; text-transform:uppercase; font-size:14px;">CV</a>
    </div>
  </div>

  <!-- Right: Profile Image -->
  <div style="width:230px; text-align:center;">
    <img src="assets/profile.jpg" alt="{{ site.author.name }}" style="width:220px; height:220px; object-fit:cover; border-radius:4px; box-shadow:0 3px 10px rgba(0,0,0,0.15);">
  </div>
</div>

<!-- NEWS -->
<h2 style="font-family:Georgia, serif; font-size:26px; color:#800000; margin-top:45px; margin-bottom:15px;">News</h2>
<ul>
<li><strong>[Dec 2024]</strong> Paper accepted to <strong>WACV 2025</strong>.</li>
<li><strong>[Aug 2021]</strong> Started Ph.D. at Georgia State University.</li>
</ul>

<!-- PUBLICATIONS -->
<h2 style="font-family:Georgia, serif; font-size:26px; color:#800000; margin-top:45px; margin-bottom:15px;">Selected Publications</h2>

<div style="display:flex; gap:25px; margin-bottom:40px;">
  <div>
    <img src="assets/wacv_teaser.png" alt="WACV Paper" style="width:240px; border-radius:4px; box-shadow:0 2px 6px rgba(0,0,0,0.15);">
  </div>
  <div>
    <h3 style="font-size:18px; font-weight:700; margin-bottom:5px;">Dataset Augmentation by Mixing Visual Concepts</h3>
    <div><strong>Abdullah Al Rahat</strong>, Hemanth Venkateswara</div>
    <div><em>WACV 2025</em></div>
    <p>A concept-mixing based augmentation strategy that improves model robustness and generalization for image classification tasks.</p>
    <a href="https://arxiv.org/abs/2412.15358" style="font-size:13px; margin-right:12px; color:#800000; font-weight:600; text-transform:uppercase;">[arXiv]</a>
    <a href="#" style="font-size:13px; margin-right:12px; color:#800000; font-weight:600; text-transform:uppercase;">[Code]</a>
  </div>
</div>

<div style="display:flex; gap:25px; margin-bottom:40px;">
  <div>
    <img src="https://via.placeholder.com/240x150?text=Secure+Payment" alt="Payment" style="width:240px; border-radius:4px; box-shadow:0 2px 6px rgba(0,0,0,0.15);">
  </div>
  <div>
    <h3 style="font-size:18px; font-weight:700; margin-bottom:5px;">A Simplified Scheme for Secure Offline Electronic Payment Systems</h3>
    <div><strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto</div>
    <div><em>High-Confidence Computing, 2021</em></div>
    <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210" style="font-size:13px; margin-right:12px; color:#800000; font-weight:600; text-transform:uppercase;">[Paper]</a>
  </div>
</div>

</div>
