<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta name="description" content="Lalan Kumar - Cyber Security Expert & Ethical Hacker. Professional portfolio showcasing skills, experience, and GitHub analytics." />
    <meta name="theme-color" content="#00f5a0" />
    <title>Lalan Kumar | Cyber Security Expert & Ethical Hacker</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet"/>
    <style>
        /* ============================================================
                   ROOT VARIABLES
                   ============================================================ */
        :root {
            --primary: #00f5a0;
            --primary-dark: #00d48a;
            --primary-glow: rgba(0, 245, 160, 0.25);
            --secondary: #00d4ff;
            --secondary-glow: rgba(0, 212, 255, 0.20);
            --bg-dark: #0a0a1a;
            --bg-card: rgba(255, 255, 255, 0.04);
            --bg-card-hover: rgba(255, 255, 255, 0.07);
            --text-primary: #ffffff;
            --text-secondary: #94a3b8;
            --text-muted: #64748b;
            --border-color: rgba(255, 255, 255, 0.06);
            --border-hover: rgba(0, 245, 160, 0.20);
            --shadow-sm: 0 4px 20px rgba(0, 0, 0, 0.3);
            --shadow-md: 0 15px 50px rgba(0, 0, 0, 0.5);
            --shadow-lg: 0 25px 70px rgba(0, 0, 0, 0.6);
            --radius: 20px;
            --radius-sm: 12px;
            --transition: all 0.35s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        /* ============================================================
                   RESET & BASE
                   ============================================================ */
        *,
        *::before,
        *::after {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
            background: var(--bg-dark);
            color: var(--text-primary);
            min-height: 100vh;
            line-height: 1.7;
            background-image:
                radial-gradient(ellipse at 10% 20%, rgba(0, 245, 160, 0.06) 0%, transparent 55%),
                radial-gradient(ellipse at 90% 80%, rgba(0, 212, 255, 0.05) 0%, transparent 55%),
                radial-gradient(ellipse at 50% 50%, rgba(0, 245, 160, 0.02) 0%, transparent 70%);
            background-attachment: fixed;
        }

        /* ============================================================
                   SCROLLBAR
                   ============================================================ */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-track {
            background: var(--bg-dark);
        }
        ::-webkit-scrollbar-thumb {
            background: var(--primary);
            border-radius: 10px;
            transition: var(--transition);
        }
        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-dark);
        }

        /* ============================================================
                   UTILITY
                   ============================================================ */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 40px 24px 30px;
        }

        .glass-card {
            background: var(--bg-card);
            backdrop-filter: blur(24px) saturate(1.2);
            -webkit-backdrop-filter: blur(24px) saturate(1.2);
            border: 1px solid var(--border-color);
            border-radius: var(--radius);
            box-shadow: var(--shadow-lg);
            padding: 52px 50px 40px;
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }

        .glass-card::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle at 30% 20%, rgba(0, 245, 160, 0.03), transparent 60%);
            pointer-events: none;
        }

        .glass-card:hover {
            border-color: var(--border-hover);
            box-shadow: var(--shadow-lg), 0 0 60px rgba(0, 245, 160, 0.03);
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px 12px;
            }
            .glass-card {
                padding: 28px 18px 24px;
                border-radius: 16px;
            }
        }

        /* ============================================================
                   HEADER
                   ============================================================ */
        .header {
            text-align: center;
            padding-bottom: 38px;
            margin-bottom: 42px;
            border-bottom: 1px solid var(--border-color);
            position: relative;
        }

        .header::after {
            content: '';
            position: absolute;
            bottom: -1px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--primary), var(--secondary), transparent);
            border-radius: 10px;
        }

        .badge-top {
            display: inline-block;
            background: linear-gradient(135deg, rgba(0, 245, 160, 0.12), rgba(0, 212, 255, 0.08));
            padding: 6px 20px;
            border-radius: 50px;
            font-size: 0.7rem;
            font-weight: 700;
            letter-spacing: 1.8px;
            text-transform: uppercase;
            color: var(--primary);
            border: 1px solid rgba(0, 245, 160, 0.15);
            margin-bottom: 16px;
            backdrop-filter: blur(4px);
        }

        .header h1 {
            font-size: 4.2rem;
            font-weight: 900;
            letter-spacing: -2px;
            background: linear-gradient(135deg, #ffffff 0%, var(--primary) 45%, var(--secondary) 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 6px;
            line-height: 1.1;
        }

        .header .subtitle {
            font-size: 1.25rem;
            font-weight: 400;
            color: var(--text-secondary);
            letter-spacing: 0.2px;
        }

        .header .subtitle strong {
            color: var(--primary);
            font-weight: 600;
        }

        .header .location {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            margin-top: 12px;
            padding: 5px 18px;
            background: rgba(255, 255, 255, 0.03);
            border-radius: 50px;
            font-size: 0.8rem;
            color: var(--text-secondary);
            border: 1px solid var(--border-color);
            backdrop-filter: blur(4px);
        }

        @media (max-width: 768px) {
            .header h1 {
                font-size: 2.6rem;
                letter-spacing: -1px;
            }
            .header .subtitle {
                font-size: 1rem;
            }
        }

        @media (max-width: 480px) {
            .header h1 {
                font-size: 2rem;
            }
        }

        /* ============================================================
                   PROFILE SECTION
                   ============================================================ */
        .profile-grid {
            display: grid;
            grid-template-columns: 360px 1fr;
            gap: 48px;
            margin-bottom: 48px;
            align-items: start;
        }

        .profile-image-wrapper {
            position: relative;
            border-radius: var(--radius);
            overflow: hidden;
            border: 2px solid rgba(0, 245, 160, 0.10);
            transition: var(--transition);
            box-shadow: var(--shadow-sm);
        }

        .profile-image-wrapper:hover {
            border-color: var(--primary);
            transform: scale(1.01);
            box-shadow: 0 20px 50px rgba(0, 245, 160, 0.08);
        }

        .profile-image-wrapper img {
            width: 100%;
            height: auto;
            display: block;
            transition: var(--transition);
        }

        .profile-image-wrapper .overlay-badge {
            position: absolute;
            bottom: 18px;
            left: 18px;
            right: 18px;
            background: rgba(10, 10, 26, 0.88);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            padding: 10px 16px;
            border-radius: var(--radius-sm);
            border-left: 3px solid var(--primary);
            font-size: 0.8rem;
            font-weight: 600;
            color: var(--text-primary);
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .profile-content h2 {
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 12px;
            letter-spacing: -0.5px;
        }

        .profile-content h2 span {
            color: var(--primary);
        }

        .profile-content .bio {
            font-size: 1.05rem;
            color: var(--text-secondary);
            line-height: 1.8;
            margin-bottom: 20px;
        }

        .highlight-box {
            background: linear-gradient(135deg, rgba(0, 245, 160, 0.06), rgba(0, 212, 255, 0.03));
            padding: 16px 22px;
            border-radius: var(--radius-sm);
            border-left: 4px solid var(--primary);
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 14px;
            flex-wrap: wrap;
            backdrop-filter: blur(4px);
        }

        .highlight-box .label {
            font-weight: 700;
            color: var(--primary);
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 0.8px;
            white-space: nowrap;
        }

        .highlight-box .text {
            color: var(--text-secondary);
        }

        .highlight-box a {
            color: var(--secondary);
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            border-bottom: 1.5px solid transparent;
        }

        .highlight-box a:hover {
            color: var(--primary);
            border-bottom-color: var(--primary);
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 4px;
        }

        .tech-tags span {
            background: rgba(255, 255, 255, 0.04);
            padding: 5px 14px;
            border-radius: 50px;
            font-size: 0.75rem;
            font-weight: 500;
            color: var(--text-secondary);
            border: 1px solid var(--border-color);
            transition: var(--transition);
            cursor: default;
            backdrop-filter: blur(4px);
        }

        .tech-tags span:hover {
            border-color: var(--primary);
            color: var(--primary);
            background: rgba(0, 245, 160, 0.06);
            transform: translateY(-1px);
        }

        @media (max-width: 1024px) {
            .profile-grid {
                grid-template-columns: 1fr;
                gap: 30px;
            }
            .profile-image-wrapper {
                max-width: 400px;
                margin: 0 auto;
                width: 100%;
            }
        }

        @media (max-width: 480px) {
            .profile-image-wrapper {
                max-width: 100%;
            }
            .highlight-box {
                flex-direction: column;
                align-items: flex-start;
                gap: 6px;
            }
            .highlight-box .label {
                white-space: normal;
            }
        }

        /* ============================================================
                   STATS
                   ============================================================ */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 18px;
            margin: 36px 0 44px;
        }

        .stat-item {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: var(--radius-sm);
            padding: 20px 14px;
            text-align: center;
            transition: var(--transition);
            backdrop-filter: blur(4px);
        }

        .stat-item:hover {
            border-color: rgba(0, 245, 160, 0.20);
            transform: translateY(-4px);
            box-shadow: 0 12px 35px rgba(0, 0, 0, 0.3);
            background: var(--bg-card-hover);
        }

        .stat-item .number {
            font-size: 2.2rem;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            line-height: 1.2;
        }

        .stat-item .label {
            font-size: 0.7rem;
            color: var(--text-muted);
            text-transform: uppercase;
            letter-spacing: 0.8px;
            margin-top: 2px;
            font-weight: 500;
        }

        @media (max-width: 768px) {
            .stats-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 12px;
            }
            .stat-item .number {
                font-size: 1.6rem;
            }
            .stat-item {
                padding: 16px 10px;
            }
        }

        @media (max-width: 480px) {
            .stats-grid {
                grid-template-columns: 1fr 1fr;
                gap: 10px;
            }
            .stat-item .number {
                font-size: 1.4rem;
            }
        }

        /* ============================================================
                   SECTION TITLE
                   ============================================================ */
        .section-title {
            font-size: 1.4rem;
            font-weight: 700;
            margin-bottom: 18px;
            display: flex;
            align-items: center;
            gap: 12px;
            letter-spacing: -0.3px;
        }

        .section-title .icon {
            font-size: 1.5rem;
        }

        .section-divider {
            width: 44px;
            height: 3px;
            background: linear-gradient(90deg, var(--primary), transparent);
            border-radius: 10px;
            margin-top: -6px;
            margin-bottom: 26px;
        }

        /* ============================================================
                   SKILLS
                   ============================================================ */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 12px;
            margin-bottom: 38px;
        }

        .skill-pill {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: var(--radius-sm);
            padding: 12px 16px;
            display: flex;
            align-items: center;
            gap: 10px;
            transition: var(--transition);
            font-weight: 500;
            font-size: 0.85rem;
            color: var(--text-secondary);
            backdrop-filter: blur(4px);
        }

        .skill-pill:hover {
            border-color: var(--primary);
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0, 245, 160, 0.05);
            color: var(--text-primary);
            background: var(--bg-card-hover);
        }

        .skill-pill .emoji {
            font-size: 1.2rem;
            flex-shrink: 0;
        }

        @media (max-width: 480px) {
            .skills-grid {
                grid-template-columns: repeat(2, 1fr);
                gap: 8px;
            }
            .skill-pill {
                padding: 10px 12px;
                font-size: 0.8rem;
            }
        }

        /* ============================================================
                   GITHUB STATS
                   ============================================================ */
        .github-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 22px;
            margin-top: 8px;
        }

        .github-card {
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: var(--radius-sm);
            overflow: hidden;
            transition: var(--transition);
            backdrop-filter: blur(4px);
        }

        .github-card:hover {
            border-color: rgba(0, 245, 160, 0.18);
            transform: translateY(-3px);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.3);
            background: var(--bg-card-hover);
        }

        .github-card img {
            width: 100%;
            height: auto;
            display: block;
        }

        @media (max-width: 1024px) {
            .github-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 768px) {
            .github-grid {
                grid-template-columns: 1fr;
                gap: 16px;
            }
        }

        /* ============================================================
                   PROFILE VIEWS
                   ============================================================ */
        .views-wrapper {
            display: flex;
            justify-content: center;
            margin: 32px 0 16px;
        }

        .views-wrapper img {
            border-radius: 50px;
            padding: 4px 18px;
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            backdrop-filter: blur(4px);
            transition: var(--transition);
        }

        .views-wrapper img:hover {
            border-color: var(--border-hover);
        }

        /* ============================================================
                   SOCIAL SECTION
                   ============================================================ */
        .social-section {
            margin-top: 44px;
            padding-top: 34px;
            border-top: 1px solid var(--border-color);
            text-align: center;
        }

        .social-section .social-label {
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 1.8px;
            color: var(--text-muted);
            margin-bottom: 16px;
            font-weight: 600;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 12px;
            flex-wrap: wrap;
        }

        .social-links a {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 9px 22px;
            background: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: 50px;
            color: var(--text-secondary);
            text-decoration: none;
            font-weight: 500;
            font-size: 0.85rem;
            transition: var(--transition);
            backdrop-filter: blur(4px);
        }

        .social-links a:hover {
            background: rgba(0, 245, 160, 0.07);
            border-color: var(--primary);
            color: var(--primary);
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 245, 160, 0.06);
        }

        .social-links a .social-icon {
            font-size: 1.1rem;
        }

        @media (max-width: 768px) {
            .social-links a {
                padding: 8px 16px;
                font-size: 0.8rem;
                gap: 6px;
            }
        }

        @media (max-width: 480px) {
            .social-links a {
                width: 100%;
                justify-content: center;
            }
        }

        /* ============================================================
                   FOOTER
                   ============================================================ */
        .footer {
            text-align: center;
            margin-top: 38px;
            padding-top: 22px;
            border-top: 1px solid var(--border-color);
            color: var(--text-muted);
            font-size: 0.8rem;
            letter-spacing: 0.3px;
        }

        .footer strong {
            color: var(--primary);
            font-weight: 600;
        }

        .footer .dot {
            color: var(--text-muted);
            margin: 0 4px;
        }

        /* ============================================================
                   ANIMATIONS
                   ============================================================ */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .glass-card {
            animation: fadeInUp 0.6s ease-out forwards;
        }

        .stat-item {
            animation: fadeInUp 0.6s ease-out forwards;
            opacity: 0;
        }
        .stat-item:nth-child(1) {
            animation-delay: 0.1s;
        }
        .stat-item:nth-child(2) {
            animation-delay: 0.2s;
        }
        .stat-item:nth-child(3) {
            animation-delay: 0.3s;
        }
        .stat-item:nth-child(4) {
            animation-delay: 0.4s;
        }

        .skill-pill {
            animation: fadeInUp 0.5s ease-out forwards;
            opacity: 0;
        }
        .skill-pill:nth-child(1) {
            animation-delay: 0.05s;
        }
        .skill-pill:nth-child(2) {
            animation-delay: 0.10s;
        }
        .skill-pill:nth-child(3) {
            animation-delay: 0.15s;
        }
        .skill-pill:nth-child(4) {
            animation-delay: 0.20s;
        }
        .skill-pill:nth-child(5) {
            animation-delay: 0.25s;
        }
        .skill-pill:nth-child(6) {
            animation-delay: 0.30s;
        }
        .skill-pill:nth-child(7) {
            animation-delay: 0.35s;
        }
        .skill-pill:nth-child(8) {
            animation-delay: 0.40s;
        }

        /* ============================================================
                   PRINT STYLES
                   ============================================================ */
        @media print {
            body {
                background: #fff;
                color: #000;
            }
            .glass-card {
                background: #fff;
                border: 1px solid #ddd;
                box-shadow: none;
                backdrop-filter: none;
            }
            .glass-card::before {
                display: none;
            }
            .header h1 {
                background: none;
                -webkit-text-fill-color: #000;
                color: #000;
            }
            .stat-item .number {
                background: none;
                -webkit-text-fill-color: #000;
                color: #000;
            }
            .skill-pill,
            .tech-tags span,
            .social-links a {
                background: #f5f5f5;
                border-color: #ddd;
                color: #333;
            }
            .highlight-box {
                background: #f9f9f9;
                border-left-color: #00a86b;
            }
            .section-divider {
                background: #ccc;
            }
            .profile-image-wrapper {
                border-color: #ddd;
            }
            .github-card {
                border-color: #ddd;
            }
            .views-wrapper img {
                border-color: #ddd;
            }
            .badge-top {
                background: #f0f0f0;
                color: #00a86b;
                border-color: #ddd;
            }
            .footer {
                border-top-color: #ddd;
            }
            .social-section {
                border-top-color: #ddd;
            }
            .header {
                border-bottom-color: #ddd;
            }
            .header::after {
                background: #ccc;
            }
            .stat-item:hover,
            .skill-pill:hover,
            .github-card:hover,
            .social-links a:hover {
                transform: none !important;
                box-shadow: none !important;
            }
        }
    </style>
