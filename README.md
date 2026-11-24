[11/25/26 12:29 AM] 🦁: <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080b14">
<meta name="description" content="Subhonbek Marufov — Python Developer from Uzbekistan. Exploring backend development and building digital solutions.">
<title>Subhonbek Marufov | Python Developer</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700;800&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<style>
:root {
    --bg: #080b14;
    --surface: #101625;
    --surface2: #141d30;
    --primary: #55a6ff;
    --secondary: #8b7bff;
    --text: #f3f6ff;
    --muted: #8995aa;
    --border: rgba(255,255,255,.08);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    background: var(--bg);
    color: var(--text);
    font-family: 'DM Sans', sans-serif;
    overflow-x: hidden;
}

a {
    color: inherit;
    text-decoration: none;
}

.container {
    width: min(1120px, 90%);
    margin: auto;
}

nav {
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 100;
    background: rgba(8,11,20,.8);
    backdrop-filter: blur(20px);
    border-bottom: 1px solid var(--border);
}

.nav-inner {
    height: 76px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font: 700 24px 'Space Grotesk';
    letter-spacing: -1px;
}

.logo span { color: var(--primary); }

.nav-links {
    display: flex;
    gap: 32px;
    align-items: center;
}

.nav-links a {
    color: var(--muted);
    font-size: 14px;
    transition: .3s;
}

.nav-links a:hover { color: var(--primary); }

.menu-btn {
    display: none;
    border: 0;
    background: none;
    color: white;
    font-size: 23px;
    cursor: pointer;
}

.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    position: relative;
    overflow: hidden;
}

.glow {
    position: absolute;
    width: 450px;
    height: 450px;
    background: var(--primary);
    filter: blur(180px);
    opacity: .13;
    border-radius: 50%;
    top: 10%;
    right: -100px;
    pointer-events: none;
}

.hero-content {
    position: relative;
    max-width: 850px;
    padding-top: 90px;
}

.available {
    display: inline-flex;
    gap: 10px;
    align-items: center;
    color: #7de4ae;
    background: rgba(125,228,174,.08);
    border: 1px solid rgba(125,228,174,.2);
    padding: 10px 16px;
    border-radius: 30px;
    font-size: 13px;
    margin-bottom: 32px;
}

.dot {
    width: 7px;
    height: 7px;
    background: #7de4ae;
    border-radius: 50%;
    box-shadow: 0 0 12px #7de4ae;
}

.hero h1 {
    font: 700 clamp(42px, 7vw, 82px)/1.08 'Space Grotesk';
    letter-spacing: -4px;
    margin-bottom: 22px;
}

