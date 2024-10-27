<!DOCTYPE html>
<html>
<head>
    <title>Cybersecurity Professional - Interactive Resume</title>
    <style>
        body {
            background-color: #0d1117;
            color: #00ff00;
            font-family: 'Courier New', monospace;
            margin: 0;
            padding: 20px;
        }
        .terminal {
            background-color: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            margin: 10px 0;
            box-shadow: 0 0 10px rgba(0,255,0,0.1);
        }
        .prompt {
            color: #58a6ff;
            margin-bottom: 10px;
        }
        .command {
            color: #00ff00;
        }
        .output {
            color: #c9d1d9;
            line-height: 1.5;
        }
        .project-card {
            border: 1px solid #30363d;
            margin: 10px 0;
            padding: 15px;
            border-radius: 4px;
            transition: transform 0.3s ease, box-shadow 0.3s ease; /* Add transition for smooth effect */
        }
        .project-card:hover {
            transform: translateY(-5px); /* Move card slightly upwards on hover */
            box-shadow: 0 4px 20px rgba(0, 255, 0, 0.5); /* Enhance shadow on hover */
        }
        .metric-bar {
            height: 20px;
            background-color: #238636;
            margin: 5px 0;
            transition: width 1s ease-in-out;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        .stats-box {
            background: rgba(35, 134, 54, 0.1);
            padding: 15px;
            border-radius: 4px;
            border: 1px solid #238636;
            transition: background-color 0.3s ease; /* Add transition for background color */
        }
        .stats-box:hover {
            background-color: rgba(35, 134, 54, 0.3); /* Darken background on hover */
        }
        .blink {
            animation: blink 1s infinite;
        }
        @keyframes blink {
            50% { opacity: 0; }
        }
    </style>
</head>
<body>
    <div class="terminal">
        <p class="prompt">root@cybersec-portfolio:~$ <span class="command">./display_projects --comprehensive</span></p>
        
        <div class="project-card">
            <h3>🛡️ [01] Microsoft Sentinel SIEM Implementation</h3>
            <div class="grid">
                <div class="stats-box">
                    <h4>Core Components</h4>
                    <ul>
                        <li>Microsoft Azure Cloud Platform</li>
                        <li>Azure Virtual Machine (Windows Pro)</li>
                        <li>Microsoft Sentinel SIEM</li>
                        <li>Log Analytics Workspace</li>
                    </ul>
                </div>
                <div class="stats-box">
                    <h4>Key Features</h4>
                    <ul>
                        <li>Centralized Log Collection</li>
                        <li>Real-Time Threat Detection</li>
                        <li>Custom Alert Rules</li>
                        <li>RDP Event Monitoring</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="project-card">
            <h3>🔐 [02] NSA Codebreaker Challenge 2023</h3>
            <div class="grid">
                <div class="stats-box">
                    <h4>Tools Utilized</h4>
                    <ul>
                        <li>Wireshark - Network Analysis</li>
                        <li>Python & Rust - Development</li>
                        <li>OpenSSL - Security Testing</li>
                        <li>Base86 & Assembly - Low-level Analysis</li>
                    </ul>
                </div>
                <div class="stats-box">
                    <h4>Achievements</h4>
                    <ul>
                        <li>Complex Task Completion</li>
                        <li>Threat Analysis Implementation</li>
                        <li>Signal Decryption Success</li>
                        <li>Security Awareness Enhancement</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="project-card">
            <h3>🌐 [03] Enterprise Home Lab Setup</h3>
            <div class="grid">
                <div class="stats-box">
                    <h4>Hardware Infrastructure</h4>
                    <ul>
                        <li>Protectli Vault (pfSense)</li>
                        <li>Netgear 84 Gbit Switch</li>
                        <li>Nighthawk WiFi 6 Router</li>
                        <li>TerraMaster F2-221 NAS</li>
                        <li>Lenovo ThinkServer TS140</li>
                    </ul>
                </div>
                <div class="stats-box">
                    <h4>Software Stack</h4>
                    <ul>
                        <li>pfSense & VLANs</li>
                        <li>Proxmox VM Management</li>
                        <li>Pi-hole DNS Protection</li>
                        <li>OpenVPN & Cloudflare</li>
                    </ul>
                </div>
                <div class="stats-box">
                    <h4>Implementations</h4>
                    <ul>
                        <li>VLAN Segmentation</li>
                        <li>Granular Firewall Rules</li>
                        <li>Virtual Machine Management</li>
                        <li>Secure Remote Access</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="project-card">
            <h3>💻 [04] Development Workstation</h3>
            <div class="grid">
                <div class="stats-box">
                    <h4>System Specifications</h4>
                    <ul>
                        <li>NVIDIA RTX 3070TI (AI/ML Ready)</li>
                        <li>Dual Boot: Windows 11 + Ubuntu</li>
                        <li>Ultrawide Monitor Setup</li>
                        <li>Custom Cooling Solution</li>
                    </ul>
                </div>
                <div class="stats-box">
                    <h4>Optimizations</h4>
                    <ul>
                        <li>AI/ML Development Environment</li>
                        <li>Enhanced Display Configuration</li>
                        <li>Performance Tuning</li>
                        <li>Comprehensive Documentation</li>
                    </ul>
                </div>
            </div>
        </div>
    </div>

    <div class="terminal">
        <p class="prompt">root@cybersec-portfolio:~$ <span class="command">./show_experience</span></p>
        <div class="grid">
            <div class="stats-box">
                <h4>Mastercard Cybersecurity Program</h4>
                <ul>
                    <li>Security Awareness Analysis</li>
                    <li>Phishing Threat Assessment</li>
                    <li>Security Training Development</li>
                    <li>Data Analysis Implementation</li>
                </ul>
            </div>
            <div class="stats-box">
                <h4>AIG Shields Up Program</h4>
                <ul>
                    <li>Threat Analysis Simulation</li>
                    <li>CISA Research & Implementation</li>
                    <li>Python Script Development</li>
                    <li>Technical Documentation</li>
                </ul>
            </div>
        </div>
    </div>

    <div class="terminal">
        <p class="prompt">root@cybersec-portfolio:~$ <span class="blink">_</span></p>

