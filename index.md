---
layout: default
title: Home
---  

<style>
    /* -----------------------------------------------------------------------
       GLOBAL STYLES (Haozhe Zhao / Academic Simple Theme)
       ----------------------------------------------------------------------- */
    body {
        font-family: 'Verdana', 'Segoe UI', sans-serif;
        font-size: 15px;
        line-height: 1.6;
        color: #333;
        max-width: 1000px;
        margin: 0 auto;
        padding: 40px 20px;
        background-color: #fff;
    }
    
    a { color: #0066cc; text-decoration: none; transition: color 0.2s; }
    a:hover { color: #004499; text-decoration: underline; }
    strong { color: #000; font-weight: 600; }

    /* -----------------------------------------------------------------------
       HEADER SECTION: Bio (Left) + Profile Image (Right)
       ----------------------------------------------------------------------- */
    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
        margin-bottom: 50px;
        border-bottom: 1px solid #f0f0f0;
        padding-bottom: 40px;
    }
    
    .bio-content {
        width: 72%;
        padding-right: 30px;
    }
    
    .bio-content h1 {
        font-size: 32px;
        font-weight: 700;
        margin-top: 0;
        margin-bottom: 5px;
        color: #111;
    }
    
    .bio-meta {
        font-size: 15px;
        color: #555;
        margin-bottom: 20px;
    }
    .bio-meta span { display: block; margin-bottom: 2px; }
    
    .social-links {
        margin-top: 20px;
        font-family: 'Courier New', monospace;
        font-size: 14px;
    }
    .social-links a { margin-right: 15px; font-weight: bold; }

    .profile-img-container {
        width: 25%;
        text-align: center;
    }
    
    .profile-img {
        width: 220px;
        height: 220px;
        object-fit: cover;
        border-radius: 50%;
        box-shadow: 0 5px 15px rgba(0,0,0,0.15);
        border: 4px solid #fff;
    }

    /* -----------------------------------------------------------------------
       SECTIONS & HEADERS
       ----------------------------------------------------------------------- */
    h2 {
        font-size: 22px;
        font-weight: 700;
        margin-top: 50px;
        margin-bottom: 25px;
        padding-bottom: 10px;
        border-bottom: 1px solid #eee;
        color: #111;
    }

    /* -----------------------------------------------------------------------
       NEWS SECTION
       ----------------------------------------------------------------------- */
    .news-item { margin-bottom: 12px; font-size: 15px; }
    .news-date { 
        font-family: 'Courier New', monospace; 
        font-weight: bold; 
        color: #444; 
        margin-right: 8px; 
    }

    /* -----------------------------------------------------------------------
       PUBLICATIONS & PROJECTS GRID
       ----------------------------------------------------------------------- */
    .item-container {
        display: flex;
        margin-bottom: 40px;
        gap: 30px;
    }
    
    .item-teaser {
        flex: 0 0 240px; /* Fixed width for teaser images */
        max-width: 240px;
    }
    
    .item-teaser img {
        width: 100%;
        border-radius: 5px;
        box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        border: 1px solid #f2f2f2;
        transition: transform 0.2s;
    }
    .item-teaser img:hover { transform: scale(1.02); }
    
    .item-details { flex: 1; }
    
    .item-title {
        font-weight: 700;
        font-size: 17px;
        color: #000;
        display: block;
        margin-bottom: 6px;
    }
    
    .item-meta { color: #555; margin-bottom: 6px; font-size: 15px; }
    .item-venue { font-style: italic; color: #666; margin-bottom: 10px; font-size: 15px; }
    .item-desc { font-size: 14px; color: #444; line-height: 1.5; margin-bottom: 12px; }
    
    .tag-links a {
        display: inline-block;
        font-size: 12px;
        font-weight: 600;
        text-transform: uppercase;
        border: 1px solid #ddd;
        border-radius: 3px;
        padding: 3px 8px;
        margin-right: 8px;
        color: #555;
        background-color: #fcfcfc;
    }
    .tag-links a:hover { background-color: #f0f0f0; color: #000; text-decoration: none; }

    /* -----------------------------------------------------------------------
       EDUCATION & EXPERIENCE LIST
       ----------------------------------------------------------------------- */
    .exp-list { list-style: none; padding: 0; }
    .exp-item {
        display: flex;
        margin-bottom: 15px;
        border-left: 2px solid #eee;
        padding-left: 20px;
    }
    .exp-date {
        flex: 0 0 120px;
        font-weight: bold;
        color: #666;
        font-size: 14px;
    }
    .exp-detail { flex: 1; }
    .exp-role { font-weight: bold; color: #000; }
    .exp-place { color: #555; }

    /* -----------------------------------------------------------------------
       RESPONSIVE DESIGN (Mobile)
       ----------------------------------------------------------------------- */
    @media (max-width: 768px) {
        .header-container { flex-direction: column-reverse; text-align: center; }
        .bio-content { width: 100%; padding: 0; }
        .profile-img-container { width: 100%; margin-bottom: 30px; }
        .item-container { flex-direction: column; }
        .item-teaser { width: 100%; max-width: 100%; margin-bottom: 15px; }
        .item-teaser img { max-width: 300px; margin: 0 auto; display: block; }
        .exp-item { flex-direction: column; }
        .exp-date { margin-bottom: 5px; }
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
            I am a Ph.D. student researching <strong>Generative AI</strong>, <strong>Vision-Language Models (VLM)</strong>, and <strong>Diffusion Models</strong>. I am currently advised by <a href="{{ site.author.advisor_url }}">{{ site.author.advisor }}</a>.
        </p>
        <p>
            My work focuses on building robust tools for instruction-based image editing (e.g., NaturalEdit) and dataset augmentation strategies. Previously, I was a Lecturer at BAUET and received my M.Sc. from Kookmin University.
        </p>

        <div class="social-links">
            <a href="mailto:{{ site.author.email }}">Email</a>
            <a href="assets/rahat_resume.pdf">CV / Resume</a>
            <a href="https://github.com/{{ site.author.github }}">GitHub</a>
            <a href="{{ site.author.scholar }}">Google Scholar</a>
        </div>
    </div>

    <div class="profile-img-container">
        <img src="assets/profile.jpg" alt="{{ site.author.name }}" class="profile-img">
    </div>
</div>

<h2>🔥 News</h2>
<div class="news-item">
    <span class="news-date">[Dec 2024]</span>
    Paper "Dataset Augmentation by Mixing Visual Concepts" accepted to <strong>WACV 2025</strong>!
</div>
<div class="news-item">
    <span class="news-date">[Aug 2021]</span>
    Started Ph.D. journey at Georgia State University.
</div>

<h2>📝 Selected Publications</h2>

{% assign publications = site.publications | sort: 'date' | reverse %}
{% for pub in publications %}
<div class="item-container">
    <div class="item-teaser">
        {% if pub.teaser %}
        <img src="{{ pub.teaser }}" alt="Teaser for {{ pub.title }}">
        {% endif %}
    </div>
    <div class="item-details">
        <a href="{{ pub.pdf | default: '#' }}" class="item-title">{{ pub.title }}</a>
        <div class="item-meta">{{ pub.authors }}</div>
        <div class="item-venue">{{ pub.venue }}</div>
        <div class="item-desc">{{ pub.content }}</div>
        
        <div class="tag-links">
            {% if pub.pdf %} <a href="{{ pub.pdf }}">[PDF]</a> {% endif %}
            {% if pub.code %} <a href="{{ pub.code }}">[Code]</a> {% endif %}
            {% if pub.video %} <a href="{{ pub.video }}">[Video]</a> {% endif %}
        </div>
    </div>
</div>
{% endfor %}

<h2>🛠️ Projects</h2>

{% assign projects = site.projects | sort: 'date' | reverse %}
{% for proj in projects %}
<div class="item-container">
    <div class="item-details">
        <a href="{{ proj.url | default: '#' }}" class="item-title">{{ proj.title }}</a>
        <div class="item-desc">{{ proj.content }}</div>
        <div class="tag-links">
            {% if proj.code %} <a href="{{ proj.code }}">[Source Code]</a> {% endif %}
        </div>
    </div>
</div>
{% endfor %}

<h2>💼 Experience</h2>
<ul class="exp-list">
    <li class="exp-item">
        <div class="exp-date">2021 – Present</div>
        <div class="exp-detail">
            <div class="exp-role">Graduate Research Assistant</div>
            <div class="exp-place">Georgia State University, Atlanta, GA</div>
        </div>
    </li>
    <li class="exp-item">
        <div class="exp-date">2017 – 2021</div>
        <div class="exp-detail">
            <div class="exp-role">Lecturer</div>
            <div class="exp-place">BAUET, Bangladesh</div>
        </div>
    </li>
    <li class="exp-item">
        <div class="exp-date">2015 – 2017</div>
        <div class="exp-detail">
            <div class="exp-role">Research Assistant</div>
            <div class="exp-place">Kookmin University, South Korea</div>
        </div>
    </li>
     <li class="exp-item">
        <div class="exp-date">2015</div>
        <div class="exp-detail">
            <div class="exp-role">Software Engineer</div>
            <div class="exp-place">SSDTECH, Dhaka, Bangladesh</div>
        </div>
    </li>
</ul>

<h2>🎓 Education</h2>
<ul class="exp-list">
    <li class="exp-item">
        <div class="exp-date">2021 – Present</div>
        <div class="exp-detail">
            <div class="exp-role">Ph.D. in Computer Science</div>
            <div class="exp-place">Georgia State University, Atlanta, GA</div>
        </div>
    </li>
    <li class="exp-item">
        <div class="exp-date">2015 – 2017</div>
        <div class="exp-detail">
            <div class="exp-role">M.Sc. in Applied Information Technology</div>
            <div class="exp-place">Kookmin University, South Korea (CGPA: 4.5/4.5)</div>
        </div>
    </li>
    <li class="exp-item">
        <div class="exp-date">2010 – 2014</div>
        <div class="exp-detail">
            <div class="exp-role">B.Sc. in Computer Science</div>
            <div class="exp-place">KUET, Khulna, Bangladesh</div>
        </div>
    </li>
</ul>

<br><br>
<div style="font-size: 12px; color: #999; text-align: center; border-top:1px solid #eee; padding-top:20px;">
    &copy; 2025 {{ site.author.name }}. Powered by Jekyll and GitHub Pages.
</div>
