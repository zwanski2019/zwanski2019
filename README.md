<!-- 
╔══════════════════════════════════════════════════════════════════╗
║                                                                    ║
║                         Z W A N S K I                             ║
║                    █▀▀ █▄░▄█ ▄▀▄ █░█ █ █▄░█ █▀▀                 ║
║                    █▄▄ █░▀░█ █▄█ █▄█ █ █░▀█ █▄█                 ║
║                                                                    ║
║                    QUANTUM SECURITY DIVISION                      ║
║                          🜁 0x7F 🜁                                ║
║                                                                    ║
║               // AUTHORIZED ACCESS ONLY //                        ║
║                 SESSION: [▓▓▓▓▓▓▓▓▓▓] 2048-bit                    ║
║                                                                    ║
╚══════════════════════════════════════════════════════════════════╝
-->

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ZWANSKI // QUANTUM SECURITY CORE</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: #0a0a0f;
            font-family: 'SF Mono', 'Fira Code', 'JetBrains Mono', monospace;
            color: #00ffaa;
            line-height: 1.4;
            padding: 20px;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }
        
        /* Quantum grid background */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                linear-gradient(rgba(0, 255, 170, 0.03) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 255, 170, 0.03) 1px, transparent 1px);
            background-size: 50px 50px;
            pointer-events: none;
            z-index: -1;
        }
        
        /* Particle effect */
        body::after {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 20% 50%, rgba(0, 255, 170, 0.05) 0%, transparent 50%);
            pointer-events: none;
            z-index: -1;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }
        
        /* Terminal-style header */
        .quantum-header {
            border: 1px solid #00ffaa20;
            padding: 30px;
            margin-bottom: 30px;
            background: #0a0a0fcc;
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }
        
        .quantum-header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 2px;
            background: linear-gradient(90deg, transparent, #00ffaa, #00ffaa, transparent);
            animation: scan 3s linear infinite;
        }
        
        @keyframes scan {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        .glitch-text {
            font-size: clamp(3rem, 10vw, 6rem);
            font-weight: 900;
            letter-spacing: -3px;
            line-height: 1;
            text-shadow: 
                3px 3px 0 #ff00aa40,
                -3px -3px 0 #00aaff40;
            position: relative;
            animation: glitch 3s infinite;
        }
        
        @keyframes glitch {
            0%, 100% { transform: none; opacity: 1; }
            92% { transform: skew(0); }
            93% { transform: skew(5deg); }
            94% { transform: skew(-5deg); }
            95% { transform: skew(3deg); }
            96% { transform: skew(-3deg); }
        }
        
        .matrix-rain {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            overflow: hidden;
            pointer-events: none;
            opacity: 0.1;
        }
        
        .matrix-rain span {
            position: absolute;
            color: #00ffaa;
            font-size: 20px;
            animation: rain 10s linear infinite;
        }
        
        @keyframes rain {
            0% { transform: translateY(-100%); }
            100% { transform: translateY(100vh); }
        }
        
        /* Quantum stats grid */
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2px;
            margin: 40px 0;
            background: #00ffaa20;
            padding: 2px;
        }
        
        .stat-item {
            background: #0a0a0f;
            padding: 30px 20px;
            text-align: center;
            position: relative;
            border: 1px solid transparent;
            transition: 0.3s;
        }
        
        .stat-item:hover {
            border-color: #00ffaa;
            transform: scale(1.02);
            z-index: 2;
        }
        
        .stat-value {
            font-size: 3rem;
            font-weight: 900;
            line-height: 1;
            margin-bottom: 10px;
            text-shadow: 0 0 20px #00ffaa;
        }
        
        .stat-label {
            font-size: 0.8rem;
            text-transform: uppercase;
            letter-spacing: 2px;
            opacity: 0.5;
        }
        
        /* Holographic cards */
        .hologram {
            background: linear-gradient(135deg, #0a0a0f 0%, #1a1a2a 100%);
            border: 1px solid #00ffaa20;
            padding: 30px;
            margin: 20px 0;
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(5px);
        }
        
        .hologram::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(45deg, transparent 30%, rgba(0, 255, 170, 0.1) 50%, transparent 70%);
            animation: shimmer 8s infinite;
        }
        
        @keyframes shimmer {
            0% { transform: translateX(-100%) translateY(-100%) rotate(45deg); }
            100% { transform: translateX(100%) translateY(100%) rotate(45deg); }
        }
        
        /* Binary rain */
        .binary-row {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            margin: 10px 0;
            font-size: 0.8rem;
            opacity: 0.3;
            color: #00ffaa;
        }
        
        /* Quantum core visualization */
        .core-container {
            position: relative;
            height: 400px;
            margin: 40px 0;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .core {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            background: radial-gradient(circle at 30% 30%, #00ffaa, #004422);
            box-shadow: 
                0 0 50px #00ffaa,
                0 0 100px #00ffaa40;
            animation: pulse 2s ease-in-out infinite;
            position: relative;
        }
        
        .core::before,
        .core::after {
            content: '';
            position: absolute;
            top: -50px;
            left: -50px;
            right: -50px;
            bottom: -50px;
            border: 2px solid #00ffaa40;
            border-radius: 50%;
            animation: orbit 4s linear infinite;
        }
        
        .core::after {
            animation: orbit 6s linear infinite reverse;
        }
        
        @keyframes pulse {
            0%, 100% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.1); opacity: 0.8; }
        }
        
        @keyframes orbit {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        /* Command line */
        .command-line {
            background: #00000080;
            border-left: 3px solid #00ffaa;
            padding: 15px;
            margin: 20px 0;
            font-family: monospace;
            position: relative;
        }
        
        .command-line::before {
            content: '>';
            position: absolute;
            left: -20px;
            color: #00ffaa;
        }
        
        /* Fingerprint grid */
        .fingerprint-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 20px;
            margin: 40px 0;
        }
        
        .fingerprint-cell {
            aspect-ratio: 1;
            background: linear-gradient(45deg, #00ffaa10, #000000);
            border: 1px solid #00ffaa30;
            position: relative;
            overflow: hidden;
        }
        
        .fingerprint-cell::before {
            content: '0x' attr(data-hex);
            position: absolute;
            bottom: 5px;
            right: 5px;
            font-size: 0.6rem;
            opacity: 0.3;
        }
        
        /* Contact matrix */
        .contact-matrix {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2px;
            background: #00ffaa20;
            padding: 2px;
            margin: 40px 0;
        }
        
        .contact-item {
            background: #0a0a0f;
            padding: 25px;
            text-align: center;
            text-decoration: none;
            color: #00ffaa;
            border: 1px solid transparent;
            transition: 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .contact-item:hover {
            border-color: #00ffaa;
            background: #00ffaa10;
        }
        
        .contact-item .key {
            font-size: 0.7rem;
            opacity: 0.5;
            margin-top: 10px;
            font-family: monospace;
        }
        
        /* Quantum signature */
        .quantum-signature {
            font-family: monospace;
            font-size: 0.8rem;
            color: #00ffaa60;
            text-align: center;
            margin: 40px 0;
            word-break: break-all;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .glitch-text {
                font-size: 2.5rem;
            }
            
            .stat-value {
                font-size: 2rem;
            }
        }
        
        /* Cursor effect */
        .cursor {
            display: inline-block;
            width: 10px;
            height: 20px;
            background: #00ffaa;
            animation: blink 1s infinite;
            vertical-align: middle;
        }
        
        @keyframes blink {
            0%, 50% { opacity: 1; }
            51%, 100% { opacity: 0; }
        }
        
        /* Hidden text */
        .hidden-text {
            opacity: 0;
            position: absolute;
            pointer-events: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Quantum Header -->
        <div class="quantum-header">
            <div class="matrix-rain" id="matrixRain"></div>
            <div class="binary-row" id="binaryStream"></div>
            <div style="margin-bottom: 20px; font-size: 0.8rem; opacity: 0.5;">
                QUANTUM SECURITY CORE v4.2.0 // 0x7F1C3A9B // ENCRYPTION: POST-QUANTUM
            </div>
            <div class="glitch-text">ZWANSKI</div>
            <div style="font-size: 1.2rem; margin: 20px 0; letter-spacing: 5px;">
                ⚡ QUANTUM SECURITY DIVISION ⚡
            </div>
            <div style="display: flex; gap: 20px; flex-wrap: wrap;">
                <div style="border-right: 1px solid #00ffaa40; padding-right: 20px;">
                    <span style="opacity: 0.5;">STATUS:</span> 
                    <span style="color: #00ffaa;">OPERATIONAL</span>
                </div>
                <div style="border-right: 1px solid #00ffaa40; padding-right: 20px;">
                    <span style="opacity: 0.5;">THREAT LEVEL:</span> 
                    <span style="color: #ffaa00;">🜁 QUANTUM</span>
                </div>
                <div>
                    <span style="opacity: 0.5;">SESSION:</span> 
                    <span>[▓▓▓▓▓▓▓▓▓▓] 2048-bit</span>
                </div>
            </div>
        </div>

        <!-- Quantum Stats -->
        <div class="stats-grid">
            <div class="stat-item">
                <div class="stat-value">0x7F</div>
                <div class="stat-label">QUANTUM ID</div>
            </div>
            <div class="stat-item">
                <div class="stat-value">47</div>
                <div class="stat-label">ZERO-DAYS</div>
            </div>
            <div class="stat-item">
                <div class="stat-value">128</div>
                <div class="stat-label">CVEs</div>
            </div>
            <div class="stat-item">
                <div class="stat-value">9.9</div>
                <div class="stat-label">CVSS AVG</div>
            </div>
            <div class="stat-item">
                <div class="stat-value">∞</div>
                <div class="stat-label">UPTIME</div>
            </div>
        </div>

        <!-- Core Visualization -->
        <div class="core-container">
            <div class="core"></div>
        </div>

        <!-- Holographic Profile -->
        <div class="hologram">
            <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap;">
                <div>
                    <div style="font-size: 0.7rem; opacity: 0.5; margin-bottom: 5px;">// OPERATOR</div>
                    <div style="font-size: 2rem; font-weight: 900;">MOHAMED IBRAHIM</div>
                    <div style="font-size: 1rem; opacity: 0.7; margin: 10px 0;">ALIAS: ZWANSKI</div>
                </div>
                <div style="text-align: right;">
                    <div style="font-size: 0.7rem; opacity: 0.5;">CLEARANCE</div>
                    <div style="font-size: 1.5rem;">OMEGA-7</div>
                </div>
            </div>
            
            <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 20px; margin-top: 30px;">
                <div>
                    <div style="font-size: 0.7rem; opacity: 0.5;">PRIMARY</div>
                    <div>QUANTUM EXPLOITATION</div>
                    <div style="height: 2px; width: 100%; background: linear-gradient(90deg, #00ffaa, transparent); margin: 5px 0;"></div>
                    <div>NEURAL NETWORK PENTEST</div>
                </div>
                <div>
                    <div style="font-size: 0.7rem; opacity: 0.5;">SECONDARY</div>
                    <div>QUANTUM CRYPTOGRAPHY</div>
                    <div style="height: 2px; width: 100%; background: linear-gradient(90deg, #00ffaa, transparent); margin: 5px 0;"></div>
                    <div>AI ADVERSARIAL</div>
                </div>
                <div>
                    <div style="font-size: 0.7rem; opacity: 0.5;">TERTIARY</div>
                    <div>QUANTUM REVERSE</div>
                    <div style="height: 2px; width: 100%; background: linear-gradient(90deg, #00ffaa, transparent); margin: 5px 0;"></div>
                    <div>DNA COMPUTING</div>
                </div>
            </div>
        </div>

        <!-- Command Line Interface -->
        <div class="command-line">
            <div style="margin-bottom: 10px;">┌──(zwanski㉿quantum-core)-[~]</div>
            <div style="margin-bottom: 10px;">└─$ ./deploy --quantum --stealth</div>
            <div style="color: #00ffaa;">[✓] QUANTUM ENTANGLEMENT ESTABLISHED</div>
            <div style="color: #00ffaa;">[✓] SUPERPOSITION ACTIVE</div>
            <div style="color: #00ffaa;">[✓] OBSERVER EFFECT NEUTRALIZED</div>
            <div style="color: #ffaa00;">[!] REALITY DISTORTION FIELD: 93%</div>
            <div style="margin-top: 10px;">
                <span style="opacity: 0.5;">λ quantum > </span>_<span class="cursor"></span>
            </div>
        </div>

        <!-- Fingerprint Grid -->
        <div class="fingerprint-grid">
            <div class="fingerprint-cell" data-hex="A1"></div>
            <div class="fingerprint-cell" data-hex="B2"></div>
            <div class="fingerprint-cell" data-hex="C3"></div>
            <div class="fingerprint-cell" data-hex="D4"></div>
            <div class="fingerprint-cell" data-hex="E5"></div>
            <div class="fingerprint-cell" data-hex="F6"></div>
            <div class="fingerprint-cell" data-hex="7A"></div>
            <div class="fingerprint-cell" data-hex="8B"></div>
            <div class="fingerprint-cell" data-hex="9C"></div>
            <div class="fingerprint-cell" data-hex="0D"></div>
            <div class="fingerprint-cell" data-hex="1E"></div>
            <div class="fingerprint-cell" data-hex="2F"></div>
            <div class="fingerprint-cell" data-hex="3A"></div>
            <div class="fingerprint-cell" data-hex="4B"></div>
            <div class="fingerprint-cell" data-hex="5C"></div>
            <div class="fingerprint-cell" data-hex="6D"></div>
            <div class="fingerprint-cell" data-hex="7E"></div>
            <div class="fingerprint-cell" data-hex="8F"></div>
            <div class="fingerprint-cell" data-hex="9A"></div>
            <div class="fingerprint-cell" data-hex="0B"></div>
        </div>

        <!-- Contact Matrix -->
        <div class="contact-matrix">
            <a href="#" class="contact-item">
                <div style="font-size: 2rem;">⌘</div>
                <div>QUANTUM MAIL</div>
                <div class="key">mohaaibb4@proton.me</div>
                <div class="key">PGP: 0x7F3A9C1B</div>
            </a>
            <a href="#" class="contact-item">
                <div style="font-size: 2rem;">⌥</div>
                <div>QUANTUM NODE</div>
                <div class="key">zwanski-store.pages.dev</div>
                <div class="key">IPv6: 2001:db8::7331</div>
            </a>
            <a href="#" class="contact-item">
                <div style="font-size: 2rem;">⇧</div>
                <div>QUANTUM SIGNAL</div>
                <div class="key">+216 94 934 141</div>
                <div class="key">ENCRYPTED</div>
            </a>
            <a href="#" class="contact-item">
                <div style="font-size: 2rem;">⌃</div>
                <div>QUANTUM CHAIN</div>
                <div class="key">@zwanski2019</div>
                <div class="key">0xZERO_DAILY</div>
            </a>
        </div>

        <!-- Quantum Signature -->
        <div class="quantum-signature">
            <div>QUANTUM SIGNATURE // 0x7F3A9C1B8D4E2F5A6C7B8D9E0F1A2B3C4D5E6F7A8B9C0D1E2F3A4B5C6D7E8F9A0B1C2D3E4F5A6B7C8D9E0F</div>
            <div style="margin: 20px 0;">⚡ HASH: 7f3a9c1b8d4e2f5a6c7b8d9e0f1a2b3c4d5e6f7a8b9c0d1e2f3a4b5c6d7e8f9a0b1c2d3e4f5a6b7c8d9e0f ⚡</div>
            <div>© 2026 ZWANSKI QUANTUM SECURITY // ALL RIGHTS RESERVED // 0x7F</div>
        </div>

        <!-- Binary Stream Generator -->
        <div class="hidden-text">
            <span id="binaryData"></span>
        </div>
    </div>

    <script>
        // Matrix rain effect
        function createMatrixRain() {
            const container = document.getElementById('matrixRain');
            for (let i = 0; i < 50; i++) {
                const span = document.createElement('span');
                span.style.left = Math.random() * 100 + '%';
                span.style.animationDelay = Math.random() * 10 + 's';
                span.style.animationDuration = 5 + Math.random() * 10 + 's';
                span.innerHTML = String.fromCharCode(0x30A0 + Math.random() * 96);
                container.appendChild(span);
            }
        }

        // Binary stream generator
        function generateBinary() {
            const stream = document.getElementById('binaryStream');
            setInterval(() => {
                let binary = '';
                for (let i = 0; i < 20; i++) {
                    binary += Math.random() > 0.5 ? '1' : '0';
                }
                stream.innerHTML = binary + ' ' + binary + ' ' + binary;
            }, 100);
        }

        // Quantum random number generator (simulated)
        function quantumRandom() {
            return Math.floor(Math.random() * 0x7FFFFFFF).toString(16);
        }

        // Update stats with quantum randomness
        setInterval(() => {
            const stats = document.querySelectorAll('.stat-value');
            stats.forEach(stat => {
                if (stat.innerText !== '∞' && stat.innerText !== '0x7F') {
                    const random = Math.floor(Math.random() * 100);
                    stat.style.opacity = 0.5 + Math.random() * 0.5;
                }
            });
        }, 2000);

        // Initialize
        createMatrixRain();
        generateBinary();

        // Console message
        console.log('%c🔐 ZWANSKI QUANTUM SECURITY CORE // ACCESS GRANTED', 
                    'color: #00ffaa; font-size: 16px; font-weight: bold;');
        console.log('%cSESSION HASH: ' + quantumRandom() + quantumRandom(), 
                    'color: #00ffaa80; font-size: 12px;');
    </script>
</body>
</html>
