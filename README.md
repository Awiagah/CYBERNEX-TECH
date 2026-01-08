<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Awiagah Ajapa Timothy | IT Specialist & Cybersecurity</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Roboto+Slab:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #1a237e;
            --primary-light: #534bae;
            --primary-dark: #000051;
            --secondary: #00bcd4;
            --secondary-light: #62efff;
            --secondary-dark: #008ba3;
            --accent: #ff4081;
            --light: #f5f7fa;
            --dark: #263238;
            --gray: #607d8b;
            --success: #4caf50;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: var(--light);
        }

        h1, h2, h3, h4 {
            font-family: 'Roboto Slab', serif;
            font-weight: 600;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        h1 {
            font-size: 2.8rem;
            line-height: 1.2;
        }

        h2 {
            font-size: 2.2rem;
            position: relative;
            padding-bottom: 0.5rem;
            margin-bottom: 2rem;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 70px;
            height: 4px;
            background: var(--secondary);
        }

        p {
            margin-bottom: 1.2rem;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        .section {
            padding: 80px 0;
        }

        .section-light {
            background-color: white;
        }

        .btn {
            display: inline-block;
            padding: 12px 30px;
            background: var(--primary);
            color: white;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        .btn-secondary {
            background: var(--secondary);
        }

        .btn-secondary:hover {
            background: var(--secondary-dark);
        }

        .btn-accent {
            background: var(--accent);
        }

        .btn-accent:hover {
            background: #e91e63;
        }

        /* Header & Navigation */
        header {
            background-color: white;
            box-shadow: var(--shadow);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            height: 50px;
            width: 50px;
            border-radius: 50%;
        }

        .logo-img {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
        }

        .logo-text {
            font-family: 'Roboto Slab', serif;
            font-weight: 700;
            font-size: 1.5rem;
            font-weight: 900; font-size: 1.5rem; letter-spacing: -1px; background: linear-gradient(to right, #ff0050, #00f2ea); -webkit-background-clip: text; -webkit-text-fill-color: transparent;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 500;
            transition: var(--transition);
        }

        .nav-links a:hover {
            color: var(--secondary);
        }

        .mobile-menu-btn {
            display: none;
            font-size: 1.5rem;
            background: none;
            border: none;
            cursor: pointer;
            color: var(--primary);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(26, 35, 126, 0.85), rgba(0, 188, 212, 0.8)), url('https://images.unsplash.com/photo-1519389950473-47ba0277781c?ixlib=rb-4.0.3&auto=format&fit=crop&w=1770&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 180px 0 100px;
            margin-top: 80px;
        }

        .hero h1 {
            color: white;
            font-size: 3.2rem;
            margin-bottom: 1rem;
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 700px;
            margin: 0 auto 2rem;
            opacity: 0.9;
        }

        .hero-btns {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
        }

        /* About Section */
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .profile-img-container {
            flex: 0 0 300px;
        }

        .profile-img {
            width: 100%;
            height: 300px;
            background-color: #e0e0e0;
            border-radius: 50%;
            background-image: url('https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80');
            background-size: cover;
            background-position: center;
            border: 5px solid var(--secondary-light);
        }

        .about-text {
            flex: 1;
        }

        .contact-info {
            margin-top: 30px;
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .contact-icon {
            background: var(--primary-light);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .whatsapp-btn {
            background-color: #25D366;
            color: white;
            padding: 8px 15px;
            border-radius: 5px;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            margin-top: 10px;
        }

        .whatsapp-btn:hover {
            background-color: #128C7E;
        }

        /* Services Section */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .service-card {
            background: white;
            border-radius: 10px;
            padding: 30px;
            box-shadow: var(--shadow);
            transition: var(--transition);
            text-align: center;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .service-icon {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 20px;
        }

        /* Cybersecurity Section */
        .cybersecurity-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }

        .cybersecurity-text {
            flex: 1;
        }

        .cybersecurity-img {
            flex: 0 0 300px;
            height: 300px;
            background-color: #e0e0e0;
            border-radius: 10px;
            background-image: url('https://images.unsplash.com/photo-1550751827-4bd374c3f58b?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=80');
            background-size: cover;
            background-position: center;
        }

        .cyber-areas {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-top: 20px;
        }

        .cyber-area {
            background: var(--primary-light);
            color: white;
            padding: 8px 15px;
            border-radius: 30px;
            font-size: 0.9rem;
        }

        /* Portfolio Section */
        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .portfolio-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .portfolio-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
        }

        .portfolio-img {
            height: 200px;
            background-color: #e0e0e0;
            background-image: url('https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80');
            background-size: cover;
            background-position: center;
        }

        .portfolio-content {
            padding: 20px;
        }

        .portfolio-links {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }

        /* Contact Section */
        .contact-container {
            display: flex;
            gap: 50px;
        }

        .contact-info-section {
            flex: 1;
        }

        .contact-form {
            flex: 1;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: 'Poppins', sans-serif;
        }

        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }

        /* Footer */
        footer {
            background-color: var(--primary-dark);
            color: white;
            padding: 50px 0 20px;
        }

        .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-logo .logo-text {
            color: white;
        }

        .footer-links h3, .footer-contact h3 {
            color: var(--secondary-light);
            margin-bottom: 20px;
        }

        .footer-links ul {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 10px;
        }

        .footer-links a {
            color: #ddd;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover {
            color: var(--secondary);
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            transition: var(--transition);
        }

        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: #aaa;
        }

        /* Responsive Design */
        @media (max-width: 992px) {
            .about-content, .cybersecurity-content, .contact-container {
                flex-direction: column;
            }
            
            .profile-img-container, .cybersecurity-img {
                flex: 0 0 250px;
                width: 250px;
                margin: 0 auto;
            }
            
            h1 {
                font-size: 2.5rem;
            }
            
            h2 {
                font-size: 2rem;
            }
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .hero-btns {
                flex-direction: column;
                align-items: center;
            }
            
            .section {
                padding: 60px 0;
            }
        }

        @media (max-width: 576px) {
            .services-grid, .portfolio-grid {
                grid-template-columns: 1fr;
            }
            
            .contact-info {
                flex-direction: column;
            }
        }
       
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container nav-container">
            <div class="logo">
                <div class="logo-img"><img src="images/cyberlogo.jpg" class="logo "></div>
                <div class="logo-text"><span class="X">CYBERNEX TECH</span> </div>
            </div>
            <button class="mobile-menu-btn">
                <i class="fas fa-bars"></i>
            </button>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#cybersecurity">Cybersecurity</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <h1>Awiagah Ajapa Timothy</h1>
            <p>IT Student | Front-End Developer | Graphic Designer | Cybersecurity Specialist</p>
            <p>Providing professional web development, graphic design, and cybersecurity solutions</p>
            <div class="hero-btns">
                <a href="#portfolio" class="btn">View My Work</a>
                <a href="#contact" class="btn btn-secondary">Hire Me</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="section section-light">
        <div class="container">
            <h2>About Me</h2>
            <div class="about-content">
                <div class="profile-img-container">
                    <div class="profile-img"><img src="images/prof.jpg"  class="profile-img" ></div>
                </div>
                <div class="about-text">
                    <p>I'm <strong>Awiagah Ajapa Timothy</strong>, a dedicated IT student at <strong>Ghana Communication Technology University</strong> with expertise in both creative design and technical development. I specialize in creating professional websites, graphic designs, and providing cybersecurity solutions.</p>
                    
                    <p>My technical skills include front-end development (HTML, CSS, JavaScript), graphic design (posters, banners, invitation cards), and cybersecurity practices to ensure digital safety for businesses and individuals.</p>
                    
                    <div class="contact-info">
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div>
                                <strong>Phone:</strong> 0597989065
                            </div>
                        </div>
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-university"></i>
                            </div>
                            <div>
                                <strong>University:</strong> Ghana Communication Technology University
                            </div>
                        </div>
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div>
                                <strong>Email:</strong> ajapa.timothy@student.gctu.edu.gh
                            </div>
                        </div>
                    </div>
                    
                    <a href="https://wa.me/233597989065" target="_blank" class="whatsapp-btn">
                        <i class="fab fa-whatsapp"></i> Chat on WhatsApp
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="section">
        <div class="container">
            <h2>My Services</h2>
            <p>I offer a wide range of creative and technical services to help bring your digital vision to life.</p>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h3>Professional Websites</h3>
                    <p>Custom, responsive websites built with modern technologies that provide excellent user experience and performance.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-paint-brush"></i>
                    </div>
                    <h3>Graphic Design</h3>
                    <p>Creative designs for posters, banners, invitation cards, logos, and other visual materials that communicate your brand effectively.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-palette"></i>
                    </div>
                    <h3>Picture Editing</h3>
                    <p>Professional photo editing and enhancement services to make your images look their best for any purpose.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <h3>Front-End Development</h3>
                    <p>Building interactive, user-friendly interfaces using HTML, CSS, JavaScript and modern frameworks.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Cybersecurity</h3>
                    <p>Security assessments, vulnerability analysis, and implementation of security measures to protect digital assets.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-lightbulb"></i>
                    </div>
                    <h3>IT Consultation</h3>
                    <p>Expert advice on technology solutions, digital strategy, and IT infrastructure for students and businesses.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Cybersecurity Section -->
    <section id="cybersecurity" class="section section-light">
        <div class="container">
            <h2>Cybersecurity Expertise</h2>
            <div class="cybersecurity-content">
                <div class="cybersecurity-text">
                    <p>While my primary focus includes web development and design, I'm also a <strong>Cybersecurity Specialist</strong> with knowledge in securing digital systems and protecting against threats.</p>
                    
                    <p><strong>What Cybersecurity Professionals Do:</strong> We protect systems, networks, and data from digital attacks. This involves implementing security measures, monitoring for security breaches, investigating incidents, and developing security protocols to safeguard information.</p>
                    
                    <p><strong>Areas of Cybersecurity Capability:</strong></p>
                    <div class="cyber-areas">
                        <span class="cyber-area">Network Security</span>
                        <span class="cyber-area">Vulnerability Assessment</span>
                        <span class="cyber-area">Security Auditing</span>
                        <span class="cyber-area">Data Protection</span>
                        <span class="cyber-area">Threat Analysis</span>
                        <span class="cyber-area">Security Awareness</span>
                        <span class="cyber-area">Risk Management</span>
                        <span class="cyber-area">Incident Response</span>
                    </div>
                    
                    <p>Whether you need security advice for your website, help with securing your digital presence, or consultation on cybersecurity best practices, I can provide expert guidance based on current industry standards.</p>
                    <a href="#contact" class="btn btn-accent">Discuss Security Needs</a>
                </div>
                <div class="cybersecurity-img"></div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="section">
        <div class="container">
            <h2>My Portfolio</h2>
            <p>Here are some of my recent projects. Click on any project to view it in detail.</p>
            <div class="portfolio-grid">
                <div class="portfolio-item">
                    <div class="portfolio-img" style="background-image: url('https://images.unsplash.com/photo-1551650975-87deedd944c3?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80')"></div>
                    <div class="portfolio-content">
                        <h3>E-commerce Website</h3>
                        <p>A fully responsive online store with shopping cart functionality and secure payment integration.</p>
                        <div class="portfolio-links">
                            <a href="#" class="btn">View Project</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <div class="portfolio-img" style="background-image: url('https://images.unsplash.com/photo-1561070791-2526d30994b5?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80')"></div>
                    <div class="portfolio-content">
                        <h3>University Event Posters</h3>
                        <p>Creative poster designs for various university events and activities.</p>
                        <div class="portfolio-links">
                            <a href="#" class="btn">View Designs</a>
                        </div>
                    </div>
                </div>
                <div class="portfolio-item">
                    <div class="portfolio-img" style="background-image: url('https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80')"></div>
                    <div class="portfolio-content">
                        <h3>Business Website</h3>
                        <p>A professional corporate website with CMS integration and responsive design.</p>
                        <div class="portfolio-links">
                            <a href="#" class="btn">View Project</a>
                        </div>
                    </div>
                </div>
            </div>
            <div style="text-align: center; margin-top: 40px;">
                <p><strong>Note:</strong> I will update this section with links to my actual projects hosted on GitHub and other platforms.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section section-light">
        <div class="container">
            <h2>Get In Touch</h2>
            <p>Have a project in mind or need assistance with cybersecurity? Contact me for a consultation.</p>
            <div class="contact-container">
                <div class="contact-info-section">
                    <h3>Contact Information</h3>
                    <p>I'm available for freelance projects, internships, and cybersecurity consultations. Feel free to reach out via any of the following methods:</p>
                    
                    <div class="contact-info">
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-user"></i>
                            </div>
                            <div>
                                <strong>Name:</strong> Awiagah Ajapa Timothy
                            </div>
                        </div>
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-phone"></i>
                            </div>
                            <div>
                                <strong>Phone:</strong> 0597989065
                            </div>
                        </div>
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-university"></i>
                            </div>
                            <div>
                                <strong>University:</strong> Ghana Communication Technology University
                            </div>
                        </div>
                    </div>
                    
                    <div style="margin-top: 30px;">
                        <a href="https://wa.me/233597989065" target="_blank" class="whatsapp-btn" style="margin-right: 10px;">
                            <i class="fab fa-whatsapp"></i> WhatsApp
                        </a>
                        <a href="mailto:ajapa.timothy@student.gctu.edu.gh" class="btn btn-secondary">
                            <i class="fas fa-envelope"></i> Email Me
                        </a>
                    </div>
                </div>
                <div class="contact-form">
                    <h3>Send a Message</h3>
                    <form id="contactForm">
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Your Name" required>
                        </div>
                        <div class="form-group">
                            <input type="email" class="form-control" placeholder="Your Email" required>
                        </div>
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Subject" required>
                        </div>
                        <div class="form-group">
                            <textarea class="form-control" placeholder="Your Message" required></textarea>
                        </div>
                        <button type="submit" class="btn">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-logo">
                    <div class="logo">
                        <div class="logo-img"><img src="images/cyberlogo.jpg" class="logo "></div>
                        <div class="logo-text" class="x">CYBERNEX TECH</div>
                    </div>
                    <p>IT Student | Front-End Developer | Graphic Designer | Cybersecurity Specialist</p>
                    <div class="social-links">
                        <a href="https://github.com/Awiagah/Awiagah-/commit/38a230dbfafced85b2653a0704c2a5c7ddfbebbd"><i class="fab fa-github"></i></a>
                        <a href="https://m.me/awiagah.ajapa.timothy"><i class="fab fa-facebook"></i></a>
                           <a href="https://www.linkedin.com/messaging/thread/new/?filter=inmail"><i class="fab fa-linkedin-in"></i></a>
                        <a href="https://x.com/i/chat/2009278172714688512-2009278172714688512"><i class="fab fa-X">X</i></a>
                        <a href="https://t.me/+233597989065"><i class="fab fa-telegram"></i></a>
                        <a href="https://www.instagram.com/p/DS0plEQDJ3Q/?igsh=MTcyYnNnbWZvZGgwYQ=="><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#about">About</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#cybersecurity">Cybersecurity</a></li>
                        <li><a href="#portfolio">Portfolio</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-contact">
                    <h3>Contact Info</h3>
                    <p><i class="fas fa-phone"></i> 0597989065</p>
                    <p><i class="fas fa-envelope"></i> ajapa.timothy@student.gctu.edu.gh</p>
                    <p><i class="fas fa-university"></i> Ghana Communication Technology University</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Awiagah Ajapa Timothy. All rights reserved.</p>
                <p>This website is hosted on GitHub Pages</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuBtn = document.querySelector('.mobile-menu-btn');
        const navLinks = document.querySelector('.nav-links');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.style.display = navLinks.style.display === 'flex' ? 'none' : 'flex';
        });
        
        // Update mobile menu on window resize
        window.addEventListener('resize', () => {
            if (window.innerWidth > 768) {
                navLinks.style.display = 'flex';
            } else {
                navLinks.style.display = 'none';
            }
        });
        
        // Form submission handling
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your message! I will get back to you soon.');
            this.reset();
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (window.innerWidth <= 768) {
                        navLinks.style.display = 'none';
                    }
                }
            });
        });
    </script>
</body>
</html>
