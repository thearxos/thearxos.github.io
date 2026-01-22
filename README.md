<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="ARXOS - Arch-based penetration testing OS with 2800+ tools. Built for hackers, developers, and power users.">
    <title>Welcome to ARXOS</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@300;400;600;700;900&family=Orbitron:wght@400;700;900&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --bg-hard: #000000;
            --fg: #ffffff;
            --accent-light: #cccccc;
            --fg-dim: #a0a0a0;
            --glow-grey: #888888;
        }

        body {
            background: #000000;
            color: #ffffff;
            font-family: 'JetBrains Mono', monospace;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            margin: 0;
            padding: 0;
            position: relative;
        }

        /* Animated gradient background */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 50% 50%, rgba(136, 136, 136, 0.15) 0%, transparent 70%);
            animation: pulse-bg 5s ease-in-out infinite;
            z-index: 1;
            opacity: 0;
            transition: opacity 1s ease;
        }

        body.show-bg::before {
            opacity: 1;
        }

        @keyframes pulse-bg {
            0%, 100% { transform: scale(1); opacity: 0.5; }
            50% { transform: scale(1.1); opacity: 1; }
        }

        /* Video intro overlay */
        .video-intro-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: #000000;
            z-index: 10000;
            display: flex;
            justify-content: center;
            align-items: center;
            opacity: 1;
            transition: opacity 0.8s ease;
        }

        .video-intro-overlay.fade-out {
            opacity: 0;
            pointer-events: none;
        }

        .video-intro-overlay video {
            max-width: 100%;
            max-height: 100%;
            object-fit: contain;
        }

        /* Skip button for video */
        .skip-video-btn {
            position: fixed;
            bottom: 40px;
            right: 40px;
            padding: 12px 30px;
            background: rgba(255, 255, 255, 0.1);
            border: 2px solid var(--accent-light);
            color: var(--accent-light);
            font-family: 'Orbitron', monospace;
            font-size: 14px;
            cursor: pointer;
            border-radius: 25px;
            z-index: 10001;
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
            opacity: 0;
            animation: fadeInBtn 0.5s ease 1s forwards;
        }

        @keyframes fadeInBtn {
            to { opacity: 1; }
        }

        .skip-video-btn:hover {
            background: var(--accent-light);
            color: var(--bg-hard);
            transform: translateY(-2px);
        }

        /* Matrix canvas */
        #matrix-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 2;
            opacity: 0;
            transition: opacity 1s ease;
        }

        #matrix-canvas.visible {
            opacity: 0.15;
        }

        /* Welcome container */
        .welcome-container {
            position: relative;
            z-index: 10;
            text-align: center;
            padding: 40px 20px;
            opacity: 0;
            transition: opacity 1.2s ease;
            transform: translateY(30px);
        }

        .welcome-container.visible {
            opacity: 1;
            animation: slideInUp 1s ease forwards;
        }

        @keyframes slideInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .welcome-text h2 {
            font-family: 'Orbitron', monospace;
            font-size: 3.5rem;
            font-weight: 900;
            margin-bottom: 25px;
            color: var(--fg);
            text-shadow: 0 0 40px rgba(255, 255, 255, 0.4);
            letter-spacing: 8px;
            animation: glow 3s ease-in-out infinite, float 4s ease-in-out infinite;
        }

        @keyframes glow {
            0%, 100% { text-shadow: 0 0 40px rgba(255, 255, 255, 0.4); }
            50% { text-shadow: 0 0 60px rgba(255, 255, 255, 0.6), 0 0 80px rgba(255, 255, 255, 0.4); }
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .welcome-text h1 {
            font-family: 'Orbitron', monospace;
            font-size: 6rem;
            font-weight: 900;
            color: var(--accent-light);
            text-shadow: 0 0 60px rgba(255, 255, 255, 0.6);
            letter-spacing: 14px;
            margin-bottom: 35px;
            animation: pulse 2s ease-in-out infinite, glitch 8s ease-in-out infinite;
            position: relative;
        }

        @keyframes pulse {
            0%, 100% { transform: scale(1); }
            50% { transform: scale(1.02); }
        }

        @keyframes glitch {
            0%, 90%, 100% { transform: translate(0); }
            92% { transform: translate(-2px, 2px); }
            94% { transform: translate(2px, -2px); }
            96% { transform: translate(-2px, -2px); }
            98% { transform: translate(2px, 2px); }
        }

        .cursor {
            display: inline-block;
            animation: blink 1s infinite;
        }

        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0; }
        }

        .welcome-text p {
            font-size: 1.4rem;
            letter-spacing: 4px;
            color: var(--glow-grey);
            margin-top: 30px;
            animation: fadeIn 2s ease forwards;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Particle effect */
        .particle {
            position: fixed;
            width: 4px;
            height: 4px;
            background: var(--accent-light);
            border-radius: 50%;
            pointer-events: none;
            z-index: 5;
            animation: particleFloat 3s ease-in-out infinite;
            opacity: 0.6;
        }

        @keyframes particleFloat {
            0%, 100% { transform: translateY(0) translateX(0); }
            25% { transform: translateY(-20px) translateX(10px); }
            50% { transform: translateY(-40px) translateX(-10px); }
            75% { transform: translateY(-20px) translateX(5px); }
        }

        /* Enter button */
        .cta-button {
            position: fixed;
            bottom: 40px;
            left: 50%;
            transform: translateX(-50%);
            z-index: 100;
            padding: 25px 60px;
            font-size: 18px;
            font-weight: 700;
            font-family: 'Orbitron', monospace;
            border: 3px solid var(--accent-light);
            background: transparent;
            color: var(--accent-light);
            cursor: pointer;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            text-decoration: none;
            text-transform: uppercase;
            letter-spacing: 3px;
            border-radius: 50px;
            box-shadow: 0 0 30px rgba(224, 224, 224, 0.2);
            opacity: 0;
            overflow: hidden;
            display: inline-block;
        }

        .cta-button.visible {
            opacity: 1;
            animation: buttonFloat 3s ease-in-out infinite, buttonPulse 2s ease-in-out infinite;
        }

        @keyframes buttonFloat {
            0%, 100% { transform: translateX(-50%) translateY(0); }
            50% { transform: translateX(-50%) translateY(-10px); }
        }

        @keyframes buttonPulse {
            0%, 100% { box-shadow: 0 0 30px rgba(224, 224, 224, 0.2); }
            50% { box-shadow: 0 0 50px rgba(224, 224, 224, 0.4), 0 0 70px rgba(224, 224, 224, 0.2); }
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 0;
            height: 100%;
            background: var(--accent-light);
            transition: width 0.4s ease;
            z-index: -1;
            border-radius: 50px;
        }

        .cta-button::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.3);
            transform: translate(-50%, -50%);
            transition: width 0.6s, height 0.6s;
        }

        .cta-button:hover::before {
            width: 100%;
        }

        .cta-button:hover::after {
            width: 300px;
            height: 300px;
        }

        .cta-button:hover {
            color: var(--bg-hard);
            box-shadow: 0 20px 50px rgba(224, 224, 224, 0.5);
            transform: translateX(-50%) translateY(-5px) scale(1.05);
        }

        .arrow {
            display: inline-block;
            margin-left: 10px;
            transition: transform 0.3s ease;
        }

        .cta-button:hover .arrow {
            transform: translateX(10px);
            animation: arrowBounce 0.6s ease-in-out infinite;
        }

        @keyframes arrowBounce {
            0%, 100% { transform: translateX(10px); }
            50% { transform: translateX(15px); }
        }

        /* Footer */
        .footer-text {
            position: fixed;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            font-size: 13px;
            color: var(--fg-dim);
            letter-spacing: 2px;
            z-index: 2;
            opacity: 0;
            transition: opacity 1s ease;
        }

        .footer-text.visible {
            opacity: 1;
            animation: fadeInUp 1s ease forwards;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateX(-50%) translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateX(-50%) translateY(0);
            }
        }

        /* Visitor counter badge */
        .visitor-badge {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: rgba(0, 0, 0, 0.9);
            border: 2px solid var(--accent-light);
            padding: 15px 25px;
            border-radius: 50px;
            font-size: 13px;
            color: var(--fg-dim);
            z-index: 100;
            backdrop-filter: blur(10px);
            box-shadow: 0 0 30px rgba(255, 255, 255, 0.2);
            opacity: 0;
            transition: all 0.5s ease;
        }

        .visitor-badge.visible {
            opacity: 1;
            animation: slideInRight 0.8s ease forwards;
        }

        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(100px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        .visitor-badge:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 40px rgba(255, 255, 255, 0.3);
        }

        .visitor-count {
            color: var(--accent-light);
            font-weight: 700;
            font-family: 'Orbitron', monospace;
            font-size: 16px;
            display: inline-block;
            animation: countUp 2s ease forwards;
        }

        @keyframes countUp {
            from { opacity: 0; transform: scale(0.5); }
            to { opacity: 1; transform: scale(1); }
        }

        /* Page transition */
        body.page-transition {
            animation: fadeOut 0.8s ease forwards;
        }

        @keyframes fadeOut {
            to { opacity: 0; }
        }

        /* Loading spinner for video */
        .video-loader {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 60px;
            height: 60px;
            border: 4px solid rgba(204, 204, 204, 0.2);
            border-top-color: var(--accent-light);
            border-radius: 50%;
            animation: spin 1s linear infinite;
            z-index: 10002;
        }

        @keyframes spin {
            to { transform: translate(-50%, -50%) rotate(360deg); }
        }

        /* Responsive */
        @media (max-width: 1024px) {
            .welcome-text h2 { font-size: 3rem; }
            .welcome-text h1 { font-size: 5rem; }
        }

        @media (max-width: 768px) {
            .welcome-text h2 { 
                font-size: 2.5rem; 
                letter-spacing: 4px; 
                margin-bottom: 20px;
            }
            .welcome-text h1 { 
                font-size: 3.5rem; 
                letter-spacing: 6px; 
            }
            .welcome-text p { 
                font-size: 1.1rem; 
                letter-spacing: 2px; 
            }
            .cta-button { 
                padding: 20px 45px; 
                font-size: 16px; 
                bottom: 100px;
                width: 90%;
                max-width: 350px;
            }
            .visitor-badge {
                bottom: 120px;
                right: 50%;
                transform: translateX(50%);
                padding: 10px 20px;
                font-size: 12px;
            }
            .visitor-badge.visible {
                animation: slideInUpMobile 0.8s ease forwards;
            }
            @keyframes slideInUpMobile {
                from {
                    opacity: 0;
                    transform: translateX(50%) translateY(50px);
                }
                to {
                    opacity: 1;
                    transform: translateX(50%) translateY(0);
                }
            }
            .visitor-count { font-size: 14px; }
            .skip-video-btn {
                bottom: 20px;
                right: 20px;
                padding: 10px 20px;
                font-size: 12px;
            }
        }

        @media (max-width: 480px) {
            .welcome-text h2 { 
                font-size: 1.8rem; 
                letter-spacing: 3px; 
            }
            .welcome-text h1 { 
                font-size: 2.5rem; 
                letter-spacing: 4px; 
            }
            .welcome-text p { 
                font-size: 0.9rem; 
                letter-spacing: 1px; 
            }
            .cta-button {
                padding: 18px 35px;
                font-size: 14px;
            }
            .footer-text {
                font-size: 10px;
                letter-spacing: 1px;
            }
        }

        /* Touch device optimizations */
        @media (hover: none) and (pointer: coarse) {
            .cta-button:active {
                transform: translateX(-50%) scale(0.95);
            }
            .visitor-badge:active {
                transform: scale(0.95);
            }
        }
    </style>
