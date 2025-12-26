<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Norify | Digital Marketing Specialist | ROI-Focused Marketing</title>
    <meta name="description" content="Transform your business with data-driven digital marketing. Proven results: 4.5x ROAS, 40% CAC reduction, 200% traffic growth.">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.7;
            color: #1a1a1a;
            background: #0f0f0f;
            overflow-x: hidden;
        }

        .bg-gradient {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 25%, #f093fb 50%, #4facfe 75%, #00f2fe 100%);
            background-size: 400% 400%;
            animation: gradientShift 15s ease infinite;
            opacity: 0.1;
            z-index: -1;
        }

        @keyframes gradientShift {
            0%, 100% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 40px;
        }

        nav {
            background: rgba(15, 15, 15, 0.95);
            backdrop-filter: blur(20px);
            padding: 1.5rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.3);
        }

        nav .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 800;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            letter-spacing: -1px;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 3rem;
            align-items: center;
        }

        nav a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s;
            position: relative;
        }

        nav a:hover {
            color: #fff;
        }

        nav a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            transition: width 0.3s;
        }

        nav a:hover::after {
            width: 100%;
        }

        .nav-cta {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            padding: 0.7rem 1.8rem;
            border-radius: 50px;
            color: #fff !important;
            font-weight: 600;
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
            transition: all 0.3s;
        }

        .nav-cta:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 30px rgba(102, 126, 234, 0.6);
        }

        .nav-cta::after {
            display: none;
        }

        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            background: linear-gradient(135deg, #0f0f0f 0%, #1a1a2e 50%, #16213e 100%);
            position: relative;
            overflow: hidden;
            padding-top: 80px;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(circle at 20% 50%, rgba(102, 126, 234, 0.1) 0%, transparent 50%),
                        radial-gradient(circle at 80% 80%, rgba(118, 75, 162, 0.1) 0%, transparent 50%);
        }

        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 900px;
        }

        .hero-badge {
            display: inline-block;
            background: rgba(102, 126, 234, 0.1);
            border: 1px solid rgba(102, 126, 234, 0.3);
            padding: 0.6rem 1.5rem;
            border-radius: 50px;
            color: #667eea;
            font-weight: 600;
            font-size: 0.9rem;
            margin-bottom: 2rem;
            animation: fadeInUp 0.8s;
        }

        .hero h1 {
            font-size: 5rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 1.5rem;
            background: linear-gradient(135deg, #fff 0%, #667eea 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: fadeInUp 1s;
        }

        .hero-highlight {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero p {
            font-size: 1.4rem;
            color: rgba(255, 255, 255, 0.7);
            margin-bottom: 3rem;
            line-height: 1.8;
            animation: fadeInUp 1.2s;
        }

        .hero-stats {
            display: flex;
            gap: 4rem;
            margin-bottom: 3rem;
            animation: fadeInUp 1.4s;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 3rem;
            font-weight: 800;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            display: block;
        }

        .stat-label {
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.9rem;
            margin-top: 0.5rem;
        }

        .cta-buttons {
            display: flex;
            gap: 1.5rem;
            animation: fadeInUp 1.6s;
        }

        .btn {
            padding: 1.2rem 2.5rem;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            text-decoration: none;
            display: inline-block;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            cursor: pointer;
            border: none;
        }

        .btn-primary {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            box-shadow: 0 10px 40px rgba(102, 126, 234, 0.4);
        }

        .btn-primary:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 50px rgba(102, 126, 234, 0.6);
        }

        .btn-secondary {
            background: rgba(255, 255, 255, 0.05);
            color: #fff;
            border: 2px solid rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(10px);
        }

        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.1);
            border-color: rgba(255, 255, 255, 0.4);
            transform: translateY(-5px);
        }

        .trust-badges {
            display: flex;
            gap: 3rem;
            margin-top: 4rem;
            flex-wrap: wrap;
            animation: fadeInUp 1.8s;
        }

        .badge-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            background: rgba(255, 255, 255, 0.03);
            padding: 1rem 1.5rem;
            border-radius: 15px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }

        .badge-icon {
            font-size: 2rem;
        }

        .badge-text {
            color: rgba(255, 255, 255, 0.9);
            font-weight: 600;
            font-size: 0.95rem;
        }

        section {
            padding: 120px 0;
            position: relative;
        }

        .section-header {
            text-align: center;
            margin-bottom: 80px;
        }

        .section-badge {
            display: inline-block;
            background: rgba(102, 126, 234, 0.1);
            border: 1px solid rgba(102, 126, 234, 0.3);
            padding: 0.5rem 1.2rem;
            border-radius: 50px;
            color: #667eea;
            font-weight: 600;
            font-size: 0.85rem;
            margin-bottom: 1rem;
        }

        .section-title {
            font-size: 3.5rem;
            font-weight: 800;
            color: #fff;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }

        .section-subtitle {
            font-size: 1.3rem;
            color: rgba(255, 255, 255, 0.6);
            max-width: 700px;
            margin: 0 auto;
        }

        #services {
            background: #0f0f0f;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2.5rem;
        }

        .service-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(20px);
            padding: 3rem;
            border-radius: 25px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2);
            opacity: 0;
            transition: opacity 0.3s;
        }

        .service-card:hover::before {
            opacity: 1;
        }

        .service-card:hover {
            transform: translateY(-15px);
            border-color: rgba(102, 126, 234, 0.5);
            box-shadow: 0 20px 60px rgba(102, 126, 234, 0.3);
        }

        .service-icon {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
        }

        .service-card h3 {
            color: #fff;
            font-size: 1.6rem;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .service-card p {
            color: rgba(255, 255, 255, 0.6);
            margin-bottom: 1.5rem;
            line-height: 1.7;
        }

        .service-card ul {
            list-style: none;
            margin-bottom: 1.5rem;
        }

        .service-card li {
            color: rgba(255, 255, 255, 0.7);
            padding: 0.5rem 0;
            padding-left: 1.5rem;
            position: relative;
        }

        .service-card li::before {
            content: '→';
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
        }

        .service-metric {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.2) 0%, rgba(118, 75, 162, 0.2) 100%);
            padding: 0.8rem 1.5rem;
            border-radius: 50px;
            display: inline-block;
            color: #fff;
            font-weight: 700;
            font-size: 0.95rem;
        }

        #portfolio {
            background: linear-gradient(180deg, #0f0f0f 0%, #1a1a2e 100%);
        }

        .case-study {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(20px);
            border-radius: 30px;
            padding: 4rem;
            margin-bottom: 3rem;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.5s;
            position: relative;
            overflow: hidden;
        }

        .case-study::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            bottom: 0;
            width: 6px;
            background: linear-gradient(180deg, #667eea, #764ba2);
        }

        .case-study:hover {
            border-color: rgba(102, 126, 234, 0.5);
            transform: translateX(10px);
        }

        .case-study h3 {
            font-size: 2rem;
            color: #fff;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .case-meta {
            color: rgba(255, 255, 255, 0.5);
            margin-bottom: 2rem;
            font-style: italic;
        }

        .case-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            margin-top: 2rem;
        }

        .case-content h4 {
            color: #fff;
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .case-content p {
            color: rgba(255, 255, 255, 0.7);
            line-height: 1.8;
        }

        .results-box {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.1) 0%, rgba(118, 75, 162, 0.1) 100%);
            padding: 2.5rem;
            border-radius: 20px;
            border: 1px solid rgba(102, 126, 234, 0.3);
        }

        .result-item {
            display: flex;
            align-items: center;
            gap: 1.5rem;
            margin: 1.5rem 0;
        }

        .result-number {
            font-size: 3rem;
            font-weight: 800;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .result-text {
            color: rgba(255, 255, 255, 0.9);
            line-height: 1.5;
        }

        .tools-used {
            display: flex;
            flex-wrap: wrap;
            gap: 0.8rem;
            margin-top: 2rem;
        }

        .tool-tag {
            background: rgba(102, 126, 234, 0.2);
            color: #fff;
            padding: 0.6rem 1.2rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 600;
            border: 1px solid rgba(102, 126, 234, 0.3);
        }

        #pricing {
            background: #0f0f0f;
        }

        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .pricing-card {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(20px);
            padding: 3rem;
            border-radius: 25px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            position: relative;
        }

        .pricing-card.featured {
            background: linear-gradient(135deg, rgba(102, 126, 234, 0.15) 0%, rgba(118, 75, 162, 0.15) 100%);
            border: 2px solid rgba(102, 126, 234, 0.5);
            transform: scale(1.05);
        }

        .pricing-badge {
            position: absolute;
            top: -15px;
            right: 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            padding: 0.5rem 1.5rem;
            border-radius: 50px;
            font-size: 0.85rem;
            font-weight: 700;
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
        }

        .pricing-card:hover {
            transform: translateY(-15px) scale(1.02);
            border-color: rgba(102, 126, 234, 0.5);
        }

        .pricing-card h3 {
            color: #fff;
            font-size: 1.8rem;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .price {
            font-size: 4rem;
            font-weight: 800;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin: 1.5rem 0;
        }

        .price-period {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.5);
            font-weight: 400;
        }

        .pricing-card ul {
            list-style: none;
            margin: 2rem 0;
        }

        .pricing-card li {
            color: rgba(255, 255, 255, 0.8);
            padding: 1rem 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            padding-left: 1.8rem;
            position: relative;
        }

        .pricing-card li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: #667eea;
            font-weight: bold;
            font-size: 1.2rem;
        }

        #contact {
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
        }

        .contact-container {
            max-width: 700px;
            margin: 0 auto;
        }

        .contact-form {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(20px);
            padding: 4rem;
            border-radius: 30px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .form-group {
            margin-bottom: 2rem;
        }

        .form-group label {
            display: block;
            color: rgba(255, 255, 255, 0.9);
            margin-bottom: 0.8rem;
            font-weight: 600;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 1.2rem;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            color: #fff;
            font-size: 1rem;
            transition: all 0.3s;
            font-family: 'Inter', sans-serif;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: rgba(102, 126, 234, 0.5);
            background: rgba(255, 255, 255, 0.08);
        }

        .form-group textarea {
            resize: vertical;
            min-height: 150px;
        }

        .contact-info {
            text-align: center;
            margin-top: 3rem;
            padding-top: 3rem;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }

        .contact-info p {
            color: rgba(255, 255, 255, 0.7);
            margin: 1rem 0;
            font-size: 1.1rem;
        }

        .contact-info a {
            color: #667eea;
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }

        .contact-info a:hover {
            color: #764ba2;
        }

        footer {
            background: #0a0a0a;
            padding: 3rem 0;
            text-align: center;
            border-top: 1px solid rgba(255, 255, 255, 0.05);
        }

        footer p {
            color: rgba(255, 255, 255, 0.5);
            margin: 0.5rem 0;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(40px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .scroll-animate {
            opacity: 0;
            transform: translateY(40px);
            transition: all 0.8s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }

        .scroll-animate.active {
            opacity: 1;
            transform: translateY(0);
        }

        @media (max-width: 1200px) {
            .services-grid,
            .pricing-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }

        @media (max-width: 768px) {
            .container {
                padding: 0 20px;
            }

            .hero h1 {
                font-size: 3rem;
            }

            .hero p {
                font-size: 1.1rem;
            }

            .hero-stats {
                flex-wrap: wrap;
                gap: 2rem;
            }

            .services-grid,
            .pricing-grid {
                grid-template-columns: 1fr;
            }

            .case-content {
                grid-template-columns: 1fr;
            }

            .section-title {
                font-size: 2.5rem;
            }

            nav ul {
                display: none;
            }

            .cta-buttons {
                flex-direction: column;
            }

            .trust-badges {
                flex-direction: column;
                gap: 1rem;
            }
        }
    </style>
</head>
<body>
    <div class="bg-gradient"></div>

    <nav>
        <div class="container">
            <div class="logo">Norify</div>
            <ul>
                <li><a href="#services">Services</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="#contact" class="nav-cta">Get Started</a></li>
            </ul>
        </div>
    </nav>

    <section class="hero">
        <div class="container">
            <div class="hero-content">
                <span class="hero-badge">🚀 Available for Projects</span>
                <h1>
                    Transform Your Business<br>
                    With <span class="hero-highlight">Data-Driven</span><br>
                    Digital Marketing
                </h1>
                <p>
                    We help US businesses achieve measurable growth through ROI-focused SEO, paid advertising, and AI-powered marketing strategies. Real results, not just promises.
                </p>

                <div class="hero-stats">
                    <div class="stat">
                        <span class="stat-number">4.5x</span>
                        <span class="stat-label">Average ROAS</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">40%</span>
                        <span class="stat-label">CAC Reduction</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">200%</span>
                        <span class="stat-label">Traffic Growth</span>
                    </div>
                </div>

                <div class="cta-buttons">
                    <a href="#contact" class="btn btn-primary">Start Your Project</a>
                    <a href="#portfolio" class="btn btn-secondary">View Case Studies</a>
                </div>

                <div class="trust-badges">
                    <div class="badge-item">
                        <span class="badge-icon">🎯</span>
                        <span class="badge-text">Google Certified</span>
                    </div>
                    <div class="badge-item">
                        <span class="badge-icon">📱</span>
                        <span class="badge-text">Meta Blueprint</span>
                    </div>
                    <div class="badge-item">
                        <span class="badge-icon">📊</span>
                        <span class="badge-text">HubSpot Certified</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="services">
        <div class="container">
            <div class="section-header scroll-animate">
                <span class="section-badge">WHAT WE DO</span>
                <h2 class="section-title">Services That Drive Revenue</h2>
                <p class="section-subtitle">
                    Comprehensive digital marketing solutions designed to deliver measurable business growth and exceptional ROI.
                </p>
            </div>

            <div class="services-grid">
                <div class="service-card scroll-animate">
                    <div class="service-icon">🎯</div>
                    <h3>SEO & Content Strategy</h3>
                    <p>Dominate search results and attract high-quality organic traffic that converts.</p>
                    <ul>
                        <li>Technical & on-page optimization</li>
                        <li>Strategic keyword research</li>
                        <li>Content creation & optimization</li>
                        <li>Competitor analysis</li>
                    </ul>
                    <span class="service-metric">50-200% Traffic Growth</span>
                </div>

                <div class="service-card scroll-animate">
                    <div class="service-icon">💰</div>
                    <h3>Paid Advertising</h3>
                    <p>Scale profitably with expertly managed Google Ads and Meta campaigns.</p>
                    <ul>
                        <li>Google Ads (Search & Display)</li>
                        <li>Facebook & Instagram Ads</li>
                        <li>Advanced A/B testing</li>
                        <li>Conversion optimization</li>
                    </ul>
                    <span class="service-metric">3-5x Average ROAS</span>
                </div>

                <div class="service-card scroll-animate">
                    <div class="service-icon">📊</div>
                    <h3>Marketing Analytics</h3>
                    <p>Make data-driven decisions with comprehensive tracking and insights.</p>
                    <ul>
                        <li>Google Analytics 4 setup</li>
                        <li>Custom dashboards</li>
                        <li>Performance tracking</li>
                        <li>ROI analysis</li>
                    </ul>
                    <span class="service-metric">Real-Time Insights</span>
                </div>

                <div class="service-card scroll-animate">
                    <div class="service-icon">🤖</div>
                    <h3>AI-Powered Marketing</h3>
                    <p>Leverage cutting-edge AI tools for efficiency and superior results.</p>
                    <ul>
                        <li>ChatGPT & Jasper.ai content</li>
                        <li>AdCreative.ai designs</li>
                        <li>Marketing automation</li>
                        <li>Workflow optimization</li>
                    </ul>
                    <span
