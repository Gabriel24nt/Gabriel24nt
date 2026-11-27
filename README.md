
<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Alan Gabriel Nte | Portfolio</title>

<style>
:root {
    --background: #050914;
    --navy: #0A1630;
    --card: #0C1930;
    --blue: #168BFF;
    --cyan: #00C8FF;
    --white: #EAF2FF;
    --muted: #A9BBD5;
    --border: #20385E;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: var(--background);
    color: var(--white);
    min-height: 100vh;
}

body::before {
    content: "";
    position: fixed;
    inset: 0;
    background:
        radial-gradient(circle at 15% 15%, #1264bd25, transparent 40%),
        radial-gradient(circle at 85% 50%, #008bff18, transparent 45%),
        radial-gradient(circle at 50% 95%, #00c8ff12, transparent 40%);
    pointer-events: none;
    z-index: -1;
}

.container {
    max-width: 760px;
    margin: auto;
    padding: 35px 22px;
}

/* HEADER */

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 25px;
    font-weight: 900;
    letter-spacing: -1px;
}

.logo span {
    color: var(--blue);
}

.menu {
    color: white;
    font-size: 26px;
    text-decoration: none;
}

/* HERO */

.hero {
    text-align: center;
    margin: 85px 0 55px;
}

.avatar {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    margin: 0 auto 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 55px;
    font-weight: 900;
    background: linear-gradient(135deg, #10264B, #168BFF, #00C8FF);
    border: 4px solid var(--blue);
    box-shadow: 0 0 35px #168bff30;
}

.hero h1 {
    font-size: clamp(32px, 6vw, 55px);
    font-weight: 900;
    margin-bottom: 20px;
    letter-spacing: -2px;
}

.hero h1 span {
    background: linear-gradient(90deg, #168BFF, #00C8FF);
    -webkit-background-clip: text;
    color: transparent;
}

.subtitle {
    font-size: 19px;
    color: var(--muted);
    line-height: 1.7;
    max-width: 500px;
    margin: auto;
}

/* SECTION */

.section-title {
    text-align: center;
    margin: 45px 0 25px;
    color: var(--cyan);
    font-size: 13px;
    letter-spacing: 3px;
    text-transform: uppercase;
}

/* CARDS */

.links {
    display: flex;
    flex-direction: column;
    gap: 18px;
}

.card {
    display: flex;
    align-items: center;
    gap: 18px;
    padding: 23px;
    text-decoration: none;
    color: white;

    background: linear-gradient(
        135deg,
        rgba(16,38,75,0.65),
        rgba(8,19,39,0.9)
    );

    border: 1px solid var(--border);
    border-radius: 24px;
    backdrop-filter: blur(12px);

    transition: all 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
    border-color: var(--blue);
    box-shadow: 0 10px 35px #168bff20;
    background: linear-gradient(
        135deg,
        #10264b,
        #0c1930
    );
}

.icon {
    min-width: 60px;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 50%;
    background: #10264B;
    border: 1px solid #254d7d;
    font-size: 27px;
}

.card-content {
    flex: 1;
}

.card h2 {
    font-size: 19px;
    margin-bottom: 8px;
}

.card p {
    color: var(--muted);
    font-size: 15px;
    line-height: 1.5;
}

.arrow {
    font-size: 25px;
    color: var(--cyan);
}

/* ABOUT */

.about {
    margin-top: 45px;
    padding: 25px;
    border-radius: 24px;
    background: #0A1630AA;
    border: 1px solid var(--border);
}

.about h2 {
    margin-bottom: 15px;
    color: var(--cyan);
}

.about p {
    color: var(--muted);
    line-height: 1.8;
    font-size: 15px;
}

/* FOOTER */

footer {
    margin-top: 65px;
    padding-top: 30px;
    border-top: 1px solid #20385e;
    text-align: center;
}

footer h2 {
    font-size: 22px;
    line-height: 1.6;
}

footer span {
    color: var(--blue);
}

.socials {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin: 25px 0;
}

.socials a {
    text-decoration: none;
    color: white;
    background: #10264B;
    border: 1px solid #254d7d;
    border-radius: 50%;
    width: 48px;
    height: 48px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: 0.3s;
}

.socials a:hover {
    background: var(--blue);
    transform: translateY(-3px);
}

.copyright {
    color: #647d9f;
    font-size: 13px;
    margin-top: 25px;
}

/* MOBILE */

@media (max-width: 600px) {
    .container {
        padding: 25px 18px;
    }

    .hero {
        margin-top: 65px;
    }

    .avatar {
        width: 130px;
        height: 130px;
    }

    .card {
        padding: 18px;
        gap: 13px;
        border-radius: 20px;
    }

    .icon {
        min-width: 52px;
        height: 52px;
        font-size: 23px;
    }

    .card h2 {
        font-size: 17px;
    }

    .card p {
        font-size: 14px;
    }
}
</style>
</head>

<body>

<div class="container">

<header>
    <div class="logo">AG<span>.</span> PORTFOLIO</div>
    <a class="menu" href="#projects">☰</a>
</header>

<section class="hero">

    <div class="avatar">AG</div>

    <h1>Alan Gabriel <span>Nte</span></h1>

    <p class="subtitle">
        Finance, Strategic Intelligence & Technology.<br>
        I analyze. I build. I create strategic value.
    </p>

</section>

<h3 class="section-title" id="projects">
    Explore my universe
</h3>

<div class="links">

    <a class="card"
       href="https://github.com/Alan-Nte"
       target="_blank">
        <div class="icon">⌘</div>
        <div class="card-content">
            <h2>GitHub</h2>
            <p>My code, projects and experiments</p>
        </div>
        <div class="arrow">›</div>
    </a>

    <a class="card" href="#">
        <div class="icon">🌐</div>
        <div class="card-content">
            <h2>STRATOS</h2>
            <p>Strategic Intelligence Platform</p>
        </div>
        <div class="arrow">›</div>
    </a>

    <a class="card" href="#">
        <div class="icon">📊</div>
        <div class="card-content">
            <h2>Equity Research</h2>
            <p>Financial modelling, valuation and investment analysis</p>
        </div>
        <div class="arrow">›</div>
    </a>

    <a class="card" href="#">
        <div class="icon">🌍</div>
        <div class="card-content">
            <h2>Meridian Risk Advisory</h2>
            <p>Economic intelligence, country risk and strategy</p>
        </div>
        <div class="arrow">›</div>
    </a>

    <a class="card" href="#">
        <div class="icon">💼</div>
        <div class="card-content">
            <h2>LinkedIn</h2>
            <p>My professional journey and insights</p>
        </div>
        <div class="arrow">›</div>
    </a>

    <a class="card" href="#">
        <div class="icon">📈</div>
        <div class="card-content">
            <h2>Financial Analysis Platform</h2>
            <p>Financial modelling and business performance analysis</p>
        </div>
        <div class="arrow">›</div>
    </a>

</div>

<section class="about">
    <h2>About me</h2>
    <p>
        Business school student passionate about financial analysis,
        investment banking, economic intelligence, strategic consulting
        and technology. I build analytical projects to develop practical
        skills and support better decision-making.
    </p>
</section>

<footer>

    <h2>
        Built with curiosity.<br>
        <span>Driven by strategy.</span>
    </h2>

    <div class="socials">
        <a href="https://github.com/Alan-Nte" target="_blank">⌘</a>
        <a href="#" target="_blank">in</a>
        <a href="mailto:contact@example.com">✉</a>
    </div>

    <p class="copyright">
        © 2026 Alan Gabriel Nte · All rights reserved
    </p>

</footer>

</div>

</body>
</html>
