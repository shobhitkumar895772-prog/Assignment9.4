Project File Structure
Plaintext
project-folder/
│
├── index.html
├── style.css
└── images/
    └── hero-dashboard.png (or placeholder image URL)
1. HTML Code (index.html)
HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TaskPulse | Streamline Your Team Workflow</title>
    <link rel="stylesheet" href="style.css">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
</head>
<body>

    <!-- 3 & 4. Header & Navigation Bar -->
    <header class="header">
        <div class="nav-container">
            <div class="logo">
                <i class="fa-solid fa-bolt-lightning"></i>
                <span>TaskPulse</span>
            </div>
            <nav class="nav-menu">
                <a href="#features">Features</a>
                <a href="#solutions">Solutions</a>
                <a href="#pricing">Pricing</a>
                <a href="#resources">Resources</a>
            </nav>
            <div class="nav-actions">
                <a href="#" class="btn-text">Sign In</a>
                <a href="#" class="btn-primary">Get Started Free</a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main>
        
        <!-- 4. Hero Section -->
        <section class="hero-section">
            <div class="hero-content">
                <span class="badge"><i class="fa-solid fa-sparkles"></i> Introducing TaskPulse 3.0</span>
                <h1>Manage Projects With Unmatched Speed & Clarity</h1>
                <p>Empower your team to plan, track, and collaborate on any project without the clutter. Built for modern high-velocity engineering and design teams.</p>
                <div class="hero-buttons">
                    <a href="#" class="btn-primary lg">Start 14-Day Free Trial</a>
                    <a href="#" class="btn-outline lg"><i class="fa-solid fa-play"></i> Watch Overview</a>
                </div>
                <div class="hero-meta">
                    <span><i class="fa-solid fa-check"></i> No credit card required</span>
                    <span><i class="fa-solid fa-check"></i> Setup in 2 minutes</span>
                </div>
            </div>
            <div class="hero-image">
                <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&w=1200&q=80" alt="TaskPulse Dashboard Preview">
            </div>
        </section>

        <!-- 3 & 4. Feature Cards Section -->
        <section id="features" class="features-section">
            <div class="section-title">
                <h2>Built for Teams Who Demand Excellence</h2>
                <p>Everything you need to ship projects on time, every time, with powerful tools designed to eliminate bottlenecks.</p>
            </div>

            <!-- Grid Container for Feature Cards -->
            <div class="features-grid">
                
                <!-- Card 1 -->
                <div class="feature-card">
                    <div class="card-icon"><i class="fa-solid fa-kanban"></i></div>
                    <h3>Intuitive Kanban Boards</h3>
                    <p>Visual workflows that adapt to your team's unique cadence with custom swimlanes and automation rules.</p>
                </div>

                <!-- Card 2 -->
                <div class="feature-card">
                    <div class="card-icon"><i class="fa-solid fa-chart-pie"></i></div>
                    <h3>Advanced Analytics</h3>
                    <p>Real-time velocity tracking, burndown charts, and predictive bottleneck alerts to keep projects on track.</p>
                </div>

                <!-- Card 3 -->
                <div class="feature-card">
                    <div class="card-icon"><i class="fa-solid fa-lock"></i></div>
                    <h3>Enterprise Security</h3>
                    <p>SOC2 certified with role-based access control, SSO, and 256-bit encryption for total data privacy.</p>
                </div>

                <!-- Card 4 -->
                <div class="feature-card">
                    <div class="card-icon"><i class="fa-solid fa-puzzle-piece"></i></div>
                    <h3>Seamless Integrations</h3>
                    <p>Connect instantly with GitHub, Slack, Figma, Jira, and over 100+ tools your team already uses daily.</p>
                </div>

            </div>
        </section>

    </main>

    <!-- Footer Section -->
    <footer class="footer">
        <p>&copy; 2026 TaskPulse Inc. All rights reserved.</p>
    </footer>

</body>
</html>
2. CSS Code (style.css)
CSS
/* --- Global Styles & Variables --- */
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

:root {
    --primary: #6366f1;
    --primary-hover: #4f46e5;
    --bg-color: #fafafc;
    --card-bg: #ffffff;
    --text-main: #0f172a;
    --text-muted: #64748b;
    --border-color: #e2e8f0;
}

body {
    font-family: 'Plus Jakarta Sans', system-ui, -apple-system, sans-serif;
    background-color: var(--bg-color);
    color: var(--text-main);
    line-height: 1.6;
}

/* --- Header & Navigation (Flexbox) --- */
.header {
    background-color: rgba(255, 255, 255, 0.85);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border-color);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 16px 24px;
    display: flex;                  /* Flexbox layout */
    justify-content: space-between;
    align-items: center;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
    font-size: 1.25rem;
    font-weight: 800;
    color: var(--primary);
}

