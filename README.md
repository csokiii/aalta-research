<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aalta Talent | Independent Recruitment Partner</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
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
</head>
<body>

    <!-- Navigation -->
    <nav>
        <div class="logo">Aalta <span>Talent</span></div>
        <div id="nav-calendar-btn"></div>
    </nav>

    <!-- Hero Section -->
    <header class="hero">
        <h1>For Employers & Startups</h1>
        <p>Strategic tech recruitment, market mapping, and executive search without agency bloat or delays.</p>
        <div id="hero-calendar-btn"></div>
    </header>

    <!-- Core Services -->
    <section class="services-section">
        <div class="section-header">
            <h2>Our Recruitment Services</h2>
            <p>Targeted capabilities to scale your engineering, product, and leadership teams.</p>
        </div>

        <div class="services-grid">
            <div class="service-card">
                <div class="icon-box">
                    <svg viewBox="0 0 24 24"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path><circle cx="9" cy="7" r="4"></circle><path d="M23 21v-2a4 4 0 0 0-3-3.87"></path><path d="M16 3.13a4 4 0 0 1 0 7.75"></path></svg>
                </div>
                <h3>Candidate Sourcing</h3>
                <p>Targeted passive talent outreach across niche networks to identify top-tier engineering and product professionals.</p>
            </div>

            <div class="service-card">
                <div class="icon-box">
                    <svg viewBox="0 0 24 24"><polygon points="12 2 2 7 12 12 22 7 12 2"></polygon><polyline points="2 17 12 22 22 17"></polyline><polyline points="2 12 12 17 22 12"></polyline></svg>
                </div>
                <h3>Talent Mapping</h3>
                <p>Comprehensive market analysis to map skill availability, location metrics, and compensation benchmarks.</p>
            </div>

            <div class="service-card">
                <div class="icon-box">
                    <svg viewBox="0 0 24 24"><circle cx="11" cy="11" r="8"></circle><line x1="21" y1="21" x2="16.65" y2="16.65"></line></svg>
                </div>
                <h3>Competitor Scouting</h3>
                <p>In-depth intelligence gathering to identify and engage top performers from key industry competitors.</p>
            </div>

            <div class="service-card">
                <div class="icon-box">
                    <svg viewBox="0 0 24 24"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"></path></svg>
                </div>
                <h3>Interviewing & Vetting</h3>
                <p>Structured behavioral and technical evaluations ensuring only high-signal candidates reach your schedule.</p>
            </div>
        </div>
    </section>

    <!-- Call to Action Banner -->
    <section class="cta-banner">
        <h3>Ready to Hire Your Next Engineering Leader?</h3>
        <p>Book a 15-minute discovery call directly on my calendar to discuss your open roles and hiring requirements.</p>
        <div id="cta-calendar-btn" class="btn-container"></div>
    </section>

    <!-- Google Calendar Appointment Scheduling Script -->
    <script src="https://calendar.google.com/calendar/scheduling-button-script.js" async></script>
    <script>
    window.addEventListener('load', function() {
      calendar.schedulingButton.load({
        url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2tJJL-VhNXyewMBNFo0XcLn6VeQknGBfiPc5Joj9Mr7lPWmh3d1G5TF3mN2PMbFuYbR3GqDUpT?gv=true',
        color: '#d946ef',
        label: 'Book a Call',
        target: document.getElementById('nav-calendar-btn'),
      });

      calendar.schedulingButton.load({
        url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2tJJL-VhNXyewMBNFo0XcLn6VeQknGBfiPc5Joj9Mr7lPWmh3d1G5TF3mN2PMbFuYbR3GqDUpT?gv=true',
        color: '#d946ef',
        label: 'Schedule a Discovery Call',
        target: document.getElementById('hero-calendar-btn'),
      });

      calendar.schedulingButton.load({
        url: 'https://calendar.google.com/calendar/appointments/schedules/AcZssZ2tJJL-VhNXyewMBNFo0XcLn6VeQknGBfiPc5Joj9Mr7lPWmh3d1G5TF3mN2PMbFuYbR3GqDUpT?gv=true',
        color: '#d946ef',
        label: 'Book 15-Min Intro Call',
        target: document.getElementById('cta-calendar-btn'),
      });
    });
    </script>
</body>
</html>
