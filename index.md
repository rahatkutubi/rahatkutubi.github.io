---
layout: default
title: Abdullah Al Rahat
---

<style>
    /* GLOBAL FONTS & SETTINGS */
    body {
        font-family: 'Verdana', sans-serif; /* Clean sans-serif like the reference */
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

    /* PUBLICATION GRID (The Haozhe Zhao Style) */
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
            I am a Ph.D. student in Computer Science at <a href="https://www.gsu.edu/">Georgia State University</a>, advised by <a href="YOUR_ADVISOR_LINK">Dr. Hemanth Venkateswara</a>[cite: 6, 63].
        </p>
        <p>
            My research interests lie in <strong>Generative AI</strong>, <strong>Vision-Language Models (VLMs)</strong>, and <strong>Diffusion Models</strong>[cite: 4]. I am particularly interested in instruction-based image editing and dataset augmentation strategies to improve model robustness.
        </p>
        <p>
            Previously, I received my M.Sc. from <a href="https://english.kookmin.ac.kr/">Kookmin University</a> and served as a Lecturer at BAUET[cite: 9, 50].
        </p>
        <div class="social-links">
            <a href="mailto:rahatcse2k9@gmail.com">Email</a>
            <a href="assets/rahat_resume.pdf">CV</a>
            <a href="YOUR_SCHOLAR_LINK">Google Scholar</a>
            <a href="https://github.com/rahatkutubi">GitHub</a>
            <a href="YOUR_LINKEDIN_LINK">LinkedIn</a>
        </div>
    </div>
    <div class="profile-img-container">
        <img src="assets/profile.jpg" alt="Abdullah Al Rahat" class="profile-img">
    </div>
</div>

<h2>🔥 News</h2>
<div class="news-item">
    <span class="news-date">[Dec 2024]</span>
    One paper accepted to <strong>WACV 2025</strong>! [cite: 63]
</div>
<div class="news-item">
    <span class="news-date">[Aug 2021]</span>
    Started my Ph.D. journey at Georgia State University. [cite: 10]
</div>

<h2>📝 Selected Publications</h2>

<div class="pub-item">
    <div class="pub-teaser">
        <img src="assets/wacv_teaser.png" alt="WACV Teaser">
    </div>
    <div class="pub-details">
        <a href="https://arxiv.org/abs/2412.15358" class="pub-title">Dataset Augmentation by Mixing Visual Concepts</a>
        <div class="pub-authors">
            <strong>Abdullah Al Rahat</strong>, Hemanth Venkateswara
        </div>
        <div class="pub-venue">
            IEEE/CVF Winter Conference on Applications of Computer Vision (WACV), 2025
        </div>
        <div class="pub-desc">
            We introduce a novel augmentation technique that mixes visual concepts at the feature level to improve generalization in low-data regimes. [cite: 63]
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
        <img src="assets/payment_teaser.png" alt="Payment System">
    </div>
    <div class="pub-details">
        <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210" class="pub-title">A Simplified Scheme for Secure Offline Electronic Payment Systems</a>
        <div class="pub-authors">
            <strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto
        </div>
        <div class="pub-venue">
            High-Confidence Computing, 2021
        </div>
        <div class="pub-links">
            <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210">[Paper]</a>
        </div>
    </div>
</div>

<h2>🎓 Education & Experience</h2>
<ul>
    <li>
        <strong>Ph.D. Student, Computer Science</strong> (2021 - Present)<br>
        Georgia State University, Atlanta, USA [cite: 6, 10]
    </li>
    <li>
        <strong>Lecturer</strong> (2017 - 2021)<br>
        BAUET, Bangladesh [cite: 49, 50]
    </li>
    <li>
        <strong>M.Sc. in Applied Information Technology</strong> (2015 - 2017)<br>
        Kookmin University, South Korea [cite: 9, 11]
    </li>
    <li>
        <strong>B.Sc. in Computer Science</strong> (2010 - 2014)<br>
        KUET, Bangladesh [cite: 16, 32]
    </li>
</ul>

<br><br>
<div style="font-size: 12px; color: #999; text-align: center;">
    Template inspired by Haozhe Zhao. Last updated: November 2025.
</div>
