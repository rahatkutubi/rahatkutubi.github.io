---
layout: default
title: Home
---

<style>
    /* PAGE BASE */
    body {
        font-family: 'Segoe UI', Verdana, sans-serif;
        font-size: 16px;
        line-height: 1.65;
        color: #333;
        max-width: 900px;
        margin: 0 auto;
        padding: 40px 20px;
    }
    a { color: #0645ad; text-decoration: none; }
    a:hover { text-decoration: underline; }

    /* HEADER LAYOUT */
    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        margin-bottom: 40px;
        padding-bottom: 25px;
        border-bottom: 1px solid #e5e5e5;
    }

    .bio-content {
        width: 70%;
        padding-right: 30px;
    }
    .bio-content h1 {
        font-size: 32px;
        font-weight: 700;
        margin: 0 0 8px 0;
    }
    .bio-meta span {
        display: block;
        font-size: 15px;
        color: #555;
        margin-bottom: 3px;
    }

    .profile-img-container {
        width: 25%;
        text-align: center;
    }
    .profile-img {
        width: 180px;
        height: 180px;
        border-radius: 50%;
        object-fit: cover;
        border: 4px solid #fff;
        box-shadow: 0 4px 12px rgba(0,0,0,0.12);
    }

    /* SOCIAL LINKS */
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
    .social-links a:hover { color: #0645ad; }

    /* SECTION TITLES */
    h2 {
        font-size: 22px;
        font-weight: 700;
        margin-top: 45px;
        margin-bottom: 20px;
    }

    /* NEWS */
    .news-item {
        margin-bottom: 10px;
    }
    .news-date {
        font-family: monospace;
        font-weight: bold;
        margin-right: 10px;
    }

    /* PUBLICATIONS */
    .pub-item {
        display: flex;
        gap: 20px;
        margin-bottom: 35px;
    }
    .pub-teaser {
        flex: 0 0 200px;
        max-width: 200px;
    }
    .pub-teaser img {
        width: 100%;
        border-radius: 5px;
        box-shadow: 0 2px 6px rgba(0,0,0,0.15);
    }
    .pub-details {
        flex: 1;
    }
    .pub-title {
        font-size: 17px;
        font-weight: 700;
        margin-bottom: 5px;
        display: block;
        color: #000;
    }
    .pub-links a {
        font-size: 13px;
        margin-right: 10px;
        text-transform: uppercase;
        font-weight: 600;
    }

    /* RESPONSIVE */
    @media (max-width: 768px) {
        .header-container { flex-direction: column-reverse; text-align: center; }
        .bio-content { width: 100%; padding: 0; }
        .profile-img-container { width: 100%; margin-bottom: 20px; }
        .pub-item { flex-direction: column; }
        .pub-teaser { margin: 0 auto; }
    }
</style>

<!-- HEADER -->
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
            I am a Ph.D. student in Computer Science at Georgia State University. My research focuses on  
            <strong>Generative AI</strong>, <strong>Vision-Language Models</strong>, <strong>Diffusion Models</strong>,  
            and <strong>instruction-based image editing</strong>. I am advised by  
            <a href="#">Dr. Hemanth Venkateswara</a>.
        </p>

        <p>
            My recent work includes dataset creation for fine-grained image editing, multi-view generation,  
            visual grounding, and improving image–language alignment in LLaVA-style models.
        </p>

        <div class="social-links">
            <a href="mailto:{{ site.author.email }}">Email</a>
            <a href="https://github.com/{{ site.author.github }}">GitHub</a>
            <a href="{{ site.author.scholar }}">Scholar</a>
            <a href="assets/rahat_resume.pdf">CV</a>
        </div>
    </div>

    <div class="profile-img-container">
        <img src="assets/profile.jpg" alt="{{ site.author.name }}" class="profile-img">
    </div>
</div>

<!-- NEWS -->
<h2>🔥 News</h2>
<div class="news-item"><span class="news-date">[Dec 2024]</span>Paper accepted to <strong>WACV 2025</strong>.</div>
<div class="news-item"><span class="news-date">[Aug 2021]</span>Started Ph.D. at Georgia State University.</div>

<!-- PUBLICATIONS -->
<h2>📝 Selected Publications</h2>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="assets/wacv_teaser.png" alt="WACV Paper">
    </div>
    <div class="pub-details">
        <a href="https://arxiv.org/abs/2412.15358" class="pub-title">
            Dataset Augmentation by Mixing Visual Concepts
        </a>
        <div><strong>Abdullah Al Rahat</strong>, Hemanth Venkateswara</div>
        <div><em>WACV 2025</em></div>
        <p>A method for augmenting datasets by mixing visual concepts to improve model robustness.</p>
        <div class="pub-links">
            <a href="https://arxiv.org/abs/2412.15358">[arXiv]</a>
            <a href="#">[Code]</a>
        </div>
    </div>
</div>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="https://via.placeholder.com/220x140?text=Payment" alt="Secure Payment Paper">
    </div>
    <div class="pub-details">
        <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210" class="pub-title">
            A Simplified Scheme for Secure Offline Electronic Payment Systems
        </a>
        <div><strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto</div>
        <div><em>High-Confidence Computing, 2021</em></div>
        <div class="pub-links">
            <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210">[Paper]</a>
        </div>
    </div>
</div>
