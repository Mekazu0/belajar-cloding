<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Belajar Cloding</title>
    <meta name="description" content="Belajar Cloding adalah platform untuk belajar pemrograman dan pengembangan web. Temukan tutorial dan informasi berguna untuk meningkatkan keterampilan Anda.">
    <meta name="keywords" content="belajar, pemrograman, pengembangan web, tutorial, coding">
    <meta name="author" content="Nama Anda">
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            line-height: 1.6;
            background-color: #f4f4f4;
        }
        header {
            background-color: #4CAF50;
            padding: 2rem 1rem;
            color: white;
            text-align: center;
            position: relative;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        header h1 {
            font-size: 2.5rem;
            margin-bottom: 1.5rem;
        }
        .menu-icon {
            display: block;
            cursor: pointer;
            padding: 10px;
            position: absolute;
            left: 50px; /* Adjusted to make space for the search icon */
            top: 10px;
        }
        .menu-icon div {
            width: 30px;
            height: 3px;
            background-color: white;
            margin: 5px 0;
        }
        .search-container {
            position: absolute;
            right: 10px;
            top: 10px;
            display: flex;
            align-items: center;
        }
        .search-container input[type="text"] {
            padding: 0.5rem;
            border: none;
            border-radius: 5px;
            width: 200px; /* Atur lebar sesuai kebutuhan */
            margin-right: 5px;
        }
        .search-container button {
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 0.5rem 0.7rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .search-container button:hover {
            background-color: #45a049;
        }
        .dropdown {
            display: none;
            flex-direction: column;
            background-color: #333;
            position: absolute;
            top: 60px;
            left: 10px;
            border-radius: 5px;
            z-index: 1;
        }
        .dropdown a {
            color: white;
            padding: 10px;
            text-decoration: none;
            display: block;
            transition: background-color 0.3s;
        }
        .dropdown a:hover {
            background-color: #45a049;
        }
        .container {
            padding: 2rem;
            max-width: 800px;
            margin: auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem 0;
            position: relative;
        }
        .footer-links a {
            color: white;
            text-decoration: none;
            margin: 0 1rem;
            transition: color 0.3s;
        }
        .footer-links a:hover {
            color: #4CAF50;
        }
        form {
            display: flex;
            flex-direction: column;
            max-width: 500px;
            margin: 0 auto;
            background: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        form label {
            margin: 0.5rem 0 0.2rem;
            font-weight: bold;
        }
        form input, form textarea {
            padding: 0.8rem;
            margin-bottom: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            transition: border-color 0.3s;
            width: 100%;
        }
        form input:focus, form textarea:focus {
            border-color: #4CAF50;
            outline: none;
        }
        form button {
            background-color: #4CAF50;
            color: white;
            padding: 0.7rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }
        form button:hover {
            background-color: #45a049;
        }
        #cookie-consent-banner {
            position: fixed;
            bottom: 0;
            left: 0;
            right: 0;
            background-color: #333;
            color: white;
            padding: 1rem;
            text-align: center;
            z-index: 1000;
            display: none;
        }
        #cookie-consent-banner button {
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 0.5rem 1rem;
            cursor: pointer;
            margin-left: 1rem;
        }
        #cookie-consent-banner button:hover {
            background-color: #45a049;
        }

        /* Media Queries untuk Responsivitas */
        @media (max-width: 600px) {
            header h1 {
                font-size: 2rem;
            }
        }

        @media (min-width: 601px) {
            .menu-icon {
                margin-top: 2rem;
            }
        }

        @media (min-width: 900px) {
            header h1 {
                font-size: 2.5rem;
            }
            .menu-icon {
                margin-top: 3rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Selamat Datang di Belajar Cloding</h1>
        <div class="search-container">
            <input type="text" placeholder="Cari..." name="search">
            <button type="submit"><i class="fas fa-search"></i></button>
        </div>
        <div class="menu-icon" onclick="toggleDropdown()">
            <div></div>
            <div></div>
            <div></div>
        </div>
        <div class="dropdown" id="dropdown">
            <a href="#home">Home</a>
            <a href="#disclaimer">Disclaimer</a>
            <a href="#privacy-policy">Privacy Policy</a>
            <a href="#contact">Contact</a>
        </div>
    </header>
    <div class="container">
        <section id="home">
            <h2>Home</h2>
            <p>Ini adalah halaman utama situs web kami.</p>
        </section>
        <section id="disclaimer">
            <h2>Disclaimer</h2>
            <p>
                Informasi yang terdapat di situs web ini disediakan hanya untuk tujuan informasi umum. 
                Meskipun kami berusaha untuk menjaga informasi yang akurat dan terkini...
            </p>
        </section>
        <section id="privacy-policy">
            <h2>Privacy Policy</h2>
            <p>
                Kami sangat menghargai privasi Anda dan berkomitmen untuk melindungi informasi pribadi Anda...
            </p>
        </section>
        <section id="contact">
            <h2>Contact</h2>
            <p>Jika Anda memiliki pertanyaan atau komentar, silakan hubungi kami melalui formulir di bawah ini:</p>
            <form action="https://formspree.io/f/YOUR_ENDPOINT" method="POST">
                <label for="name">Nama:</label>
                <input type="text" id="name" name="name" required>
                
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                
                <label for="message">Pesan:</label>
                <textarea id="message" name="message" rows="4" required></textarea>
                
                <button type="submit">Kirim</button>
            </form>
        </section>
    </div>

    <!-- Cookie Consent Banner -->
    <div id="cookie-consent-banner">
        <p>
            Kami menggunakan cookies untuk meningkatkan pengalaman Anda di situs kami. 
            Dengan melanjutkan menggunakan situs ini, Anda setuju dengan penggunaan cookies kami.
            <button id="accept-cookies">Setuju</button>
        </p>
    </div>

    <footer>
        <div class="footer-links">
            <a href="#home">Home</a> |
            <a href="#disclaimer">Disclaimer</a> |
            <a href="#privacy-policy">Privacy Policy</a> |
            <a href="#contact">Contact</a>
        </div>
        <p>&copy; 2025 Belajar Cloding. All rights reserved.</p>
    </footer>

    <script>
        function toggleDropdown() {
            const dropdown = document.getElementById('dropdown');
            dropdown.style.display = dropdown.style.display === 'flex' ? 'none' : 'flex';
        }

        document.addEventListener("DOMContentLoaded", function() {
            const cookieBanner = document.getElementById('cookie-consent-banner');
            const acceptButton = document.getElementById('accept-cookies');

            // Cek apakah pengguna sudah memberikan persetujuan
            if (!localStorage.getItem('cookiesAccepted')) {
                cookieBanner.style.display = 'block'; // Tampilkan banner jika belum disetujui
            }

            // Jika pengguna mengklik tombol setuju
            acceptButton.addEventListener('click', function() {
                localStorage.setItem('cookiesAccepted', 'true'); // Simpan persetujuan
                cookieBanner.style.display = 'none'; // Sembunyikan banner
            });
        });
    </script>
</body>
</html>
