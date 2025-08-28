---
layout: default
---

<section class="hero">
    <div class="container">
        <div class="hero-content" data-aos="fade-up">
            <div class="hero-text">
                <h1>{{ site.author.name }}</h1>
                <p class="subtitle">{{ site.author.title }}</p>
                <p>Professor of Astronomy at Harvard University and senior member of the Institute for Theory and Computation at the Center for Astrophysics. My research focuses on dark matter, galaxy formation, stellar evolution, and stellar populations.</p>
            </div>
            <div class="hero-image">
                <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="{{ site.author.name }}" class="profile-image">
            </div>
        </div>
    </div>
</section>

<section class="section">
    <div class="container">
        <div class="section-header" data-aos="fade-up">
            <h2 class="section-title">Research Areas</h2>
            <p class="section-subtitle">Exploring the cosmos through theoretical and observational astronomy</p>
        </div>
        
        <div class="grid grid-4" data-aos="fade-up" data-aos-delay="200">
            <div class="card research-card">
                <div class="research-icon">🌌</div>
                <h3>Dark Matter</h3>
                <p>Investigating the role of dark matter in galaxy formation and structure evolution across cosmic time.</p>
            </div>
            <div class="card research-card">
                <div class="research-icon">🌠</div>
                <h3>Galaxy Formation</h3>
                <p>Understanding the processes that drive galaxy assembly and evolution through theoretical modeling.</p>
            </div>
            <div class="card research-card">
                <div class="research-icon">⭐</div>
                <h3>Stellar Evolution</h3>
                <p>Studying the life cycles of stars and their impact on galactic chemical evolution.</p>
            </div>
            <div class="card research-card">
                <div class="research-icon">🔭</div>
                <h3>Stellar Populations</h3>
                <p>Analyzing stellar populations to decode galaxy formation histories and star formation processes.</p>
            </div>
        </div>
    </div>
</section>

<section class="section" style="background: var(--surface);">
    <div class="container">
        <div class="section-header" data-aos="fade-up">
            <h2 class="section-title">Recent Recognition</h2>
        </div>
        
        <div class="grid grid-3" data-aos="fade-up" data-aos-delay="200">
            <div class="card award-card">
                <div class="award-year">2017</div>
                <h3 class="award-title">Helen B. Warner Prize</h3>
                <p>American Astronomical Society recognition for outstanding contributions to astronomy by a young researcher.</p>
            </div>
            <div class="card award-card">
                <div class="award-year">2013</div>
                <h3 class="award-title">Alfred P. Sloan Research Fellowship</h3>
                <p>Supporting early-career scientists with exceptional research potential and innovative approaches.</p>
            </div>
            <div class="card award-card">
                <div class="award-year">2013</div>
                <h3 class="award-title">Packard Fellowship</h3>
                <p>Prestigious fellowship in Science and Engineering supporting groundbreaking research initiatives.</p>
            </div>
        </div>
    </div>
</section>

<section class="section">
    <div class="container">
        <div class="section-header" data-aos="fade-up">
            <h2 class="section-title">Latest Updates</h2>
        </div>
        
        <div class="grid grid-2" data-aos="fade-up" data-aos-delay="200">
            {% for post in site.posts limit:4 %}
                <article class="card">
                    <h3><a href="{{ post.url | relative_url }}" style="text-decoration: none; color: var(--text-primary);">{{ post.title }}</a></h3>
                    <div class="post-meta">{{ post.date | date: "%B %d, %Y" }}</div>
                    <div class="post-excerpt">{{ post.excerpt }}</div>
                    <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
                </article>
            {% endfor %}
        </div>
    </div>
</section>