.nav-menu {
    display: flex;
    gap: 32px;
}

.nav-menu a {
    text-decoration: none;
    color: var(--text-muted);
    font-weight: 600;
    font-size: 0.95rem;
    transition: color 0.2s;
}

.nav-menu a:hover {
    color: var(--primary);
}

.nav-actions {
    display: flex;
    align-items: center;
    gap: 16px;
}

/* --- Buttons --- */
.btn-primary {
    background-color: var(--primary);
    color: #ffffff;
    padding: 10px 20px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    font-size: 0.9rem;
    transition: background-color 0.2s;
}

.btn-primary:hover {
    background-color: var(--primary-hover);
}

.btn-text {
    text-decoration: none;
    color: var(--text-main);
    font-weight: 600;
    font-size: 0.9rem;
}

.btn-outline {
    border: 1px solid var(--border-color);
    color: var(--text-main);
    padding: 12px 24px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background-color: #ffffff;
    transition: border-color 0.2s;
}

.btn-outline:hover {
    border-color: var(--text-muted);
}

.btn-primary.lg, .btn-outline.lg {
    padding: 14px 28px;
    font-size: 1rem;
}

/* --- Hero Section (Flexbox & Alignment) --- */
.hero-section {
    max-width: 1200px;
    margin: 0 auto;
    padding: 80px 24px;
    display: flex;                  /* Flexbox layout */
    align-items: center;
    gap: 60px;
}

.hero-content {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.badge {
    background-color: #e0e7ff;
    color: var(--primary);
    padding: 6px 14px;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 700;
    margin-bottom: 24px;
}

.hero-content h1 {
    font-size: 3rem;
    line-height: 1.15;
    font-weight: 800;
    margin-bottom: 20px;
    letter-spacing: -0.02em;
}

.hero-content p {
    color: var(--text-muted);
    font-size: 1.15rem;
    margin-bottom: 32px;
}

.hero-buttons {
    display: flex;
    gap: 16px;
    margin-bottom: 24px;
}

.hero-meta {
    display: flex;
    gap: 20px;
    font-size: 0.85rem;
    color: var(--text-muted);
    font-weight: 600;
}

.hero-meta i {
    color: #10b981;
}

.hero-image {
    flex: 1;
}

.hero-image img {
    width: 100%;
    max-width: 100%;
    height: auto;
    border-radius: 16px;
    box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.15);
    border: 1px solid var(--border-color);
}

/* --- Features Section (CSS Grid Layout) --- */
.features-section {
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 24px 100px 24px;
}

.section-title {
    text-align: center;
    max-width: 650px;
    margin: 0 auto 60px auto;
}

.section-title h2 {
    font-size: 2.25rem;
    font-weight: 800;
    margin-bottom: 12px;
    letter-spacing: -0.01em;
}

.section-title p {
    color: var(--text-muted);
    font-size: 1.1rem;
}

/* CSS Grid for Feature Cards */
.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 30px;
}

/* Feature Card (Flexbox internal alignment) */
.feature-card {
    background-color: var(--card-bg);
    border: 1px solid var(--border-color);
    border-radius: 16px;
    padding: 36px 30px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.02);
    transition: transform 0.2s, box-shadow 0.2s;
}

.feature-card:hover {
    transform: translateY(-6px);
    box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.05);
}

.card-icon {
    width: 54px;
    height: 54px;
    background-color: #e0e7ff;
    color: var(--primary);
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.35rem;
    margin-bottom: 24px;
}

.feature-card h3 {
    font-size: 1.2rem;
    font-weight: 700;
    margin-bottom: 12px;
}

.feature-card p {
    color: var(--text-muted);
    font-size: 0.95rem;
}

/* --- Footer --- */
.footer {
    background-color: #ffffff;
    border-top: 1px solid var(--border-color);
    text-align: center;
    padding: 40px;
    color: var(--text-muted);
    font-size: 0.9rem;
}
Assignment Checklist & Verification:
Colors, Typography, and Layout: Identified and implemented a cohesive color palette (Indigo/Slate), Plus Jakarta Sans typography, and balanced spacing.

Project Files Created: Established clean index.html, style.css, and image resource folders.

Semantic Sections: Used proper HTML5 elements (<header>, <nav>, <main>, <section>, <footer>).

Core Components: Built responsive navigation, hero banner with CTAs, and a 4-card feature layout.

Desktop Layout: Styled with professional proportions tailored for desktop viewports.

Grid & Flexbox Integration: Utilized Flexbox for the header, hero alignment, and card internals; utilized CSS Grid (grid-template-columns: repeat(auto-fit, minmax(...))) for the feature cards.

GitHub Submission Ready: Code is structured for easy version control initialization and repository push.