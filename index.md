<body>
    <div class="container-lg px-3 my-5 markdown-body">
      
      <h1><a href="https://jhnygz.github.io/jwilliams.github.io/">JhnyGz Portfolio</a></h1>
      

      <p>&lt;!DOCTYPE html&gt;</p>


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
                <h1>Cybersecurity Professional Resume</h1>
                <p>Protecting digital assets and securing the future</p>
                <a href="#about" class="btn">About Me</a>
                <a href="#projects" class="btn">My Projects</a>
                <a href="#experience" class="btn">Experience</a>
                <a href="#contact" class="btn">Contact</a>
            </div>
        </section>

        <section id="about">
            <div class="container">
                <h2 id="about-me">About Me<a class="anchorjs-link " href="#about-me" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>
                <div class="terminal">
                    <p>IT Professional with 5+ years of experience in systems management,
                    technical support, and cybersecruity. Professionally skilled in optimizing
                    multiple CRMs, CDK, Microsfot Office, and Forms, driving effciency across
                    16 locations. Experienced in network admininstation, VoIP systems, SIP
                    Trucking and scalable network design. Personal Expertise includes full 
                    stack development with Python, React, Github, Azure, AWS, and Virtual 
                    machines. Dedicated to enhancing opertional perfoamce through digital
                    transformation.:</p>
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
                <h2 id="projects-1">Projects<a class="anchorjs-link " href="#projects-1" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>
                <div class="projects-grid">
                    <div class="project-card">
                        <h3 id="secure-network-implementation">Secure Network Implementation<a class="anchorjs-link " href="#secure-network-implementation" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>
                        <p>Microsoft Sentinel Based SIEM for Centralized Log Managment and Security Monitoring: Built
an SIEM solution using Microsoft Sentinel, enabling real-time treat detection and automated incident
response for home network security</p>
                        <ul>
                            <li>Configured enterprise-grade firewalls</li>
                            <li>Implemented intrusion detection and prevention systems</li>
                            <li>Set up VPN for secure remote access</li>
                            <li>Conducted thorough network segmentation</li>
                            <li>Implemented multi-factor authentication across the network</li>
                        </ul>
                    </div>
                    <div class="project-card">
                        <h3 id="penetration-testing-framework">Penetration Testing Framework<a class="anchorjs-link " href="#penetration-testing-framework" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>
                        <p>AZURE SOC with Honeypot and Threat Intelligence Intergration for Proactive Threat Detection:
Implemented an AZURE based security Operation Center (SOC) solution designed to capture attacker
tactics, integrate global threat intelligence m and provide real time threat detection and incident
response for enterprise environments.</p>
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
                <h2 id="experience-1">Experience<a class="anchorjs-link " href="#experience-1" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>
                <div class="terminal">
                    <div>
                        <h3 id="mastercard-cybersecurity-virtual-experience-program">Mastercard Cybersecurity Virtual Experience Program<a class="anchorjs-link " href="#mastercard-cybersecurity-virtual-experience-program" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>
                        <p>Mastercard | August 2024</p>
                        <ul>
                            <li>Simulated role as Security Awareness Team analyst at Mastercard</li>
                            <li>Identified phishing threats and analyzed business areas needing enhancing security</li>
                            <li>Designed Targeted security training courses and procedures</li>
                            <li>Developed skills in cybersecurity problem solving and data analysis</li>
                        </ul>
                    </div>
                    <div>
                        <h3 id="aig-sheilds-up-cybersecurity-virtual-experience-program">AIG Sheilds Up: Cybersecurity Virtual Experience Program<a class="anchorjs-link " href="#aig-sheilds-up-cybersecurity-virtual-experience-program" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h3>
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
                <h2 id="contact-me">Contact Me<a class="anchorjs-link " href="#contact-me" aria-label="Anchor" data-anchorjs-icon="" style="font: 1em / 1 anchorjs-icons; padding-left: 0.375em;"></a></h2>
                <p>Interested in working together? Get in touch!</p>
                <a href="mailto:jwilliams2940@outlook.com" class="btn">Email Me</a>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>© 2025 Cybersecurity Professional. All rights reserved.</p>
        </div>
    </footer>




      
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/anchor-js/4.1.0/anchor.min.js" integrity="sha256-lZaRhKri35AyJSypXXs4o6OPFTbTmUoltBbDCbdzegg=" crossorigin="anonymous"></script>
    <script>anchors.add();</script>
  

</body>
