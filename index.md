---
layout: default
title: Abdullah Al Rahat
---

<style>
    /* GLOBAL FONTS & SETTINGS */
    body {
        font-family: 'Verdana', sans-serif;
        font-size: 15px;
        line-height: 1.6;
        color: #333;
        max-width: 960px;
        margin: 0 auto;
        padding: 40px 20px;
    }
    a { color: #007bff; text-decoration: none; }
    a:hover { text-decoration: underline; }
    strong { color: #000; }

    /* HEADER SECTION */
    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 50px;
    }
    .bio-content {
        width: 70%;
        padding-right: 20px;
    }
    .bio-content h1 {
        font-size: 28px;
        font-weight: 700;
        margin-bottom: 10px;
        color: #000;
    }
    .bio-content p { margin-bottom: 15px; }
    .profile-img-container {
        width: 25%;
        text-align: right;
    }
    .profile-img {
        width: 200px;
        height: 200px;
        object-fit: cover;
        border-radius: 50%;
        box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    .social-links a { margin-right: 15px; font-weight: 500; }

    /* SECTION HEADERS */
    h2 {
        font-size: 20px;
        font-weight: 700;
        border-bottom: 1px solid #eaeaea;
        padding-bottom: 10px;
        margin-top: 50px;
        margin-bottom: 25px;
        color: #000;
    }

    /* NEWS SECTION */
    .news-item { margin-bottom: 8px; }
    .news-date { font-family: 'Courier New', monospace; font-weight: bold; margin-right: 10px; }

    /* PUBLICATION GRID */
    .pub-item {
        display: flex;
        margin-bottom: 40px;
        gap: 25px;
    }
    .pub-teaser {
        flex: 0 0 220px; /* Fixed width for the image */
        max-width: 220px;
    }
    .pub-teaser img {
        width: 100%;
        border-radius: 4px;
        border: 1px solid #f0f0f0;
        box-shadow: 0 2px 4px rgba(0,0,0,0.05);
    }
    .pub-details { flex: 1; }
    .pub-title { font-weight: 700; font-size: 16px; color: #000; display: block; margin-bottom: 5px;}
    .pub-authors { margin-bottom: 5px; color: #555; }
    .pub-venue { font-style: italic; color: #666; margin-bottom: 8px; }
    .pub-desc { font-size: 14px; color: #444; margin-bottom: 10px; }
    .pub-links a {
        font-size: 13px;
        margin-right: 10px;
        text-transform: uppercase;
        font-weight: 600;
    }
    
    /* RESPONSIVE FOR MOBILE */
    @media (max-width: 700px) {
        .header-container { flex-direction: column-reverse; text-align: center; }
        .bio-content { width: 100%; padding: 0; }
        .profile-img-container { width: 100%; margin-bottom: 20px; text-align: center; }
        .pub-item { flex-direction: column; }
        .pub-teaser { max-width: 100%; width: 100%; }
        .pub-teaser img { width: 100%; max-width: 300px; }
    }
</style>

<div class="header-container">
    <div class="bio-content">
        <h1>Abdullah Al Rahat</h1>
        <p>
            I am a Ph.D. [cite_start]Student in Computer Science at <a href="https://www.gsu.edu/">Georgia State University</a>[cite: 6], advised by <a href="#">Dr. Hemanth Venkateswara</a>.
        </p>
        <p>
            [cite_start]My research interests lie in <strong>Generative AI</strong>, <strong>Large Language Models (LLM)</strong>, <strong>Vision-Language Models (VLM)</strong>, and <strong>Diffusion Models</strong>[cite: 4]. [cite_start]I am currently working on instruction-based image editing and dataset augmentation strategies[cite: 56, 57].
        </p>
        <p>
            [cite_start]Previously, I served as a Lecturer at BAUET [cite: 50] [cite_start]and received my M.Sc. in Applied Information Technology from Kookmin University, South Korea[cite: 8, 9].
        </p>
        <div class="social-links">
            <a href="mailto:rahatcse2k9@gmail.com">Email</a>
            <a href="assets/rahat_resume.pdf">CV</a>
            <a href="https://github.com/rahatkutubi">GitHub</a>
            <a href="YOUR_SCHOLAR_LINK">Google Scholar</a>
        </div>
    </div>
    <div class="profile-img-container">
        <img src="assets/profile.jpg" alt="Abdullah Al Rahat" class="profile-img">
    </div>
</div>

<h2>🔥 News</h2>
<div class="news-item">
    <span class="news-date">[Dec 2024]</span>
    [cite_start]Paper accepted to <strong>WACV 2025</strong>[cite: 63].
</div>
<div class="news-item">
    <span class="news-date">[Aug 2021]</span>
    [cite_start]Started Ph.D. at Georgia State University[cite: 10].
</div>

<h2>📝 Selected Publications</h2>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="assets/wacv_teaser.png" alt="WACV Teaser">
    </div>
    <div class="pub-details">
        <a href="https://arxiv.org/abs/2412.15358" class="pub-title">Dataset Augmentation by Mixing Visual Concepts</a>
        <div class="pub-authors">
            [cite_start]<strong>Abdullah Al Rahat</strong>, Hemanth Venkateswara [cite: 63]
        </div>
        <div class="pub-venue">
            IEEE/CVF Winter Conference on Applications of Computer Vision (WACV), 2025
        </div>
        <div class="pub-desc">
            We propose a novel method for augmenting datasets by mixing visual concepts to improve model robustness in low-data regimes.
        </div>
        <div class="pub-links">
            <a href="https://arxiv.org/abs/2412.15358">[arXiv]</a>
            <a href="#">[Code]</a>
            <a href="#">[BibTeX]</a>
        </div>
    </div>
</div>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="https://via.placeholder.com/220x140?text=Secure+Payment" alt="Payment System">
    </div>
    <div class="pub-details">
        <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210" class="pub-title">A Simplified Scheme for Secure Offline Electronic Payment Systems</a>
        <div class="pub-authors">
            [cite_start]<strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto [cite: 64]
        </div>
        <div class="pub-venue">
            High-Confidence Computing, 2021
        </div>
        <div class="pub-links">
            <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210">[Paper]</a>
        </div>
    </div>
</div>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="https://via.placeholder.com/220x140?text=Blind+Signature" alt="Blind Signature">
    </div>
    <div class="pub-details">
        <a href="http://www.itiis.org/digital-library/manuscript/1700" class="pub-title">An Offline Electronic Payment System Based on an Untraceable Blind Signature Scheme</a>
        <div class="pub-authors">
            <strong>Md. [cite_start]Abdullah Al Rahat Kutubi</strong>, et al. [cite: 69]
        </div>
        <div class="pub-venue">
            KSII Transactions on Internet and Information Systems, 2017
        </div>
        <div class="pub-links">
            <a href="http://www.itiis.org/digital-library/manuscript/1700">[Paper]</a>
        </div>
    </div>
</div>


<h2>🎓 Education & Experience</h2>
<ul>
    <li>
        <strong>Ph.D. [cite_start]Student in Computer Science</strong> (2021 - Present) [cite: 6, 10]<br>
        Georgia State University, Atlanta, USA
    </li>
    <li>
        [cite_start]<strong>Lecturer</strong> (2017 - 2021) [cite: 48, 50]<br>
        BAUET, Bangladesh
    </li>
    <li>
        [cite_start]<strong>M.Sc. in Applied Information Technology</strong> (2015 - 2017) [cite: 9, 12]<br>
        [cite_start]Kookmin University, South Korea (CGPA: 4.5/4.5) [cite: 13]
    </li>
    <li>
        [cite_start]<strong>Software Engineer</strong> (2015) [cite: 53]<br>
        SSDTECH, Dhaka, Bangladesh
    </li>
</ul>

<br><br>
<div style="font-size: 12px; color: #999; text-align: center;">
    Last updated: November 2025.
</div>