</head>
<body>

    <div class="container">

        <!-- ==========================================================
        MAIN GLASS CARD
        ========================================================== -->
        <div class="glass-card">

            <!-- ===== HEADER ===== -->
            <header class="header">
                <div class="badge-top">🔐 Cyber Security Professional</div>
                <h1>Lalan Kumar</h1>
                <p class="subtitle">
                    Ethical Hacker &amp; Security Trainer &middot; <strong>India</strong>
                </p>
                <div class="location">
                    <span>📍</span> India &middot; Available Worldwide
                </div>
            </header>

            <!-- ===== PROFILE ===== -->
            <div class="profile-grid">
                <div class="profile-image-wrapper">
                    <img
                        src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExdGtpNTJ1MGFncW9mN3I3anNqZ3hrMHY3Ym45eWh1NHpubnVrb243byZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/RbDKaczqWovIugyJmW/giphy.gif"
                        alt="Lalan Kumar - Cyber Security Expert"
                        loading="lazy"
                        width="600"
                        height="400"
                    />
                    <div class="overlay-badge">
                        🛡️ 5+ Years Experience
                    </div>
                </div>

                <div class="profile-content">
                    <h2>👋 Hi, I'm <span>Lalan</span></h2>
                    <p class="bio">
                        A passionate Cyber Security professional dedicated to protecting digital
                        assets and educating the next generation of security experts. I specialize
                        in ethical hacking, penetration testing, and security awareness training.
                    </p>

                    <div class="highlight-box">
                        <span class="label">🎯 Current Focus</span>
                        <span class="text">
                            Training students in Cyber Security &amp; Ethical Hacking at
                            <a href="https://chat.whatsapp.com/LfmqklX6qlK3iskbq6RtCA?mode=ems_wa_t" target="_blank" rel="noopener noreferrer">
                                Radhe Cyber Academy
                            </a>
                        </span>
                    </div>

                    <div class="tech-tags">
                        <span>🛡️ CEH Certified</span>
                        <span>🔍 Penetration Testing</span>
                        <span>🐧 Linux Security</span>
                        <span>📚 Security Trainer</span>
                        <span>🌐 Network Security</span>
                        <span>🔐 Cryptography</span>
                    </div>
                </div>
            </div>

            <!-- ===== STATS ===== -->
            <div class="stats-grid">
                <div class="stat-item">
                    <div class="number">5+</div>
                    <div class="label">Years Experience</div>
                </div>
                <div class="stat-item">
                    <div class="number">200+</div>
                    <div class="label">Students Trained</div>
                </div>
                <div class="stat-item">
                    <div class="number">50+</div>
                    <div class="label">Projects</div>
                </div>
                <div class="stat-item">
                    <div class="number">100%</div>
                    <div class="label">Commitment</div>
                </div>
            </div>

            <!-- ===== SKILLS ===== -->
            <div class="section-title">
                <span class="icon">🛠️</span> Core Competencies
            </div>
            <div class="section-divider"></div>

            <div class="skills-grid">
                <div class="skill-pill"><span class="emoji">🐧</span> Linux</div>
                <div class="skill-pill"><span class="emoji">🐍</span> Python</div>
                <div class="skill-pill"><span class="emoji">🌐</span> Network Security</div>
                <div class="skill-pill"><span class="emoji">🔐</span> Cryptography</div>
                <div class="skill-pill"><span class="emoji">🕵️</span> OSINT</div>
                <div class="skill-pill"><span class="emoji">⚡</span> Kali Linux</div>
                <div class="skill-pill"><span class="emoji">🛡️</span> Firewall &amp; IDS</div>
                <div class="skill-pill"><span class="emoji">📊</span> Risk Assessment</div>
            </div>

            <!-- ===== GITHUB STATS ===== -->
            <div class="section-title" style="margin-top:6px;">
                <span class="icon">📊</span> GitHub Analytics
            </div>
            <div class="section-divider"></div>

            <div class="github-grid">
                <div class="github-card">
                    <img
                        src="https://github-readme-stats.vercel.app/api/top-langs?username=radhacyberacademy-143&show_icons=true&locale=en&layout=compact&theme=dark&bg_color=0a0a1a&border_color=1a1a2e&title_color=00f5a0&text_color=94a3b8"
                        alt="Top Languages"
                        loading="lazy"
                        width="400"
                        height="200"
                    />
                </div>
                <div class="github-card">
                    <img
                        src="https://github-readme-stats.vercel.app/api?username=radhacyberacademy-143&show_icons=true&locale=en&theme=dark&bg_color=0a0a1a&border_color=1a1a2e&title_color=00f5a0&text_color=94a3b8&icon_color=00d4ff"
                        alt="GitHub Stats"
                        loading="lazy"
                        width="400"
                        height="200"
                    />
                </div>
                <div class="github-card">
                    <img
                        src="https://github-readme-streak-stats.herokuapp.com/?user=radhacyberacademy-143&theme=dark&background=0a0a1a&border=1a1a2e&stroke=00f5a0&ring=00f5a0&fire=00d4ff&currStreakNum=ffffff&sideNums=94a3b8&currStreakLabel=00f5a0&sideLabels=94a3b8&dates=94a3b8"
                        alt="Streak Stats"
                        loading="lazy"
                        width="400"
                        height="200"
                    />
                </div>
            </div>

            <!-- ===== PROFILE VIEWS ===== -->
            <div class="views-wrapper">
                <img
                    src="https://komarev.com/ghpvc/?username=radhacyberacademy-143&label=Profile%20Views&color=00f5a0&style=flat-square"
                    alt="Profile Views"
                    loading="lazy"
                />
            </div>

            <!-- ===== SOCIAL ===== -->
            <div class="social-section">
                <div class="social-label">🌐 Connect With Me</div>
                <div class="social-links">
                    <a href="#" target="_blank" rel="noopener noreferrer">
                        <span class="social-icon">📧</span> Email
                    </a>
                    <a href="#" target="_blank" rel="noopener noreferrer">
                        <span class="social-icon">💼</span> LinkedIn
                    </a>
                    <a href="#" target="_blank" rel="noopener noreferrer">
                        <span class="social-icon">🐦</span> Twitter
                    </a>
                    <a href="https://chat.whatsapp.com/LfmqklX6qlK3iskbq6RtCA?mode=ems_wa_t" target="_blank" rel="noopener noreferrer">
                        <span class="social-icon">💬</span> WhatsApp
                    </a>
                    <a href="#" target="_blank" rel="noopener noreferrer">
                        <span class="social-icon">🐙</span> GitHub
                    </a>
                    <a href="#" target="_blank" rel="noopener noreferrer">
                        <span class="social-icon">📺</span> YouTube
                    </a>
                </div>
            </div>

            <!-- ===== FOOTER ===== -->
            <div class="footer">
                &copy; 2026 <strong>Lalan Kumar</strong> <span class="dot">&middot;</span>
                Radhe Cyber Academy <span class="dot">&middot;</span>
                <span style="color:var(--text-secondary);">Securing Tomorrow, Today</span>
            </div>

        </div>
        <!-- ===== END GLASS CARD ===== -->

    </div>

</body>
</html>
