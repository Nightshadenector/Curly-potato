<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy 6 Months My Love ❤️</title>
    <!-- Canvas Confetti CDN -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #ff4b72;
            --secondary: #ff85a2;
            --accent: #ffe6eb;
            --dark: #2a0812;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #ffe6eb 0%, #ffd1dc 100%);
            color: var(--dark);
            overflow-x: hidden;
            text-align: center;
        }

        /* Floating Hearts Animation */
        .heart {
            position: fixed;
            color: var(--primary);
            font-size: 20px;
            animation: float 6s linear infinite;
            z-index: 0;
            opacity: 0.6;
        }

        @keyframes float {
            0% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
            100% { transform: translateY(-10vh) rotate(360deg); opacity: 0; }
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            position: relative;
            z-index: 1;
        }

        header {
            margin-bottom: 50px;
            animation: fadeIn 2s ease-in-out;
        }

        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5rem;
            color: var(--primary);
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
            margin-bottom: 20px;
        }

        .hero-poem {
            background: rgba(255, 255, 255, 0.85);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(255, 75, 114, 0.2);
            backdrop-filter: blur(5px);
            font-style: italic;
            font-size: 1.1rem;
            line-height: 1.8;
            margin-bottom: 40px;
            border: 2px solid var(--secondary);
        }

        .section-title {
            font-family: 'Dancing Script', cursive;
            font-size: 2.8rem;
            color: var(--primary);
            margin: 40px 0 20px;
        }

        /* Memories Section */
        .memories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }

        .memory-card {
            background: white;
            padding: 15px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
        }

        .memory-card:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: 0 12px 25px rgba(255, 75, 114, 0.3);
        }

        .memory-card img {
            width: 100%;
            border-radius: 10px;
            object-fit: cover;
            margin-bottom: 10px;
        }

        .memory-card p {
            font-size: 0.95rem;
            font-weight: 600;
            color: var(--primary);
        }

        .paradise-note {
            font-family: 'Dancing Script', cursive;
            font-size: 2rem;
            color: var(--dark);
            margin: 30px 0 50px;
            background: rgba(255, 255, 255, 0.6);
            padding: 20px;
            border-radius: 15px;
        }

        /* Open When Cards */
        .letters-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
        }

        .envelope-btn {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: white;
            border: none;
            padding: 20px 30px;
            border-radius: 15px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(255, 75, 114, 0.4);
            transition: all 0.3s ease;
            flex: 1 1 250px;
            max-width: 280px;
        }

        .envelope-btn:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(255, 75, 114, 0.6);
        }

        /* Modal Overlay */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 100;
            padding: 20px;
        }

        .modal-content {
            background: white;
            padding: 30px;
            border-radius: 20px;
            max-width: 600px;
            width: 100%;
            max-height: 80vh;
            overflow-y: auto;
            position: relative;
            box-shadow: 0 10px 30px rgba(0,0,0,0.3);
            animation: popUp 0.3s ease-out;
            text-align: left;
            line-height: 1.8;
        }

        @keyframes popUp {
            from { transform: scale(0.8); opacity: 0; }
            to { transform: scale(1); opacity: 1; }
        }

        .close-btn {
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 1.8rem;
            color: var(--primary);
            cursor: pointer;
            font-weight: bold;
        }

        .modal-content h3 {
            font-family: 'Dancing Script', cursive;
            font-size: 2.2rem;
            color: var(--primary);
            margin-bottom: 15px;
            text-align: center;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-20deg); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Happy Six Months, My Love! ❤️</h1>
            <div class="hero-poem">
                "Across the miles and through the screen,<br>
                You are the sweetest dream I’ve ever seen.<br>
                Six months of laughter, late-night calls and sighs,<br>
                Of finding my whole world inside your eyes.<br>
                Distance is heavy, but my love is true,<br>
                Every beat of my heart belongs only to you." 💖
            </div>
        </header>

        <section>
            <h2 class="section-title">Our Top 6 Favorite Memories 💕</h2>
            <div class="memories-grid">
                <!-- Memory 1 -->
                <div class="memory-card">
                    <img src="image1.png" alt="Memory 1">
                    <p>1. "I missed you too baby" — Reunited in VC 🎧</p>
                </div>
                <!-- Memory 2 -->
                <div class="memory-card">
                    <img src="image2.png" alt="Memory 2">
                    <p>2. "Why is my phone always at 4%" 📱💔</p>
                </div>
                <!-- Memory 3 -->
                <div class="memory-card">
                    <img src="image3.png" alt="Memory 3">
                    <p>3. "I love you too mwaaaahhhhh" 😘</p>
                </div>
                <!-- Memory 4 -->
                <div class="memory-card">
                    <img src="image4.png" alt="Memory 4">
                    <p>4. "You are my Walmart Miku :)" 💙</p>
                </div>
                <!-- Memory 5 -->
                <div class="memory-card">
                    <img src="image5.png" alt="Memory 5">
                    <p>5. "Lobster spotted, time to eat >:)" 🦞❤️</p>
                </div>
                <!-- Memory 6 -->
                <div class="memory-card">
                    <img src="image6.png" alt="Memory 6">
                    <p>6. 7-Hour Calls & Dreaming of Us 🌙✨</p>
                </div>
            </div>

            <div class="paradise-note">
                ✨ "I wish I could mention every single moment with you here, because every moment with you is pure paradise!" ✨
            </div>
        </section>

        <!-- Open When Section -->
        <section>
            <h2 class="section-title">Letters For You ✉️</h2>
            <div class="letters-section">
                <button class="envelope-btn" onclick="openModal('modal1')">💌 Open When You Miss Me</button>
                <button class="envelope-btn" onclick="openModal('modal2')">🎉 Open On Our Anniversary</button>
                <button class="envelope-btn" onclick="openModal('modal3')">🌙 Open When Sleepy</button>
            </div>
        </section>
    </div>

    <!-- Modals -->
    <!-- Modal 1: Miss Me -->
    <div id="modal1" class="modal-overlay" onclick="closeModalOnOutside(event, 'modal1')">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('modal1')">&times;</span>
            <h3>Call Me Right Now, My Love! 📞❤️</h3>
            <p style="text-align: center;">If you're reading this and missing me, don't hesitate for even a second. Pick up the phone and call me right now! I am always waiting to hear your voice, no matter what time it is. You are my home, and I miss you just as much!</p>
        </div>
    </div>

    <!-- Modal 2: Anniversary Poem -->
    <div id="modal2" class="modal-overlay" onclick="closeModalOnOutside(event, 'modal2')">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('modal2')">&times;</span>
            <h3>6 Months of Endless Love 📜✨</h3>
            <p>My dearest husband,</p><br>
            <p>Six months ago, you walked into my life and completely reshaped my world. In these 180 days, you have given me a sanctuary in your voice, comfort in your sweetest words, and a love deeper than I ever thought possible.</p><br>
            <p><em>"We count the seconds, hours, and days,<br>
            Lost in a long-distance lovers' maze.<br>
            Yet every call, every 'I love you' whispered low,<br>
            Makes my heart swell and my passion grow.<br>
            These six months brought us closer than ever before,<br>
            And every single day I love you even more.<br>
            I count every heartbeat until the day we meet,<br>
            When holding you tight will finally feel complete."</em></p><br>
            <p>Thank you for being my safe place, my best friend, and my whole heart. Happy 6 months, my love!</p>
        </div>
    </div>

    <!-- Modal 3: Sleepy -->
    <div id="modal3" class="modal-overlay" onclick="closeModalOnOutside(event, 'modal3')">
        <div class="modal-content">
            <span class="close-btn" onclick="closeModal('modal3')">&times;</span>
            <h3>Sweet Dreams, Baby 😴✨</h3>
            <p style="text-align: center;">Go to sleep baby, I’m loving you from the dream world! Close your eyes, rest your head, and know that even as you sleep, my heart is right there holding you tight. Goodnight, my entire world. 🤍☁️</p>
        </div>
    </div>

    <script>
        // Automatic Confetti Trigger on Load
        window.addEventListener('DOMContentLoaded', () => {
            var count = 200;
            var defaults = {
                origin: { y: 0.7 }
            };

            function fire(particleRatio, opts) {
                confetti(Object.assign({}, defaults, opts, {
                    particleCount: Math.floor(count * particleRatio)
                }));
            }

            fire(0.25, { spread: 26, startVelocity: 55, });
            fire(0.2, { spread: 60, });
            fire(0.35, { spread: 100, decay: 0.91, scalar: 0.8 });
            fire(0.1, { spread: 120, startVelocity: 25, decay: 0.92, scalar: 1.2 });
            fire(0.1, { spread: 120, startVelocity: 45, });
        });

        // Floating Hearts Background Generator
        function createHearts() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 3 + 3 + 's';
            document.body.appendChild(heart);
            setTimeout(() => heart.remove(), 6000);
        }
        setInterval(createHearts, 400);

        // Modal Controls
        function openModal(id) {
            document.getElementById(id).style.display = 'flex';
        }

        function closeModal(id) {
            document.getElementById(id).style.display = 'none';
        }

        function closeModalOnOutside(event, id) {
            if (event.target.id === id) {
                closeModal(id);
            }
        }
    </script>
</body>
</html>

