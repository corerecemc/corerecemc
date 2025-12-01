<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>COREREC - electronic music creations</title>

    <style>
        /* --- Global Reset --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0b0b0b;
            color: #fff;
            font-family: "Arial", sans-serif;
            overflow-x: hidden;
            scroll-behavior: auto; /* verhindert scroll animation beim laden */
        }

        /* --- Header / Navigation --- */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            height: 110px;
            background: rgba(255, 255, 255, 0.10);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0 40px;
            z-index: 2000;
        }

        .logo {
            font-size: 28px;
            font-weight: 700;
            letter-spacing: 1px;
            color: #fff;
        }

        .main-menu ul {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .main-menu a {
            text-decoration: none;
            color: #fff;
            font-size: 18px;
            transition: color 0.25s ease;
        }

        .main-menu a:hover {
            color: #ff0055;
        }

        /* --- Social Icons --- */
        .social-icons {
            display: flex;
            align-items: center;
            gap: 18px;
            height: 100%;
        }

        .social-icons img {
            width: 30px;
            height: 30px;
            object-fit: contain;
            transition: transform 0.2s ease;
            filter: invert(1);
        }

        .social-icons img:hover {
            transform: scale(1.3);
        }

        /* --- Sections Layout --- */
        section {
            width: 100%;
            max-width: 1400px;
            margin: 150px auto 80px auto;
            padding: 0 40px;
        }

        section h2 {
            font-size: 32px;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .image-block {
            width: 100%;
            margin: 30px 0;
        }

        .image-block img {
            width: 100%;
            border-radius: 12px;
        }

        /* --- Footer --- */
        footer {
            text-align: center;
            padding: 50px 0;
            font-size: 14px;
            opacity: 0.6;
        }

        /* --- Mobile --- */
        @media (max-width: 768px) {
            header {
                height: 90px;
                padding: 0 20px;
            }

            .main-menu ul {
                gap: 20px;
            }

            .main-menu a {
                font-size: 16px;
            }

            .social-icons img {
                width: 26px;
                height: 26px;
            }

            section {
                padding: 0 20px;
            }
        }
    </style>
</head>

<body id="top">

    <!-- HEADER -->
    <header>
        <div class="logo">COREREC</div>

        <nav class="main-menu">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#releases">Releases</a></li>
                <li><a href="#artists">Artists</a></li>
                <li><a href="#shop">Shop</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>

        <div class="social-icons">
            <a href="https://facebook.com" target="_blank">
                <img src="icons/facebook.svg" alt="Facebook">
            </a>
            <a href="https://instagram.com" target="_blank">
                <img src="icons/instagram.svg" alt="Instagram">
            </a>
            <a href="https://youtube.com" target="_blank">
                <img src="icons/youtube.svg" alt="YouTube">
            </a>
        </div>
    </header>

    <!-- SECTIONS -->
    <section id="home">
        <h2>Welcome to COREREC</h2>
        <div class="image-block">
            <img src="images/home.jpg" alt="Home Image">
        </div>
        <p>Electronic music creations – hard, dark, industrial, cinematic.</p>
    </section>

    <section id="releases">
        <h2>Latest Releases</h2>
        <div class="image-block">
            <img src="images/releases.jpg" alt="Releases">
        </div>
        <p>Here you will find all EPs, singles and collaborations.</p>
    </section>

    <section id="artists">
        <h2>Artists</h2>
        <div class="image-block">
            <img src="images/artists.jpg" alt="Artists">
        </div>
        <p>The creators behind the COREREC sound.</p>
    </section>

    <section id="shop">
        <h2>Shop</h2>
        <div class="image-block">
            <img src="images/shop.jpg" alt="Shop">
        </div>
        <p>Merch, downloads and more coming soon.</p>
    </section>

    <section id="contact">
        <h2>Contact</h2>
        <div class="image-block">
            <img src="images/contact.jpg" alt="Contact">
        </div>
        <p>For booking, releases or collaborations – get in touch.</p>
    </section>

    <footer>
        © 2025 COREREC – All rights reserved.
    </footer>

    <!-- Scroll to top on load robust -->
    <script>
    window.onload = function() {
        // Direkt auf den oberen Rand scrollen
        document.documentElement.scrollTop = 0;
        document.body.scrollTop = 0;
    };
    </script>

</body>
</html>
