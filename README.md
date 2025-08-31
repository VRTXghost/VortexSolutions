<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vortex Solutions - AI Innovation & Digital Transformation</title>
    <meta name="description" content="Leading AI integration company in Cape Town. We provide workflows, app development, AI integration, and digital transformation services.">
    <meta name="keywords" content="AI, artificial intelligence, digital transformation, Cape Town, South Africa, workflows, app development">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://www.vortexsolutions.co.za/">
    <meta property="og:title" content="Vortex Solutions - AI Innovation & Digital Transformation">
    <meta property="og:description" content="Transform your business with AI. Custom solutions for the digital future.">
    <meta property="og:image" content="https://www.vortexsolutions.co.za/og-image.png">

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://www.vortexsolutions.co.za/">
    <meta property="twitter:title" content="Vortex Solutions - AI Innovation & Digital Transformation">
    <meta property="twitter:description" content="Transform your business with AI. Custom solutions for the digital future.">
    <meta property="twitter:image" content="https://www.vortexsolutions.co.za/og-image.png">
    
    <!-- Security Headers -->
    <meta http-equiv="X-Content-Type-Options" content="nosniff">
    <meta http-equiv="X-Frame-Options" content="SAMEORIGIN">
    <meta http-equiv="X-XSS-Protection" content="1; mode=block">
    <meta name="referrer" content="strict-origin-when-cross-origin">
    
    <!-- Favicon -->
    <link rel="icon" type="image/x-icon" href="favicon.ico">
    <link rel="apple-touch-icon" sizes="180x180" href="apple-touch-icon.png">
    <link rel="icon" type="image/png" sizes="32x32" href="favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="16x16" href="favicon-16x16.png">
    
    <!-- Preconnect to external resources -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    
    <!-- Google Fonts (optional - for better typography) -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --secondary: #0ea5e9;
            --dark: #0f172a;
            --light: #f8fafc;
            --gray: #64748b;
            --success: #10b981;
            --gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.6;
            color: var(--dark);
            overflow-x: hidden;
            background: var(--light);
        }

        /* Navigation */
        nav {
            position: fixed;
            width: 100%;
            top: 0;
            background: rgba(15, 23, 42, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            transition: all 0.3s ease;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: glow 3s ease-in-out infinite;
        }

        @keyframes glow {
            0%, 100% { filter: brightness(1); }
            50% { filter: brightness(1.2); }
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--light);
            text-decoration: none;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .mobile-menu-btn {
            display: none;
            background: var(--primary);
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            font-size: 1.5rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
            margin-top: 60px;
        }

        .hero-particles {
            position: absolute;
            width: 100%;
            height: 100%;
            overflow: hidden;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: var(--primary);
            border-radius: 50%;
            animation: float 20s infinite linear;
            opacity: 0.5;
        }

        @keyframes float {
            from {
                transform: translateY(100vh) translateX(0);
            }
            to {
                transform: translateY(-100vh) translateX(100px);
            }
        }

        .hero-content {
            text-align: center;
            z-index: 1;
            padding: 2rem;
            max-width: 900px;
            animation: fadeInUp 1s ease;
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

        .hero h1 {
            font-size: clamp(2.5rem, 5vw, 4rem);
            color: var(--light);
            margin-bottom: 1rem;
            font-weight: 800;
            line-height: 1.2;
        }

        .hero .tagline {
            font-size: 1.25rem;
            color: #94a3b8;
            margin-bottom: 2rem;
        }

        .cta-buttons {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn {
            padding: 1rem 2rem;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            position: relative;
            overflow: hidden;
        }

        .btn-primary {
            background: var(--gradient);
            color: white;
            box-shadow: 0 10px 30px rgba(99, 102, 241, 0.3);
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 40px rgba(99, 102, 241, 0.4);
        }

        .btn-secondary {
            background: transparent;
            color: var(--light);
            border: 2px solid var(--primary);
        }

        .btn-secondary:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }

        /* Services Section */
        .services {
            padding: 5rem 2rem;
            background: var(--light);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 1rem;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .section-subtitle {
            text-align: center;
            color: var(--gray);
            margin-bottom: 3rem;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .service-card {
            background: white;
            border-radius: 20px;
            padding: 2rem;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: var(--gradient);
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
        }

        .service-icon {
            width: 60px;
            height: 60px;
            background: var(--gradient);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 1rem;
            font-size: 1.5rem;
            color: white;
        }

        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--dark);
        }

        .service-card p {
            color: var(--gray);
            line-height: 1.8;
        }

        /* Features Section */
        .features {
            padding: 5rem 2rem;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .feature-item {
            text-align: center;
            padding: 2rem;
            background: white;
            border-radius: 15px;
            transition: transform 0.3s ease;
        }

        .feature-item:hover {
            transform: scale(1.05);
        }

        .feature-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        /* Contact Section */
        .contact {
            padding: 5rem 2rem;
            background: var(--dark);
            color: var(--light);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .contact-form {
            background: rgba(255, 255, 255, 0.05);
            padding: 2rem;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            color: #cbd5e1;
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 1rem;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            color: var(--light);
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary);
            background: rgba(255, 255, 255, 0.1);
        }

        .contact-info {
            padding: 2rem;
        }

        .contact-item {
            margin-bottom: 2rem;
            display: flex;
            align-items: center;
            gap: 1rem;
        }

        .contact-icon {
            width: 50px;
            height: 50px;
            background: var(--gradient);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            flex-shrink: 0;
        }

        /* Crypto Payment */
        .crypto-section {
            padding: 3rem 2rem;
            background: white;
            text-align: center;
        }

        .crypto-grid {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
            flex-wrap: wrap;
        }

        .crypto-item {
            padding: 1rem 2rem;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            border-radius: 50px;
            font-weight: bold;
            transition: transform 0.3s ease;
        }

        .crypto-item:hover {
            transform: scale(1.1);
        }

        /* Social Links */
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 2rem;
            justify-content: center;
        }

        .social-link {
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--light);
            text-decoration: none;
            transition: all 0.3s ease;
        }

        .social-link:hover {
            background: var(--primary);
            transform: translateY(-5px);
        }

        /* Footer */
        footer {
            background: #0a0e1a;
            color: var(--light);
            text-align: center;
            padding: 2rem;
        }

        /* Sign Up Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            z-index: 2000;
            align-items: center;
            justify-content: center;
        }

        .modal-content {
            background: white;
            padding: 2rem;
            border-radius: 20px;
            max-width: 500px;
            width: 90%;
            animation: slideIn 0.3s ease;
            max-height: 90vh;
            overflow-y: auto;
        }

        @keyframes slideIn {
            from {
                transform: translateY(-50px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        .close-modal {
            float: right;
            font-size: 2rem;
            cursor: pointer;
            color: var(--gray);
        }

        .close-modal:hover {
            color: var(--dark);
        }

        /* Security Badge */
        .security-badge {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: var(--success);
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 50px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            z-index: 100;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(16, 185, 129, 0.7); }
            70% { box-shadow: 0 0 0 10px rgba(16, 185, 129, 0); }
            100% { box-shadow: 0 0 0 0 rgba(16, 185, 129, 0); }
        }

        /* Loading Animation */
        .loading {
            display: inline-block;
            width: 20px;
            height: 20px;
            border: 3px solid rgba(255,255,255,.3);
            border-radius: 50%;
            border-top-color: white;
            animation: spin 1s ease-in-out infinite;
        }

        @keyframes spin {
            to { transform: rotate(360deg); }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2rem;
            }
            
            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .btn {
                width: 100%;
                max-width: 300px;
            }
            
            .services-grid,
            .features-grid {
                grid-template-columns: 1fr;
            }
            
            .contact-grid {
                grid-template-columns: 1fr;
            }
            
            .security-badge {
                bottom: 10px;
                right: 10px;
                font-size: 0.8rem;
            }
        }

        /* Mobile Menu */
        .mobile-menu {
            display: none;
            position: fixed;
            top: 60px;
            left: 0;
            width: 100%;
            background: rgba(15, 23, 42, 0.98);
            padding: 1rem;
            z-index: 999;
        }

        .mobile-menu.active {
            display: block;
        }

        .mobile-menu a {
            display: block;
            color: var(--light);
            text-decoration: none;
            padding: 1rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            transition: background 0.3s ease;
        }

        .mobile-menu a:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        /* Accessibility */
        .sr-only {
            position: absolute;
            width: 1px;
            height: 1px;
            padding: 0;
            margin: -1px;
            overflow: hidden;
            clip: rect(0, 0, 0, 0);
            white-space: nowrap;
            border-width: 0;
        }

        /* Print Styles */
        @media print {
            nav, .security-badge, .modal {
                display: none;
            }
            
            body {
                color: black;
                background: white;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav id="navbar" role="navigation">
        <div class="nav-container">
            <div class="logo">VORTEX SOLUTIONS</div>
            <button class="mobile-menu-btn" id="mobileMenuBtn" aria-label="Toggle mobile menu">☰</button>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
        <div class="mobile-menu" id="mobileMenu">
            <a href="#home">Home</a>
            <a href="#services">Services</a>
            <a href="#features">Features</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-particles" id="particles"></div>
        <div class="hero-content">
            <h1>Welcome to the AI Revolution</h1>
            <p class="tagline">We don't use AI for replacement, we use AI for improvement</p>
            <p style="color: #94a3b8; margin-bottom: 2rem;">Transform your business with cutting-edge AI solutions tailored to your needs. Based in Cape Town, serving the world.</p>
            <div class="cta-buttons">
                <button class="btn btn-primary" onclick="openSignUp()">Get Started Today</button>
                <a href="#contact" class="btn btn-secondary">Schedule Consultation</a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <h2 class="section-title">Our Services</h2>
            <p class="section-subtitle">Comprehensive AI solutions to accelerate your digital transformation</p>
            
            <div class="services-grid">
                <article class="service-card">
                    <div class="service-icon">🤖</div>
                    <h3>AI Integration</h3>
                    <p>Seamlessly integrate AI into your existing systems and workflows. We ensure smooth adoption without disrupting your operations.</p>
                </article>
                
                <article class="service-card">
                    <div class="service-icon">⚡</div>
                    <h3>Workflow Automation</h3>
                    <p>Automate repetitive tasks and optimize business processes with intelligent workflows that save time and reduce errors.</p>
                </article>
                
                <article class="service-card">
                    <div class="service-icon">💻</div>
                    <h3>App Development</h3>
                    <p>Custom AI-powered applications built to solve your specific business challenges and drive innovation.</p>
                </article>
                
                <article class="service-card">
                    <div class="service-icon">🌐</div>
                    <h3>AI Websites</h3>
                    <p>Modern, intelligent websites with AI features, complete with hosting and ongoing maintenance.</p>
                </article>
                
                <article class="service-card">
                    <div class="service-icon">🚀</div>
                    <h3>Digital Transformation</h3>
                    <p>Complete digital makeover for your business, ensuring you stay ahead in the AI-driven future.</p>
                </article>
                
                <article class="service-card">
                    <div class="service-icon">👥</div>
                    <h3>AI Consulting</h3>
                    <p>Expert guidance on AI strategy, implementation, and best practices tailored to your industry.</p>
                </article>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features" id="features">
        <div class="container">
            <h2 class="section-title">Why Choose Vortex Solutions?</h2>
            <p class="section-subtitle">Leading the way in AI innovation</p>
            
            <div class="features-grid">
                <article class="feature-item">
                    <div class="feature-icon">🛡️</div>
                    <h3>Enterprise Security</h3>
                    <p>Military-grade encryption and DDoS protection for all solutions</p>
                </article>
                
                <article class="feature-item">
                    <div class="feature-icon">⚡</div>
                    <h3>Lightning Fast</h3>
                    <p>AI-optimized performance that delivers results in milliseconds</p>
                </article>
                
                <article class="feature-item">
                    <div class="feature-icon">🎯</div>
                    <h3>Tailored Solutions</h3>
                    <p>Custom-built for your specific needs and goals</p>
                </article>
                
                <article class="feature-item">
                    <div class="feature-icon">🌍</div>
                    <h3>Global Reach</h3>
                    <p>In-person or virtual meetings, wherever you are</p>
                </article>
            </div>
        </div>
    </section>

    <!-- Crypto Payment Section -->
    <section class="crypto-section">
        <div class="container">
            <h2 class="section-title">We Accept Crypto Payments</h2>
            <p class="section-subtitle">Future-ready payment solutions for future-ready businesses</p>
            <div class="crypto-grid">
                <div class="crypto-item">BTC</div>
                <div class="crypto-item">ETH</div>
                <div class="crypto-item">USDC</div>
                <div class="crypto-item">XRP</div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <h2 class="section-title" style="color: white;">Get In Touch</h2>
            <p class="section-subtitle" style="color: #94a3b8;">Ready to transform your business with AI?</p>
            
            <div class="contact-grid">
                <div class="contact-form">
                    <h3 style="margin-bottom: 1.5rem;">Send us a message</h3>
                    <form id="contactForm" action="#" method="POST">
                        <div class="form-group">
                            <label for="name">Your Name</label>
                            <input type="text" id="name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email">Email Address</label>
                            <input type="email" id="email" name="email" required>
                        </div>
                        <div class="form-group">
                            <label for="company">Company</label>
                            <input type="text" id="company" name="company">
                        </div>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" name="message" rows="5" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary" style="width: 100%;">Send Message</button>
                    </form>
                </div>
                
                <div class="contact-info">
                    <h3 style="margin-bottom: 2rem;">Contact Information</h3>
                    
                    <div class="contact-item">
                        <div class="contact-icon">📧</div>
                        <div>
                            <h4>Email</h4>
                            <p><a href="mailto:info@vortexsolutions.co.za" style="color: inherit; text-decoration: none;">info@vortexsolutions.co.za</a></p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">📍</div>
                        <div>
                            <h4>Location</h4>
                            <p>Cape Town, Western Cape<br>South Africa</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">💬</div>
                        <div>
                            <h4>WhatsApp</h4>
                            <p>Coming Soon</p>
                        </div>
                    </div>
                    
                    <div class="social-links">
                        <a href="https://linkedin.com" class="social-link" title="LinkedIn" target="_blank" rel="noopener noreferrer">in</a>
                        <a href="https://x.com" class="social-link" title="X (Twitter)" target="_blank" rel="noopener noreferrer">X</a>
                        <a href="https://facebook.com" class="social-link" title="Facebook" target="_blank" rel="noopener noreferrer">f</a>
                        <a href="https://instagram.com" class="social-link" title="Instagram" target="_blank" rel="noopener noreferrer">ig</a>
                        <a href="https://tiktok.com" class="social-link" title="TikTok" target="_blank" rel="noopener noreferrer">TT</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; <span id="currentYear">2024</span> Vortex Solutions. All rights reserved.</p>
        <p>Empowering businesses with AI innovation</p>
    </footer>

    <!-- Sign Up Modal -->
    <div id="signupModal" class="modal" role="dialog" aria-labelledby="signupTitle" aria-hidden="true">
        <div class="modal-content">
            <span class="close-modal" onclick="closeSignUp()" aria-label="Close modal">&times;</span>
            <h2 id="signupTitle" style="margin-bottom: 1.5rem; background: var(--gradient); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">Start Your AI Journey</h2>
            <form id="signupForm" action="#" method="POST">
                <div class="form-group">
                
