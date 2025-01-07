<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cybersecurity Professional - Interactive Resume</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #4299e1;
            --secondary-color: #63b3ed;
            --background-color: #0f172a;
            --text-color: #f3f4f6; /* Updated text color */
            --card-bg-color: rgba(45, 55, 72, 0.3);
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%); /* Updated background */
            min-height: 100vh;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        header {
            background-color: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(10px);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--secondary-color);
        }
        nav ul {
            list-style-type: none;
            display: flex;
        }
        nav ul li {
            margin-left: 2rem;
        }
        nav ul li a {
            color: var(--text-color);
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }
        nav ul li a:hover {
            color: var(--secondary-color);
        }
        main {
            padding-top: 80px;
        }
        section {
            margin-bottom: 4rem;
        }
        h1, h2, h3 {
            color: var(--secondary-color);
            margin-bottom: 1rem;
        }
        .hero {
            text-align: center;
            padding: 6rem 0;
            background: linear-gradient(rgba(15, 23, 42, 0.8), rgba(15, 23, 42, 0.8)), url('https://source.unsplash.com/1600x900/?technology,cybersecurity') no-repeat center center/cover;
        }
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 30px;
            text-decoration: none;
            transition: all 0.3s ease;
            font-weight: 600;
            margin: 0.5rem;
        }
        .btn:hover {
            background-color: var(--secondary-color);
            transform: translateY(-3px);
            box-shadow: 0 4px 15px rgba(66, 153, 225, 0.4);
        }
        .terminal {
            background-color: var(--card-bg-color);
            backdrop-filter: blur(10px);
            border-radius: 10px;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            border: 1px solid rgba(74, 85, 104, 0.3);
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        .terminal::before {
            content: "$ ";
            color: #48bb78;
        }
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .project-card {
            background-color: var(--card-bg-color);
            backdrop-filter: blur(10px);
            border-radius: 10px;
            padding: 1.5rem;
            border: 1px solid rgba(74, 85, 104, 0.3);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }
        footer {
            background-color: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(10px);
            color: var(--text-color);
            text-align: center;
            padding: 2rem 0;
            margin-top: 4rem;
        }
        .footer-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }
        .social-links a {
            color: var(--text-color);
            margin: 0 10px;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }
        .social-links a:hover {
            color: var(--secondary-color);
        }
        @media (max-width: 768px) {
            nav ul {
                display: none;
            }
            .footer-content {
                flex-direction: column;
            }
            .social-links {
                margin-top: 1rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <nav>
                <div class="logo">CyberPro</div>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#experience">Experience</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main>
        <section class="hero">
            <div class="container">
                <h1>Cybersecurity Professional</h1>
                <p>Protecting digital assets and securing the future</p>
                <a href="#about" class="btn">Discover My Skills</a>
                <a href="#contact" class="btn">Get In Touch</a>
            </div>
        </section>

        <section id="about">
            <div class="container">
                <h2>About Me</h2>
                <div class="terminal">
                    <p>IT Professional with 5+ years of experience in systems management, technical support, and cybersecurity. Professionally skilled in optimizing multiple CRMs, CDK, Microsoft Office, and Forms, driving efficiency across 16 locations. Experienced in network administration, VoIP systems, SIP Trunking and scalable network design. Personal expertise includes full stack development with Python, React, GitHub, Azure, AWS, and Virtual machines. Dedicated to enhancing operational performance through digital transformation.</p>
                    <ul>
                        <li>Operating Systems</li>
                        <li>Penetration Testing</li>
                        <li>Incident Response</li>
                        <li>Security Architecture</li>
                        <li>Networking</li>
                        <li>Technical Documentation</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="projects">
            <div class="container">
                <h2>Projects</h2>
                <div class="projects-grid">
                    <div class="project-card">
                        <h3>Secure Network Implementation</h3>
                        <p>Microsoft Sentinel Based SIEM for Centralized Log Management and Security Monitoring: Built an SIEM solution using Microsoft Sentinel, enabling real-time threat detection and automated incident response for home network security</p>
                        <ul>
                            <li>Configured enterprise-grade firewalls</li>
                            <li>Implemented intrusion detection and prevention systems</li>
                            <li>Set up VPN for secure remote access</li>
                            <li>Conducted thorough network segmentation</li>
                            <li>Implemented multi-factor authentication across the network</li>
                        </ul>
                    </div>
                    <div class="project-card">
                        <h3>Penetration Testing Framework</h3>
                        <p>AZURE SOC with Honeypot and Threat Intelligence Integration for Proactive Threat Detection: Implemented an AZURE based Security Operation Center (SOC) solution designed to capture attacker tactics, integrate global threat intelligence, and provide real-time threat detection and incident response for enterprise environments.</p>
                        <ul>
                            <li>Created modular architecture for easy expansion</li>
                            <li>Implemented automated vulnerability scanning</li>
                            <li>Developed custom exploit modules</li>
                            <li>Integrated with popular security tools like Metasploit and Nmap</li>
                            <li>Implemented detailed reporting and analytics features</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section id="experience">
            <div class="container">
                <h2>Experience</h2>
                <div class="terminal">
                    <div>
                        <h3>Mastercard Cybersecurity Virtual Experience Program</h3>
                        <p>Mastercard | August 2024</p>
                        <ul>
                            <li>Simulated role as Security Awareness Team analyst at Mastercard</li>
                            <li>Identified phishing threats and analyzed business areas needing enhanced security</li>
                            <li>Designed targeted security training courses and procedures</li>
                            <li>Developed skills in cybersecurity problem solving and data analysis</li>
                        </ul>
                    </div>
                    <div>
                        <h3>AIG Shields Up: Cybersecurity Virtual Experience Program</h3>
                        <p>AIG Corp | August 2024</p>
                        <ul>
                            <li>Participated in Cyber Defense Unity Threat Analysis Simulation</li>
                            <li>Researched vulnerabilities using CISA publications</li>
                            <li>Drafted clear communications for vulnerabilities remediation</li>
                            <li>Developed ethical hacking script for decryption key bruteforcing using Python</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <div class="container">
                <h2>Contact Me</h2>
                <p>Interested in working together? Get in touch!</p>
                <a href="mailto:your.email@example.com" class="btn">Email Me</a>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <div class="footer-content">
                <p>&copy; 2025 Cybersecurity Professional. All rights reserved.</p>
                <div class="social-links">
                    <a href="#" aria-label="LinkedIn"><i class="fab fa-linkedin"></i></a>
                    <a href="#" aria-label="GitHub"><i class="fab fa-github"></i></a>
                    <a href="#" aria-label="Twitter"><i class="fab fa-twitter"></i></a>
                </div>
            </div>
        </div>
    </footer>
    <script src="https://kit.fontawesome.com/your-fontawesome-kit.js" crossorigin="anonymous"></script>
</body>
</html>

