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
            position: relative;
            overflow-x: hidden;
        }

        /* Matrix rain effect */
        .matrix-bg {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            pointer-events: none;
            opacity: 0.1;
            z-index: -1;
        }

        .terminal {
            background-color: rgba(22, 27, 34, 0.95);
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            margin: 10px 0;
            box-shadow: 0 0 10px rgba(0,255,0,0.1);
            position: relative;
            backdrop-filter: blur(5px);
            transition: all 0.3s ease;
        }

        .terminal:hover {
            box-shadow: 0 0 20px rgba(0,255,0,0.2);
            transform: scale(1.01);
        }

        .prompt {
            color: #58a6ff;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .command {
            color: #00ff00;
            position: relative;
            display: inline-block;
        }

        .command::after {
            content: '';
            position: absolute;
            width: 100%;
            height: 2px;
            background: #00ff00;
            bottom: -2px;
            left: 0;
            transform: scaleX(0);
            transform-origin: right;
            transition: transform 0.3s ease;
        }

        .terminal:hover .command::after {
            transform: scaleX(1);
            transform-origin: left;
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
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .project-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 2px;
            background: linear-gradient(90deg, transparent, #00ff00);
            animation: scan 3s linear infinite;
        }

        @keyframes scan {
            0% { left: -100%; }
            100% { left: 100%; }
        }

        .project-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 20px rgba(0, 255, 0, 0.5);
            background: linear-gradient(rgba(22, 27, 34, 0.95), rgba(22, 27, 34, 0.98));
        }

        .metric-bar {
            height: 20px;
            background: linear-gradient(90deg, #238636, #00ff00);
            margin: 5px 0;
            transition: width 1s ease-in-out;
            border-radius: 10px;
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
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .stats-box::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(
                rgba(255, 255, 255, 0.1),
                transparent
            );
            transform: rotate(45deg);
            transition: 0.5s;
            opacity: 0;
        }

        .stats-box:hover::after {
            opacity: 1;
        }

        .stats-box:hover {
            background-color: rgba(35, 134, 54, 0.3);
            transform: translateY(-2px);
        }

        .blink {
            animation: blink 1s infinite;
        }

        @keyframes blink {
            50% { opacity: 0; }
        }

        /* New glitch effect for headings */
        h3 {
            position: relative;
            text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
                        -0.025em -0.05em 0 rgba(0, 255, 0, 0.75),
                        0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
            animation: glitch 500ms infinite;
        }

        @keyframes glitch {
            0% {
                text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
                            -0.05em -0.025em 0 rgba(0, 255, 0, 0.75),
                            -0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
            }
            14% {
                text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
                            -0.05em -0.025em 0 rgba(0, 255, 0, 0.75),
                            -0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
            }
            15% {
                text-shadow: -0.05em -0.025em 0 rgba(255, 0, 0, 0.75),
                            0.025em 0.025em 0 rgba(0, 255, 0, 0.75),
                            -0.05em -0.05em 0 rgba(0, 0, 255, 0.75);
            }
        }

        /* New typing animation for commands */
        .typing {
            overflow: hidden;
            white-space: nowrap;
            border-right: 2px solid #00ff00;
            animation: typing 3.5s steps(40, end),
                       blink-caret 0.75s step-end infinite;
            margin: 0;
        }

        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }

        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #00ff00 }
        }

        /* New list style */
        ul {
            list-style: none;
            padding-left: 0;
        }

        li {
            position: relative;
            padding-left: 20px;
            margin: 8px 0;
            transition: transform 0.2s ease;
        }

        li:before {
            content: '>';
            position: absolute;
            left: 0;
            color: #00ff00;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        li:hover {
            transform: translateX(5px);
        }

        li:hover:before {
            opacity: 1;
        }
    </style>
</head>
<body>
    <!-- Matrix rain canvas will be added by JavaScript -->
    <canvas class="matrix-bg" id="matrix"></canvas>

    <!-- Rest of your existing HTML content remains the same -->
    <!-- ... -->

    <script>
        // Matrix rain effect
        const canvas = document.getElementById('matrix');
        const ctx = canvas.getContext('2d');

        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        const characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*()_+";
        const fontSize = 14;
        const columns = canvas.width/fontSize;
        const drops = [];

        for(let x = 0; x < columns; x++) {
            drops[x] = 1;
        }

        function draw() {
            ctx.fillStyle = 'rgba(0, 0, 0, 0.05)';
            ctx.fillRect(0, 0, canvas.width, canvas.height);

            ctx.fillStyle = '#0F0';
            ctx.font = fontSize + 'px monospace';

            for(let i = 0; i < drops.length; i++) {
                const text = characters.charAt(Math.floor(Math.random() * characters.length));
                ctx.fillText(text, i*fontSize, drops[i]*fontSize);

                if(drops[i]*fontSize > canvas.height && Math.random() > 0.975) {
                    drops[i] = 0;
                }
                drops[i]++;
            }
        }

        setInterval(draw, 33);

        // Resize handler
        window.addEventListener('resize', () => {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
        });
    </script>
</body>
</html>