.gradient {
    background: linear-gradient(100deg, #55a6ff, #a18aff);
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}

.hero p {
    max-width: 620px;
    color: var(--muted);
    font-size: 17px;
    line-height: 1.9;
}

.hero-actions {
    display: flex;
    gap: 15px;
    margin-top: 38px;
    flex-wrap: wrap;
}

.btn {
    padding: 14px 23px;
    border-radius: 9px;
    font-weight: 600;
    font-size: 14px;
    transition: .3s;
    display: inline-flex;
    align-items: center;
    gap: 10px;
}

.btn-primary {
    background: var(--primary);
    color: #07101d;
}

.btn-primary:hover {
    transform: translateY(-4px);
    box-shadow: 0 10px 30px rgba(85,166,255,.2);
}

.btn-outline {
    border: 1px solid var(--border);
    color: white;
}

.btn-outline:hover {
    border-color: var(--primary);
    color: var(--primary);
}

.socials {
    display: flex;
    gap: 23px;
    margin-top: 45px;
}

.socials a {
    color: var(--muted);
    font-size: 21px;
    transition: .3s;
}
[11/25/26 12:29 AM] 🦁: .socials a:hover {
    color: var(--primary);
    transform: translateY(-4px);
}

section {
    padding: 110px 0;
}

.section-label {
    color: var(--primary);
    font-size: 13px;
    font-weight: 700;
    letter-spacing: 3px;
    text-transform: uppercase;
    margin-bottom: 15px;
}

.section-title {
    font: 700 clamp(30px, 4vw, 45px) 'Space Grotesk';
    letter-spacing: -1.5px;
    margin-bottom: 18px;
}

.section-desc {
    color: var(--muted);
    max-width: 600px;
    line-height: 1.8;
}

.about-grid {
    display: grid;
    grid-template-columns: 1.3fr .7fr;
    gap: 55px;
    align-items: center;
    margin-top: 45px;
}

.about-text p {
    color: var(--muted);
    line-height: 2;
    margin-bottom: 17px;
}

.about-card {
    background: linear-gradient(145deg, #131e32, #0d1422);
    border: 1px solid var(--border);
    border-radius: 20px;
    padding: 30px;
}

.about-card h3 {
    font: 600 21px 'Space Grotesk';
    margin-bottom: 25px;
}

.info-row {
    display: flex;
    justify-content: space-between;
    padding: 15px 0;
    border-bottom: 1px solid var(--border);
    font-size: 13px;
}

.info-row:last-child { border: 0; }
.info-row span:first-child { color: var(--muted); }
.info-row span:last-child { color: var(--primary); }

.skills {
    background: #0b101c;
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
}

.skills-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    margin-top: 45px;
}

.skill-card {
    padding: 28px;
    border-radius: 15px;
    background: var(--surface);
    border: 1px solid var(--border);
    transition: .3s;
}

.skill-card:hover {
    transform: translateY(-6px);
    border-color: rgba(85,166,255,.4);
}

.skill-icon {
    font-size: 26px;
    color: var(--primary);
    margin-bottom: 22px;
}

.skill-card h3 {
    font: 600 19px 'Space Grotesk';
    margin-bottom: 17px;
}

.skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 9px;
}

.skill-tags span {
    padding: 7px 11px;
    border-radius: 6px;
    background: var(--surface2);
    color: #b7c4da;
    font-size: 12px;
}

.focus-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 18px;
    margin-top: 40px;
}

.focus-card {
    padding: 24px;
    background: var(--surface);
    border: 1px solid var(--border);
    border-radius: 13px;
    display: flex;
    gap: 18px;
    align-items: center;
}

.focus-card i {
    font-size: 22px;
    color: var(--secondary);
}

.focus-card h4 {
    font-size: 15px;
    margin-bottom: 5px;
}

.focus-card p {
    color: var(--muted);
    font-size: 12px;
}

.github-section {
    background: #0b101c;
    border-top: 1px solid var(--border);
}

.github-card {
    margin-top: 35px;
    padding: 30px;
    border: 1px solid var(--border);
    border-radius: 18px;
    background: var(--surface);
    text-align: center;
}

.github-card i {
    font-size: 45px;
    margin-bottom: 20px;
}

.github-card p {
    color: var(--muted);
    line-height: 1.8;
    margin: 12px auto 25px;
    max-width: 550px;
}

