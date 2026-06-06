
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mahal</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@600&family=Poppins:wght@300;400;600&display=swap');

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: #03071e;
            color: #f8f9fa;
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* --- Audio Player Container --- */
        .audio-container {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.1);
            padding: 10px;
            border-radius: 30px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 215, 0, 0.3);
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }

        /* --- Hero Section --- */
        header {
            background: linear-gradient(rgba(3, 7, 30, 0.6), rgba(3, 7, 30, 0.85)), url('CD8FBE85-0CF8-4EC7-8078-7DEE3C62B10C.jpg') no-repeat center center/cover;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
        }

        /* Twinkling Star Background Effect */
        header::before {
            content: "";
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background: transparent url('https://www.transparenttextures.com/patterns/stardust.png') repeat;
            opacity: 0.6;
            pointer-events: none;
        }

        header h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 5rem;
            color: #ffd700;
            margin-bottom: 15px;
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.6);
            animation: float 3s ease-in-out infinite;
        }

        header p {
            font-size: 1.4rem;
            font-weight: 300;
            color: #e9ecef;
            text-shadow: 1px 1px 4px rgba(0,0,0,0.8);
        }

        /* --- Story Section --- */
        #story {
            padding: 80px 0;
            text-align: center;
            background: linear-gradient(#03071e, #0a0f24);
        }

        .section-title {
            font-family: 'Dancing Script', cursive;
            font-size: 3.5rem;
            color: #ffd700;
            margin-bottom: 30px;
            text-shadow: 0 0 10px rgba(255, 215, 0, 0.3);
        }

        /* --- Photo Gallery --- */
        #gallery {
            padding: 60px 0;
            background: #0a0f24;
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            padding: 0 10px;
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.5);
            height: 380px;
            border: 1px solid rgba(255, 215, 0, 0.1);
            transition: all 0.4s ease;
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.6s ease;
        }

        .gallery-item:hover {
            border-color: #ffd700;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.4);
            transform: translateY(-5px);
        }

        .gallery-item:hover img {
            transform: scale(1.05);
        }

        /* --- Love Note Section --- */
        #message {
            padding: 100px 0;
            background: linear-gradient(rgba(10, 15, 36, 0.9), rgba(3, 7, 30, 0.95)), url('IMG_9165.jpg') no-repeat center center/cover;
            text-align: center;
            border-top: 1px solid rgba(255, 215, 0, 0.2);
        }

        .message-box {
            max-width: 750px;
            margin: 0 auto;
            font-size: 1.3rem;
            font-style: italic;
            line-height: 2;
            color: #f8f9fa;
            padding: 20px;
        }

        /* --- Footer --- */
        footer {
            background-color: #03071e;
            color: rgba(255,255,255,0.5);
            text-align: center;
            padding: 40px 0;
            font-size: 0.9rem;
            border-top: 1px solid rgba(255,255,255,0.05);
        }

        footer span {
            color: #ffd700;
        }

        /* --- Keyframes --- */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        @media(max-width: 768px) {
            header h1 { font-size: 3.5rem; }
            header p { font-size: 1.1rem; }
            .section-title { font-size: 2.8rem; }
        }
    </style>
</head>
<body>

    <div class="audio-container">
        <audio controls loop autoplay>
            <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
    </div>

    <header>
        <div>
            <h1>Our Magical World</h1>
            <p>Every single moment spent with you feels exactly like a fairytale.</p>
        </div>
    </header>

    <section id="story">
        <div class="container">
            <h2 class="section-title">Our Captured Memories</h2>
        </div>
    </section>

    <section id="gallery">
        <div class="container">
            <div class="gallery-grid">
                <div class="gallery-item">
                    <img src="IMG_8795.jpg" alt="Sweet smiles together">
                </div>
                <div class="gallery-item">
                    <img src="IMG_8939.jpg" alt="Forehead kiss at night">
                </div>
                <div class="gallery-item">
                    <img src="IMG_9165.jpg" alt="Beautiful landscape backdrop">
                </div>
                <div class="gallery-item">
                    <img src="IMG_9373.jpg" alt="Cozy theater moments">
                </div>
                <div class="gallery-item">
                    <img src="AEBC7C12-0E39-4B00-92C4-85D911AC1801.jpg" alt="Dancing by the twilight tent">
                </div>
                <div class="gallery-item">
                    <img src="C73AEB35-6A58-44F6-B38D-2C66C4461D94.jpg" alt="Watching the golden hour sunset">
                </div>
                <div class="gallery-item">
                    <img src="130377e14a367c6720d77aed66dfcb93.jpeg" alt="Making a heart under the sky">
                </div>
                <div class="gallery-item">
                    <img src="ef304e081acca9f8f270260157ab2707.jpeg" alt="Hand in hand into the sunset">
                </div>
            </div>
        </div>
    </section>

    <section id="message">
        <div class="container">
            <h2 class="section-title">I Love You So Much</h2>
            <div class="message-box">
                <p>"You are my favorite song, my brightest star, and my home. No matter where we go or what we do, my heart is completely yours forever and always. Thank you for loving me."</p>
            </div>
        </div>
    </section>

    <footer>
        <p>Made with magic and <span>✨</span> for my favorite person.</p>
    </footer>

</body>
</html>
