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
<h2>News</h2>
<div class="news-item">
    <span class="news-date">[Dec 2024]</span>
    Paper accepted to <strong>WACV 2025</strong>.
</div>
<div class="news-item">
    <span class="news-date">[Aug 2021]</span>
    Started Ph.D. at Georgia State University.
</div>

<!-- PUBLICATIONS -->
<h2>Selected Publications</h2>

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
        <div><strong>Kutubi, Md Abdullah Al Rahat</strong>, Kazi Md Rokibul Alam, Yasuhiko Morimoto</div>
        <div><em>High-Confidence Computing, 2021</em></div>
        <div class="pub-links">
            <a href="https://www.sciencedirect.com/science/article/pii/S2667295221000210">[Paper]</a>
        </div>
    </div>
</div>