.contact-box {
    margin-top: 40px;
    padding: 55px 30px;
    text-align: center;
    border-radius: 22px;
    background: linear-gradient(130deg, #12213a, #17142f);
    border: 1px solid rgba(85,166,255,.2);
}

.contact-box h2 {
    font: 700 clamp(30px, 5vw, 48px) 'Space Grotesk';
    margin-bottom: 17px;
}

.contact-box p {
    color: #a6b3ca;
    line-height: 1.8;
    margin-bottom: 30px;
}

footer {
    border-top: 1px solid var(--border);
    padding: 28px 0;
    color: var(--muted);
    font-size: 13px;
}

.footer-inner {
    display: flex;
    justify-content: space-between;
    gap: 15px;
    flex-wrap: wrap;
}

.reveal {
    opacity: 0;
    transform: translateY(25px);
    transition: .7s ease;
}

.reveal.show {
    opacity: 1;
    transform: translateY(0);
}
[11/25/26 12:29 AM] 🦁: @media(max-width: 750px) {
    .nav-links {
        display: none;
        position: absolute;
        top: 76px;
        left: 0;
        width: 100%;
        background: #101625;
        padding: 25px;
        flex-direction: column;
        border-bottom: 1px solid var(--border);
    }

    .nav-links.active { display: flex; }
    .menu-btn { display: block; }

    .hero h1 { letter-spacing: -2px; }
    .about-grid { grid-template-columns: 1fr; gap: 30px; }
    .skills-grid { grid-template-columns: 1fr; }
    .focus-grid { grid-template-columns: 1fr; }
    section { padding: 80px 0; }
}
</style>
</head>

<body>

<nav>
    <div class="container nav-inner">
        <a href="#" class="logo">subhonbek<span>.</span></a>

        <div class="nav-links" id="navLinks">
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#focus">Focus</a>
            <a href="#contact">Contact</a>
        </div>

        <button class="menu-btn" id="menuBtn" aria-label="Toggle menu">
            <i class="fa-solid fa-bars"></i>
        </button>
    </div>
</nav>

<main>
<section class="hero" id="home">
    <div class="glow"></div>
    <div class="container">
        <div class="hero-content reveal">
            <div class="available">
                <span class="dot"></span>
                Always learning & building
            </div>

            <h1>
                Hey, I'm<br>
                <span class="gradient">Subhonbek.</span>
            </h1>

            <p>
                Python Developer from Uzbekistan, passionate about
                backend engineering, clean code, and building
                technology that makes a difference.
            </p>

            <div class="hero-actions">
                <a href="#about" class="btn btn-primary">
                    Explore my profile <i class="fa-solid fa-arrow-right"></i>
                </a>
                <a href="https://github.com/marufovsubhonbe-code"
                   target="_blank" rel="noopener noreferrer"
                   class="btn btn-outline">
                    <i class="fa-brands fa-github"></i> GitHub Profile
                </a>
            </div>

            <div class="socials">
                <a href="https://github.com/marufovsubhonbe-code"
                   target="_blank" rel="noopener noreferrer"
                   aria-label="GitHub"><i class="fa-brands fa-github"></i></a>

                <a href="mailto:msubhonbe@gmail.com"
                   aria-label="Email"><i class="fa-solid fa-envelope"></i></a>
            </div>
        </div>
    </div>
</section>

<section id="about">
    <div class="container reveal">
        <div class="section-label">01 / About me</div>
        <h2 class="section-title">A little about myself.</h2>
        <p class="section-desc">
            Curious mind. Developer mindset. Continuous growth.
        </p>

        <div class="about-grid">
            <div class="about-text">
                <p>
                    Hello! I'm Subhonbek Marufov, a developer from
                    Uzbekistan who enjoys exploring the world of
                    programming and technology.
                </p>
                <p>
                    My current journey revolves around Python,
                    backend development, and database technologies.
                    I enjoy understanding how systems work behind
                    the scenes and turning ideas into working solutions.
                </p>
                <p>
                    I believe that becoming a great developer is not
                    about knowing everything — it's about learning,
                    experimenting, and improving every day.
                </p>
            </div>
[11/25/26 12:29 AM] 🦁: <div class="about-card">
                <h3>Quick overview</h3>
                <div class="info-row">
                    <span>Name</span>
                    <span>Subhonbek</span>
                </div>
                <div class="info-row">
                    <span>Location</span>
                    <span>Uzbekistan</span>
                </div>
                <div class="info-row">
                    <span>Main language</span>
                    <span>Python</span>
                </div>
                <div class="info-row">
                    <span>Focus</span>
                    <span>Backend</span>
                </div>
                <div class="info-row">
                    <span>Mindset</span>
                    <span>Keep learning</span>
                </div>
            </div>
        </div>
    </div>
</section>

<section class="skills" id="skills">
    <div class="container reveal">
        <div class="section-label">02 / Technologies</div>
        <h2 class="section-title">Tools I explore.</h2>
        <p class="section-desc">
            Technologies and tools I'm currently learning and working with.
        </p>

        <div class="skills-grid">
            <div class="skill-card">
                <div class="skill-icon"><i class="fa-brands fa-python"></i></div>
                <h3>Programming & Web</h3>
                <div class="skill-tags">
                    <span>Python</span>
                    <span>HTML5</span>
                    <span>CSS3</span>
                </div>
            </div>

            <div class="skill-card">
                <div class="skill-icon"><i class="fa-solid fa-server"></i></div>
                <h3>Backend Development</h3>
                <div class="skill-tags">
                    <span>Django</span>
                    <span>Backend</span>
                </div>
            </div>

            <div class="skill-card">
                <div class="skill-icon"><i class="fa-solid fa-database"></i></div>
                <h3>Databases</h3>
                <div class="skill-tags">
                    <span>PostgreSQL</span>
                    <span>SQLite</span>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="focus">
    <div class="container reveal">
        <div class="section-label">03 / My direction</div>
        <h2 class="section-title">What I'm working towards.</h2>
        <p class="section-desc">
            My goals are built around curiosity, consistency,
            and practical experience.
        </p>

        <div class="focus-grid">
            <div class="focus-card">
                <i class="fa-solid fa-code"></i>
                <div>
                    <h4>Build real-world projects</h4>
                    <p>Turn ideas into practical software.</p>
                </div>
            </div>

            <div class="focus-card">
                <i class="fa-solid fa-brain"></i>
                <div>
                    <h4>Deepen technical knowledge</h4>
                    <p>Understand systems beyond the surface.</p>
                </div>
            </div>

            <div class="focus-card">
                <i class="fa-solid fa-database"></i>
                <div>
                    <h4>Master backend technologies</h4>
                    <p>Explore databases and backend architecture.</p>
                </div>
            </div>

            <div class="focus-card">
                <i class="fa-brands fa-linux"></i>
                <div>
                    <h4>Explore open source</h4>
                    <p>Learn through Linux and open-source communities.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<section class="github-section">
    <div class="container reveal">
        <div class="section-label">04 / My activity</div>
        <h2 class="section-title">Let's build something.</h2>
        <p class="section-desc">
            Follow my journey, explore my repositories,
            and see what I'm working on.
        </p>
[11/25/26 12:29 AM] 🦁: <div class="github-card">
            <i class="fa-brands fa-github"></i>
            <h3>Find me on GitHub</h3>
            <p>
                Explore my code, projects, experiments,
                and continuous learning journey.
            </p>
            <a class="btn btn-primary"
               href="https://github.com/marufovsubhonbe-code"
               target="_blank" rel="noopener noreferrer">
                Visit GitHub <i class="fa-solid fa-arrow-up-right-from-square"></i>
            </a>
        </div>
    </div>
</section>

<section id="contact">
    <div class="container reveal">
        <div class="contact-box">
            <div class="section-label">05 / Get in touch</div>
            <h2>Have an idea?</h2>
            <p>
                I'm always interested in technology, new ideas,
                and opportunities to learn and collaborate.
            </p>
            <a href="mailto:msubhonbe@gmail.com" class="btn btn-primary">
                <i class="fa-solid fa-paper-plane"></i> Say Hello
            </a>
        </div>
    </div>
</section>
</main>

<footer>
    <div class="container footer-inner">
        <span>© 2026 Subhonbek Marufov</span>
        <span>Designed with purpose. Built with curiosity.</span>
    </div>
</footer>

<script>
const menuBtn = document.getElementById('menuBtn');
const navLinks = document.getElementById('navLinks');

menuBtn.addEventListener('click', () => {
    navLinks.classList.toggle('active');
    menuBtn.innerHTML = navLinks.classList.contains('active')
        ? '<i class="fa-solid fa-xmark"></i>'
        : '<i class="fa-solid fa-bars"></i>';
});

document.querySelectorAll('.nav-links a').forEach(link => {
    link.addEventListener('click', () => {
        navLinks.classList.remove('active');
        menuBtn.innerHTML = '<i class="fa-solid fa-bars"></i>';
    });
});

const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('show');
            observer.unobserve(entry.target);
        }
    });
}, { threshold: 0.12 });

document.querySelectorAll('.reveal').forEach(element => {
    observer.observe(element);
});
</script>

</body>
</html>
