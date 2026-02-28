<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Агриппина Валерьевна Келиоус — Профессиональная няня в Санкт-Петербурге</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #2d3436;
            --secondary: #e17055;
            --accent: #fdcb6e;
            --light: #f8f9fa;
            --text: #2d3436;
            --gradient-1: #ff9a9e;
            --gradient-2: #fecfef;
            --gradient-3: #fecfef;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text);
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            overflow-x: hidden;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Hero Section */
        .hero {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 30px;
            padding: 60px 40px;
            margin-bottom: 40px;
            box-shadow: 0 25px 80px rgba(0,0,0,0.3);
            text-align: center;
            position: relative;
            overflow: hidden;
            animation: fadeInUp 1s ease-out;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 6px;
            background: linear-gradient(90deg, var(--secondary), var(--accent), #00b894, var(--secondary));
            background-size: 300% 100%;
            animation: gradientShift 3s ease infinite;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .hero-badge {
            display: inline-block;
            background: linear-gradient(135deg, var(--secondary), #e84393);
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            font-size: 1em;
            font-weight: 700;
            margin-bottom: 30px;
            box-shadow: 0 10px 30px rgba(225, 112, 85, 0.4);
            text-transform: uppercase;
            letter-spacing: 2px;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.05); }
        }

        h1 {
            font-size: 3em;
            color: var(--primary);
            margin-bottom: 15px;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary), #636e72);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .subtitle {
            font-size: 1.5em;
            color: #636e72;
            font-weight: 300;
            margin-bottom: 20px;
        }

        .availability-hero {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: #00b894;
            color: white;
            padding: 15px 30px;
            border-radius: 50px;
            font-size: 1.1em;
            font-weight: 600;
            margin-top: 20px;
            box-shadow: 0 10px 30px rgba(0, 184, 148, 0.4);
        }

        .live-indicator {
            width: 12px;
            height: 12px;
            background: #fff;
            border-radius: 50%;
            animation: blink 1.5s infinite;
        }

        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.3; }
        }

        /* Main Grid */
        .main-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-bottom: 40px;
        }

        @media (max-width: 768px) {
            .main-grid {
                grid-template-columns: 1fr;
            }
            h1 { font-size: 2em; }
        }

        /* Cards */
        .card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.2);
            transition: all 0.4s ease;
            animation: fadeInUp 1s ease-out 0.2s both;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 30px 80px rgba(0,0,0,0.3);
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Profile Section */
        .profile-section {
            text-align: center;
            position: relative;
        }

        .profile-image-container {
            position: relative;
            width: 280px;
            height: 280px;
            margin: 0 auto 30px;
        }

        .profile-image {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: cover;
            border: 8px solid white;
            box-shadow: 0 15px 50px rgba(0,0,0,0.3);
            transition: all 0.4s ease;
        }

        .profile-image:hover {
            transform: scale(1.05) rotate(2deg);
        }

        .experience-badge {
            position: absolute;
            bottom: 10px;
            right: 10px;
            background: var(--secondary);
            color: white;
            width: 80px;
            height: 80px;
            border-radius: 50%;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
            border: 4px solid white;
        }

        .experience-badge span {
            font-size: 1.5em;
            line-height: 1;
        }

        .experience-badge small {
            font-size: 0.7em;
            text-transform: uppercase;
        }

        /* Info Grid */
        .info-title {
            font-size: 1.8em;
            color: var(--primary);
            margin-bottom: 25px;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .info-list {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .info-item {
            display: flex;
            align-items: center;
            gap: 20px;
            padding: 20px;
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            border-radius: 15px;
            border-left: 5px solid var(--secondary);
            transition: all 0.3s ease;
        }

        .info-item:hover {
            transform: translateX(10px);
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .info-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--secondary), #e84393);
            color: white;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5em;
            flex-shrink: 0;
        }

        .info-content h4 {
            color: #636e72;
            font-size: 0.9em;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 5px;
        }

        .info-content p {
            color: var(--primary);
            font-size: 1.2em;
            font-weight: 700;
        }

        .age-highlight {
            display: inline-block;
            background: var(--accent);
            color: var(--primary);
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.8em;
            margin-left: 10px;
        }

        /* Features Section */
        .features-section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 50px;
            margin-bottom: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.2);
            animation: fadeInUp 1s ease-out 0.4s both;
        }

        .section-header {
            text-align: center;
            margin-bottom: 40px;
        }

        .section-title {
            font-size: 2.2em;
            color: var(--primary);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
            border-radius: 2px;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .feature-card {
            background: white;
            padding: 30px;
            border-radius: 20px;
            text-align: center;
            transition: all 0.4s ease;
            border: 2px solid transparent;
            position: relative;
            overflow: hidden;
        }

        .feature-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--secondary), var(--accent));
            transform: scaleX(0);
            transition: transform 0.4s ease;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0,0,0,0.1);
            border-color: var(--accent);
        }

        .feature-card:hover::before {
            transform: scaleX(1);
        }

        .feature-icon {
            font-size: 3em;
            margin-bottom: 20px;
            display: inline-block;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .feature-card h3 {
            color: var(--primary);
            font-size: 1.3em;
            margin-bottom: 10px;
        }

        .feature-card p {
            color: #636e72;
            line-height: 1.6;
        }

        /* Gallery Section */
        .gallery-section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 50px;
            margin-bottom: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.2);
            animation: fadeInUp 1s ease-out 0.6s both;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .gallery-item {
            position: relative;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            aspect-ratio: 4/3;
            cursor: pointer;
            transition: all 0.4s ease;
        }

        .gallery-item:hover {
            transform: scale(1.02);
            box-shadow: 0 20px 50px rgba(0,0,0,0.3);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.6s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.15);
        }

        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
            padding: 30px;
            color: white;
            transform: translateY(100%);
            transition: transform 0.4s ease;
        }

        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }

        .gallery-overlay h3 {
            font-size: 1.3em;
            margin-bottom: 8px;
        }

        /* Contact Section */
        .contact-section {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 25px;
            padding: 50px;
            margin-bottom: 40px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.2);
            text-align: center;
            animation: fadeInUp 1s ease-out 0.8s both;
        }

        .contact-intro {
            font-size: 1.2em;
            color: #636e72;
            margin-bottom: 10px;
        }

        .contact-promise {
            color: var(--secondary);
            font-weight: 600;
            margin-bottom: 40px;
            font-size: 1.1em;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .contact-card {
            display: flex;
            align-items: center;
            gap: 15px;
            padding: 25px;
            border-radius: 15px;
            text-decoration: none;
            color: white;
            font-weight: 600;
            transition: all 0.4s ease;
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .contact-card:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0,0,0,0.3);
        }

        .contact-icon {
            font-size: 2em;
        }

        .contact-info {
            text-align: left;
        }

        .contact-label {
            font-size: 0.9em;
            opacity: 0.9;
            margin-bottom: 5px;
        }

        .contact-value {
            font-size: 1.2em;
            font-weight: 700;
        }

        .telegram {
            background: linear-gradient(135deg, #0088cc, #00aced);
        }

        .whatsapp {
            background: linear-gradient(135deg, #25d366, #128c7e);
        }

        .phone {
            background: linear-gradient(135deg, #e17055, #d63031);
        }

        .direct-call {
            background: linear-gradient(135deg, #f8f9fa, #e9ecef);
            padding: 30px;
            border-radius: 20px;
            margin-top: 20px;
        }

        .direct-call h3 {
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 1.3em;
        }

        .phone-number {
            font-size: 2em;
            color: var(--secondary);
            font-weight: 800;
            text-decoration: none;
            display: inline-block;
            transition: all 0.3s ease;
        }

        .phone-number:hover {
            transform: scale(1.1);
            color: #e84393;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px;
            color: white;
            animation: fadeInUp 1s ease-out 1s both;
        }

        .footer-content {
            background: rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            padding: 30px;
            border-radius: 20px;
            margin-bottom: 20px;
        }

        .heart {
            color: #ff6b6b;
            display: inline-block;
            animation: heartbeat 1.5s ease-in-out infinite;
        }

        @keyframes heartbeat {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.2); }
        }

        .location-tag {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: rgba(255,255,255,0.2);
            padding: 10px 25px;
            border-radius: 50px;
            margin-top: 15px;
            font-weight: 600;
        }

        /* Scroll animations */
        .scroll-reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease;
        }

        .scroll-reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hero Section -->
        <header class="hero">
            <div class="hero-badge">⭐ Профессиональная няня</div>
            <h1>Агриппина Валерьевна Келиоус</h1>
            <p class="subtitle">Забота и любовь к вашим детям с 2014 года</p>
            <div class="availability-hero">
                <span class="live-indicator"></span>
                <span>Доступна 7/7 — 24/24</span>
            </div>
        </header>

        <!-- Main Info Grid -->
        <div class="main-grid">
            <!-- Profile Card -->
            <div class="card profile-section">
                <div class="profile-image-container">
                    <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?w=400&h=400&fit=crop" alt="Агриппина Валерьевна" class="profile-image">
                    <div class="experience-badge">
                        <span>10+</span>
                        <small>лет</small>
                    </div>
                </div>
                <h2 style="color: var(--primary); margin-bottom: 15px; font-size: 1.8em;">Ваш надежный помощник</h2>
                <p style="color: #636e72; line-height: 1.8; font-size: 1.1em;">
                    Добросовестная няня с медицинской подготовкой и всеми необходимыми сертификатами. 
                    Создаю безопасную, развивающую и любящую среду для детей с самого рождения.
                </p>
                <div style="margin-top: 25px; display: flex; gap: 10px; justify-content: center; flex-wrap: wrap;">
                    <span style="background: #e8f5e9; color: #2e7d32; padding: 8px 16px; border-radius: 20px; font-size: 0.9em; font-weight: 600;">✓ Мед. книжка</span>
                    <span style="background: #e3f2fd; color: #1565c0; padding: 8px 16px; border-radius: 20px; font-size: 0.9em; font-weight: 600;">✓ Рекомендации</span>
                    <span style="background: #fff3e0; color: #ef6c00; padding: 8px 16px; border-radius: 20px; font-size: 0.9em; font-weight: 600;">✓ Педагогическое образование</span>
                </div>
            </div>

            <!-- Details Card -->
            <div class="card">
                <h2 class="info-title">
                    <span>📋</span>
                    Информация о специалисте
                </h2>
                <div class="info-list">
                    <div class="info-item">
                        <div class="info-icon">👩</div>
                        <div class="info-content">
                            <h4>Возраст</h4>
                            <p>35 лет <span class="age-highlight">Зрелый специалист</span></p>
                        </div>
                    </div>

                    <div class="info-item">
                        <div class="info-icon">📍</div>
                        <div class="info-content">
                            <h4>Локация</h4>
                            <p>Санкт-Петербург, Россия</p>
                        </div>
                    </div>

                    <div class="info-item">
                        <div class="info-icon">📜</div>
                        <div class="info-content">
                            <h4>Опыт работы</h4>
                            <p>Более 10 лет с сертификатами</p>
                        </div>
                    </div>

                    <div class="info-item">
                        <div class="info-icon">👶</div>
                        <div class="info-content">
       
