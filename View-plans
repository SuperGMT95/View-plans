<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CoreMMC Hosting</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        /* Base Body & Layout */
        body {
            font-family: 'Arial', sans-serif;
            color: #fff;
            line-height: 1.6;
            margin: 0;
            padding: 50px 20px;
            overflow-x: hidden;
            background: #050816;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* --- New Animated Background --- */
        .background { 
            position: fixed; 
            inset: -20px;
            background: url('https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExNTg0d2ZyaXRlZGJqeXVmNG5ra2JocTZ2eno2OGp5YjhtZjhpeGNqcCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/JNySPj69tVEEaaqoa9/giphy.gif') center/cover; 
            filter: blur(8px) brightness(0.5); 
            z-index: -1; 
        }

        /* --- Snowfall Effect --- */
        .snowflake {
            position: fixed;
            top: -10px;
            z-index: 10;
            font-size: 1.2em;
            color: #fff;
            opacity: 0.8;
            user-select: none;
            pointer-events: none;
            animation: fall linear infinite;
        }

        @keyframes fall {
            0% { transform: translateY(0vh) translateX(0px); }
            100% { transform: translateY(110vh) translateX(20px); }
        }

        /* Main Section */
        .hosting-section {
            max-width: 1100px;
            width: 100%;
            z-index: 2;
        }

        .header {
            text-align: left;
            margin-bottom: 40px;
        }

        .header h1 { font-size: 2.8rem; margin: 0; }
        .header p { color: #ccc; }

        /* Pricing Grid */
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 20px;
        }

        /* Glassmorphism Cards */
        .card {
            background: rgba(22, 27, 34, 0.7);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 30px;
            position: relative;
            transition: 0.3s;
        }

        .card:hover { transform: translateY(-10px); border-color: rgba(255, 255, 255, 0.3); }

        .popular { border: 2px solid #a371f7; }
        .badge {
            position: absolute; top: 15px; right: 15px;
            background: #a371f7; font-size: 10px; padding: 4px 10px; border-radius: 20px;
        }

        .price { font-size: 1.1rem; margin: 20px 0; color: #8b949e; }
        .price span { font-size: 2rem; font-weight: bold; color: #fff; }

        .vps .price span { color: #2188ff; }
        .minecraft .price span { color: #a371f7; }
        .bot .price span { color: #e3b341; }
        .web .price span { color: #3fb950; }

        .features { list-style: none; padding: 0; margin-bottom: 30px; }
        .features li { margin-bottom: 12px; font-size: 0.9rem; color: #d1d5db; display: flex; align-items: center; }
        .features i { margin-right: 12px; width: 20px; color: #58a6ff; }

        /* Buttons */
        .btn {
            width: 100%; padding: 12px; border-radius: 10px; border: none;
            cursor: pointer; font-weight: bold; transition: 0.3s;
        }
        .btn-mc { background: #a371f7; color: white; }
        .btn-outline { background: transparent; border: 1px solid #444; color: white; }
        .btn:hover { filter: brightness(1.2); }

    </style>
</head>
<body>

    <div class="background"></div>

    <section class="hosting-section">
        <div class="header">
            <h1>Our Hosting Solutions</h1>
            <p>Select the perfect infrastructure for your project.</p>
        </div>

        <div class="pricing-grid">
            <div class="card vps">
                <h3>VPS Hosting</h3>
                <div class="price">Starts at <span>₹45</span> / GB RAM</div>
                <ul class="features">
                    <li><i class="fas fa-terminal"></i> Full Root Access</li>
                    <li><i class="fas fa-network-wired"></i> 1 Gbps Network</li>
                    <li><i class="fas fa-hdd"></i> Gen4 NVMe</li>
                </ul>
                <button class="btn btn-outline">Configure VPS</button>
            </div>

            <div class="card minecraft popular">
                <span class="badge">POPULAR</span>
                <h3>Minecraft</h3>
                <div class="price">Starts at <span>₹25</span> / GB RAM</div>
                <ul class="features">
                    <li><i class="fas fa-users"></i> Unlimited Slots</li>
                    <li><i class="fas fa-bolt"></i> Ryzen-Powered</li>
                    <li><i class="fas fa-shield-alt"></i> Dedicated IP</li>
                </ul>
                <button class="btn btn-mc">Launch Server</button>
            </div>

            <div class="card bot">
                <h3>Bot Hosting</h3>
                <div class="price">Starts at <span>₹20</span> / GB RAM</div>
                <ul class="features">
                    <li><i class="fas fa-code"></i> Python & Node.js</li>
                    <li><i class="fas fa-clock"></i> 24/7 Uptime</li>
                    <li><i class="fas fa-folder"></i> FTP Access</li>
                </ul>
                <button class="btn btn-outline">Start Bot</button>
            </div>

            <div class="card web">
                <h3>Web Hosting</h3>
                <div class="price"><span>Free</span> to Start</div>
                <ul class="features">
                    <li><i class="fas fa-lock"></i> Free SSL</li>
                    <li><i class="fas fa-columns"></i> CyberPanel</li>
                    <li><i class="fas fa-envelope"></i> Pro Email</li>
                </ul>
                <button class="btn btn-outline">Host Website</button>
            </div>
        </div>
    </section>

    <script>
        function createSnowflake() {
            const snowflake = document.createElement('div');
            snowflake.classList.add('snowflake');
            snowflake.innerHTML = '❄';
            snowflake.style.left = Math.random() * 100 + 'vw';
            snowflake.style.animationDuration = Math.random() * 3 + 2 + 's';
            snowflake.style.opacity = Math.random();
            snowflake.style.fontSize = Math.random() * 1.5 + 0.5 + 'em';
            
            document.body.appendChild(snowflake);

            setTimeout(() => {
                snowflake.remove();
            }, 5000);
        }

        setInterval(createSnowflake, 200);
    </script>
</body>
</html>