</head>
<body>
    <!-- Video Intro (arxos.mp4) -->
    <div class="video-intro-overlay" id="videoIntroOverlay">
        <div class="video-loader" id="videoLoader"></div>
        <video id="introVideo" autoplay muted playsinline>
            <source src="arxos.mp4" type="video/mp4">
        </video>
        <button class="skip-video-btn" onclick="showWelcomeScreen()">Skip Intro</button>
    </div>

    <!-- Matrix Canvas -->
    <canvas id="matrix-canvas"></canvas>

    <!-- Visitor Badge -->
    <div class="visitor-badge" id="visitorBadge">
        👁️ Visitors: <span class="visitor-count" id="visitorCount">...</span>
    </div>

    <!-- Welcome Container -->
    <div class="welcome-container" id="welcomeContainer">
        <div class="welcome-text">
            <h2>WELCOME TO</h2>
            <h1>ARXOS<span class="cursor">_</span></h1>
            <p>Where Performance Meets Penetration Testing</p>
        </div>
    </div>

    <!-- Enter Button -->
    <a href="main.html" class="cta-button" id="enterButton">
        Enter ARXOS <span class="arrow">→</span>
    </a>

    <!-- Footer -->
    <div class="footer-text" id="footerText">
        &copy; 2026 ARXOS | Created by oxbv1 | 0xb0rn3
    </div>

    <!-- Hidden tracking -->
    <iframe id="ghTrack" style="display:none;width:0;height:0;border:0;"></iframe>

    <script>
        const videoIntroOverlay = document.getElementById('videoIntroOverlay');
        const introVideo = document.getElementById('introVideo');
        const videoLoader = document.getElementById('videoLoader');
        const matrixCanvas = document.getElementById('matrix-canvas');
        const welcomeContainer = document.getElementById('welcomeContainer');
        const enterButton = document.getElementById('enterButton');
        const footerText = document.getElementById('footerText');
        const visitorBadge = document.getElementById('visitorBadge');

        // Hide loader when video loads
        introVideo.addEventListener('loadeddata', () => {
            videoLoader.style.display = 'none';
        });

        function showWelcomeScreen() {
            videoIntroOverlay.classList.add('fade-out');
            setTimeout(() => {
                videoIntroOverlay.style.display = 'none';
                document.body.classList.add('show-bg');
                matrixCanvas.classList.add('visible');
                welcomeContainer.classList.add('visible');
                
                setTimeout(() => {
                    if (enterButton) {
                        enterButton.classList.add('visible');
                        enterButton.style.display = 'block';
                    }
                    if (footerText) footerText.classList.add('visible');
                    if (visitorBadge) visitorBadge.classList.add('visible');
                    createParticles();
                }, 500);
                
                startMatrixRain();
            }, 800);
        }

        // Create floating particles
        function createParticles() {
            const particleCount = window.innerWidth < 768 ? 10 : 20;
            for (let i = 0; i < particleCount; i++) {
                setTimeout(() => {
                    const particle = document.createElement('div');
                    particle.className = 'particle';
                    particle.style.left = Math.random() * 100 + '%';
                    particle.style.top = Math.random() * 100 + '%';
                    particle.style.animationDelay = Math.random() * 3 + 's';
                    particle.style.animationDuration = (Math.random() * 2 + 2) + 's';
                    document.body.appendChild(particle);
                }, i * 100);
            }
        }

        introVideo.addEventListener('ended', showWelcomeScreen);
        introVideo.addEventListener('error', showWelcomeScreen);
        setTimeout(showWelcomeScreen, 6000);

        function startMatrixRain() {
            const ctx = matrixCanvas.getContext('2d');
            matrixCanvas.width = window.innerWidth;
            matrixCanvas.height = window.innerHeight;

            const matrix = "ARXOS01アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲン";
            const fontSize = 14;
            const columns = matrixCanvas.width / fontSize;
            const drops = Array(Math.floor(columns)).fill(1);

            function draw() {
                ctx.fillStyle = 'rgba(0, 0, 0, 0.05)';
                ctx.fillRect(0, 0, matrixCanvas.width, matrixCanvas.height);
                ctx.fillStyle = '#cccccc';
                ctx.font = fontSize + 'px monospace';

                for (let i = 0; i < drops.length; i++) {
                    const text = matrix[Math.floor(Math.random() * matrix.length)];
                    ctx.fillText(text, i * fontSize, drops[i] * fontSize);
                    if (drops[i] * fontSize > matrixCanvas.height && Math.random() > 0.975) drops[i] = 0;
                    drops[i]++;
                }
            }

            setInterval(draw, 50);
            window.addEventListener('resize', () => {
                matrixCanvas.width = window.innerWidth;
                matrixCanvas.height = window.innerHeight;
            });
        }

        enterButton.addEventListener('click', (e) => {
            e.preventDefault();
            document.body.classList.add('page-transition');
            setTimeout(() => window.location.href = 'main.html', 800);
        });

        // Enhanced visitor tracking with animation
        (function(){
            var _0x1=['ghTrack','getElementById','src','https://github.com/thearxos/thearxos.github.io','https://api.github.com/repos/thearxos/thearxos.github.io','then','json','watchers_count','textContent','toLocaleString','visitorBadge','classList','add','visible','visitorCount'];
            setTimeout(function(){
                try{
                    document[_0x1[1]](_0x1[0])[_0x1[2]]=_0x1[3];
                    fetch(_0x1[4])[_0x1[5]](function(r){
                        return r[_0x1[6]]();
                    })[_0x1[5]](function(d){
                        var c=d[_0x1[7]]||0;
                        var e=document[_0x1[1]](_0x1[14]);
                        var b=document[_0x1[1]](_0x1[10]);
                        if(e){
                            // Animate count up
                            let current = 0;
                            const target = c;
                            const increment = Math.ceil(target / 50);
                            const timer = setInterval(() => {
                                current += increment;
                                if (current >= target) {
                                    current = target;
                                    clearInterval(timer);
                                }
                                e[_0x1[8]]=current[_0x1[9]]();
                            }, 30);
                        }
                        if(b){
                            b[_0x1[11]][_0x1[12]](_0x1[13]);
                        }
                    }).catch(function(){
                        // Fallback display
                        var e=document[_0x1[1]](_0x1[14]);
                        if(e) e[_0x1[8]]='1000+';
                    });
                }catch(e){}
            },2000);
        })();
    </script>
</body>
</html>
