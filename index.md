<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cybersecurity Professional - Interactive Resume</title>
    <style>
        /* Base styles */
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #e2e8f0;
            margin: 0;
            padding: 0;
            background: linear-gradient(to bottom right, #1a202c, #000000, #2a4365);
            min-height: 100vh;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        /* Header styles */
        header {
            background-color: rgba(26, 32, 44, 0.8);
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
            display: flex;
            justify-content: center;
        }
        nav ul li {
            margin: 0 15px;
        }
        nav ul li a {
            color: #e2e8f0;
            text-decoration: none;
            font-weight: bold;
        }
        /* Main content styles */
        main {
            padding-top: 80px;
        }
        section {
            margin-bottom: 4rem;
        }
        h1, h2, h3 {
            color: #63b3ed;
        }
        .hero {
            text-align: center;
            padding: 4rem 0;
        }
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        .btn {
            display: inline-block;
            background-color: #4299e1;
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 9999px;
            text-decoration: none;
            transition: background-color 0.3s;
            margin: 0.5rem;
        }
        .btn:hover {
            background-color: #3182ce;
        }
        /* Terminal-like box styles */
        .terminal {
            background-color: rgba(45, 55, 72, 0.3);
            backdrop-filter: blur(10px);
            border-radius: 0.5rem;
            padding: 1.5rem;
            margin-bottom: 1.5rem;
            border: 1px solid #4a5568;
        }
        .terminal::before {
            content: "$ ";
            color: #48bb78;
        }
        /* Project styles */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .project-card {
            background-color: rgba(45, 55, 72, 0.3);
            backdrop-filter: blur(10px);
            border-radius: 0.5rem;
            padding: 1.5rem;
            border: 1px solid #4a5568;
        }
        /* Footer styles */
        footer {
            background-color: #1a202c;
            color: #e2e8f0;
            text-align: center;
            padding: 2rem 0;
            margin-top: 4rem;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="container">
                <h1>Cybersecurity Professional</h1>
                <p>Protecting digital assets and securing the future</p>
                <a href="#about" class="btn">About Me</a>
                <a href="#projects" class="btn">My Projects</a>
                <a href="#experience" class="btn">Experience</a>
                <a href="#contact" class="btn">Contact</a>
            </div>
        </section>

        <section id="about">
            <div class="container">
                <h2>About Me</h2>
                <div class="terminal">
                    <p>Experienced cybersecurity professional with expertise in:</p>
                    <ul>
                        <li>Network Security</li>
                        <li>Penetration Testing</li>
                        <li>Incident Response</li>
                        <li>Security Architecture</li>
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
                        <p>Designed and implemented a secure network infrastructure for a Fortune 500 company.</p>
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
                        <p>Developed a custom penetration testing framework for the security team.</p>
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
                        <h3>Senior Cybersecurity Analyst</h3>
                        <p>TechGuard Solutions | 2020 - Present</p>
                        <ul>
                            <li>Lead a team of security analysts in threat detection and incident response</li>
                            <li>Implement and maintain security information and event management (SIEM) systems</li>
                            <li>Conduct regular security assessments and provide recommendations for improvements</li>
                        </ul>
                    </div>
                    <div>
                        <h3>Information Security Specialist</h3>
                        <p>CyberDefense Corp | 2017 - 2020</p>
                        <ul>
                            <li>Performed vulnerability assessments and penetration testing for client networks</li>
                            <li>Developed and implemented security policies and procedures</li>
                            <li>Provided security awareness training to employees across the organization</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact">
            <div class="container">
                <h2>Contact Me</h2>
                <p>Interested in working together? Get in touch!</p>
                <a href="mailto:contact@example.com" class="btn">Email Me</a>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 Cybersecurity Professional. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>
