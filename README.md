<!-- Google Calendar Appointment Scheduling Stylesheet -->
<link href="https://calendar.google.com/calendar/scheduling-button-script.css" rel="stylesheet">

<style>
    :root {
        --bg-dark: #0f0a1c;
        --card-bg: #1c1033;
        --border-color: #3b1d6e;
        --text-main: #fcf7ff;
        --text-muted: #c2b5de;
        --accent-purple: #d946ef;
        --glow-color: rgba(217, 70, 239, 0.15);
    }

    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: 'Inter', sans-serif;
    }

    body {
        background-color: var(--bg-dark);
        color: var(--text-main);
        line-height: 1.6;
    }

    /* Navigation */
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1.5rem 5%;
        background: rgba(15, 10, 28, 0.85);
        backdrop-filter: blur(12px);
        position: sticky;
        top: 0;
        z-index: 100;
        border-bottom: 1px solid var(--border-color);
    }

    .logo {
        font-size: 1.35rem;
        font-weight: 700;
        color: var(--text-main);
    }

    .logo span {
        color: var(--accent-purple);
    }

    /* Hero Section */
    .hero {
        position: relative;
        padding: 6rem 5% 4rem;
        text-align: center;
        background: radial-gradient(circle at center, rgba(217, 70, 239, 0.12) 0%, rgba(15, 10, 28, 0) 70%);
    }

    .hero h1 {
        font-size: 3.2rem;
        font-weight: 700;
        letter-spacing: -0.03em;
        margin-bottom: 1rem;
        background: linear-gradient(135deg, #ffffff 0%, #e879f9 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    .hero p {
        font-size: 1.2rem;
        color: var(--text-muted);
        max-width: 650px;
        margin: 0 auto 2.5rem;
    }

    /* Services Grid Section */
    .services-section {
        padding: 4rem 5%;
        max-width: 1200px;
        margin: 0 auto;
    }

    .section-header {
        text-align: center;
        margin-bottom: 3.5rem;
    }

    .section-header h2 {
        font-size: 2rem;
        font-weight: 600;
        margin-bottom: 0.5rem;
    }

    .section-header p {
        color: var(--text-muted);
    }

    .services-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 1.5rem;
    }

    .service-card {
        background-color: var(--card-bg);
        border: 1px solid var(--border-color);
        border-radius: 12px;
        padding: 2.5rem 1.5rem;
        text-align: center;
        transition: transform 0.2s ease, border-color 0.2s ease;
    }

    .service-card:hover {
        transform: translateY(-4px);
        border-color: var(--accent-purple);
        box-shadow: 0 8px 25px var(--glow-color);
    }

    .icon-box {
        width: 56px;
        height: 56px;
        background: rgba(217, 70, 239, 0.12);
        border: 1px solid rgba(217, 70, 239, 0.25);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        margin: 0 auto 1.5rem;
        color: var(--accent-purple);
    }

    .icon-box svg {
        width: 26px;
        height: 26px;
        fill: none;
        stroke: currentColor;
        stroke-width: 2;
        stroke-linecap: round;
        stroke-linejoin: round;
    }

    .service-card h3 {
        font-size: 1.2rem;
        font-weight: 600;
        margin-bottom: 0.75rem;
    }

    .service-card p {
        color: var(--text-muted);
        font-size: 0.9rem;
        line-height: 1.5;
    }

    /* Call To Action Banner */
    .cta-banner {
        margin: 2rem 5% 5rem;
        max-width: 1200px;
        margin-left: auto;
        margin-right: auto;
        background: linear-gradient(135deg, #241242 0%, #100624 100%);
        border: 1px solid var(--border-color);
        border-radius: 16px;
        padding: 3.5rem 2rem;
        text-align: center;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
    }

    .cta-banner h3 {
        font-size: 2rem;
        margin-bottom: 1rem;
    }

    .cta-banner p {
        color: var(--text-muted);
        max-width: 600px;
        margin: 0 auto 2.5rem;
    }

    .btn-container {
        display: flex;
        justify-content: center;
    }

    @media (max-width: 768px) {
        .hero h1 { font-size: 2.3rem; }
    }
</style>
