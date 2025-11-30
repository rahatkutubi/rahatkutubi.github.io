---
layout: default
title: Home
---

<style>
    /* GLOBAL SETTINGS */
    body {
        font-family: 'Segoe UI', Verdana, sans-serif;
        font-size: 15px;
        line-height: 1.6;
        color: #333;
        max-width: 1000px;
        margin: 0 auto;
        padding: 40px 20px;
    }
    a { color: #0066cc; text-decoration: none; }
    a:hover { text-decoration: underline; }

    /* HEADER: LEFT SIDE BIO / RIGHT SIDE PHOTO */
    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: flex-start; /* Aligns content to top */
        margin-bottom: 50px;
        border-bottom: 1px solid #eee;
        padding-bottom: 30px;
    }
    
    /* LEFT SIDE: CONFIG DATA */
    .bio-content {
        width: 70%;
        padding-right: 30px;
    }
    .bio-content h1 {
        font-size: 32px;
        font-weight: 700;
        margin-top: 0;
        margin-bottom: 5px;
        color: #000;
    }
    .bio-meta {
        font-size: 16px;
        color: #555;
        margin-bottom: 20px;
    }
    .bio-meta span {
        display: block; /* Stacks items vertically */
        margin-bottom: 3px;
    }
    
    /* SOCIAL LINKS ROW */
    .social-links {
        margin-top: 15px;
        font-size: 14px;
    }
    .social-links a {
        margin-right: 15px;
        font-weight: 600;
        text-transform: uppercase;
        color: #444;
    }
    .social-links a:hover { color: #0066cc; }

    /* RIGHT SIDE: PHOTO */
    .profile-img-container {
        width: 25%;
        text-align: center;
    }
    .profile-img {
        width: 200px;
        height: 200px;
        object-fit: cover;
        border-radius: 50%; /* Circle shape */
        box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        border: 4px solid #fff;
    }

    /* SECTIONS */
    h2 {
        font-size: 22px;
        font-weight: 700;
        margin-top: 50px;
        margin-bottom: 20px;
        color: #000;
    }

    /* PUBLICATIONS & NEWS (Same as before) */
    .news-item { margin-bottom: 10px; }
    .news-date { font-family: monospace; font-weight: bold; margin-right: 10px; }
    
    .pub-item { display: flex; margin-bottom: 35px; gap: 25px; }
    .pub-teaser { flex: 0 0 220px; max-width: 220px; }
    .pub-teaser img { width: 100%; border-radius: 4px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
    .pub-details { flex: 1; }
    .pub-title { font-weight: 700; font-size: 17px; color: #000; display: block; margin-bottom: 5px;}
    .pub-links a { font-size: 13px; margin-right: 10px; text-transform: uppercase; font-weight: 600; }

    /* MOBILE RESPONSIVENESS */
    @media (max-width: 768px) {
        .header-container { flex-direction: column-reverse; text-align: center; }
        .bio-content { width: 100%; padding: 0; }
        .profile-img-container { width: 100%; margin-bottom: 20px; }
        .pub-item { flex-direction: column; }
        .pub-teaser { width: 100%; max-width: 300px; margin: 0 auto 15px auto; }
    }
</style>

<div class="header-container">
    <div class="bio-content">
        <h1>{{ site.author.name }}</h1>
        
        <div class="bio-meta">
            <span>{{ site.author.role }}</span>
            <span>{{ site.author.department }}</span>
            <span><a href="{{ site.author.university_url }}">{{ site.author.university }}</a></span>
            <span>📍 {{ site.author.location }}</span>
        </div>

        <p>
            I am a Ph.D. student researching <strong>Generative AI</strong>, <strong>Vision-Language Models (VLM)</strong>, and <strong>Diffusion Models</strong>. I am currently advised by <a href="#">Dr. Hemanth Venkateswara</a>.
        </p>
        <p>
            My work focuses on building robust tools for instruction-based image editing and dataset augmentation. Previously, I was a Lecturer at BAUET and received my M.Sc. from Kookmin University.
        </p>

        <div class="social-links">
            <a href="mailto:{{ site.author.email }}">Email</a>
            <a href="https://github.com/{{ site.author.github }}">GitHub</a>
            <a href="{{ site.author.scholar }}">Google Scholar</a>
            <a href="assets/rahat_resume.pdf">CV / Resume</a>
        </div>
    </div>

    <div class="profile-img-container">
        <img src="assets/profile.jpg" alt="{{ site.author.name }}" class="profile-img">
    </div>
</div>

<h2>🔥 News</h2>
<div class="news-item">
    <span class="news-date">[Dec 2024]</span>
    Paper accepted to <strong>WACV 2025</strong>.
</div>
<div class="news-item">
    <span class="news-date">[Aug 2021]</span>
    Started Ph.D. at Georgia State University.
</div>

<h2>📝 Selected Publications</h2>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="assets/wacv_teaser.png" alt="WACV Teaser">
    </div>
    <div class="pub-details">
        <a href="https://arxiv.org/abs/2412.15358" class="pub-title">Dataset Augmentation by Mixing Visual Concepts</a>
        <div><strong>Abdullah Al Rahat</strong>, Hemanth Venkateswara</div>
        <div><em>WACV 2025</em></div>
        <p>We propose a novel method for augmenting datasets by mixing visual concepts to improve model robustness.</p>
        <div class="pub-links">
            <a href="https://arxiv.org/abs/2412.15358">[arXiv]</a>
            <a href="#">[Code]</a>
        </div>
    </div>
</div>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="https://via.placeholder.com/220x140?text=Payment" alt="Secure Payment">
    </div>
    <div class="pub-details">
        <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210" class="pub-title">A Simplified Scheme for Secure Offline Electronic Payment Systems</a>
        <div><strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto</div>
        <div><em>High-Confidence Computing, 2021</em></div>
        <div class="pub-links">
            <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210">[Paper]</a>
        </div>
    </div>
</div>
