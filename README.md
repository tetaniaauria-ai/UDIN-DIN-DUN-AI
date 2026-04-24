<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Anime Library - Koleksi Katalog Pribadi</title>
    <style>
        /* --- CSS INTERNAL --- */
        :root {
            --primary-color: #ff4655; /* Warna aksen merah modern */
            --bg-color: #0f0f0f;
            --card-bg: #1a1a1a;
            --text-main: #ffffff;
            --text-dim: #b3b3b3;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Navigasi / Header */
        header {
            background: linear-gradient(135deg, #1a1a1a 0%, #000000 100%);
            padding: 60px 20px;
            text-align: center;
            border-bottom: 3px solid var(--primary-color);
        }

        header h1 {
            font-size: 2.8rem;
            text-transform: uppercase;
            letter-spacing: 4px;
            margin-bottom: 10px;
        }

        header p {
            color: var(--text-dim);
            font-size: 1.1rem;
        }

        /* Container Katalog */
        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
            gap: 25px;
        }

        /* Kartu Anime */
        .card {
            background-color: var(--card-bg);
            border-radius: 12px;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            border: 1px solid #333;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
        }

        .card:hover {
            transform: translateY(-12px);
            border-color: var(--primary-color);
            box-shadow: 0 10px 25px rgba(255, 70, 85, 0.3);
        }

        .card img {
            width: 100%;
            height: 320px;
            object-fit: cover;
            display: block;
        }

        .card-info {
            padding: 15px;
        }

        .card-info span {
            display: block;
            font-size: 0.75rem;
            color: var(--primary-color);
            font-weight: bold;
            margin-bottom: 5px;
            text-transform: uppercase;
        }

        .card-info h3 {
            font-size: 1.1rem;
            margin: 0;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 40px 20px;
            border-top: 1px solid #222;
            margin-top: 60px;
            color: #666;
            font-size: 0.9rem;
        }

        /* Responsif untuk HP */
        @media (max-width: 600px) {
            header h1 { font-size: 1.8rem; }
            .container { 
                grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); 
                gap: 15px;
            }
            .card img { height: 230px; }
        }
    </style>
</head>
<body>

    <header>
        <h1>Anime Library</h1>
        <p>Katalog Koleksi Media Favorit</p>
    </header>

    <main class="container">
        <div class="card">
            <img src="https://via.placeholder.com/300x450/1a1a1a/ffffff?text=Anime+Poster+1" alt="Poster">
            <div class="card-info">
                <span>Action / Supernatural</span>
                <h3>Judul Anime Satu</h3>
            </div>
        </div>

        <div class="card">
            <img src="https://via.placeholder.com/300x450/1a1a1a/ffffff?text=Anime+Poster+2" alt="Poster">
            <div class="card-info">
                <span>Adventure / Shounen</span>
                <h3>Judul Anime Dua</h3>
            </div>
        </div>

        <div class="card">
            <img src="https://via.placeholder.com/300x450/1a1a1a/ffffff?text=Anime+Poster+3" alt="Poster">
            <div class="card-info">
                <span>Romance / Slice of Life</span>
                <h3>Judul Anime Tiga</h3>
            </div>
        </div>

        <div class="card">
            <img src="https://via.placeholder.com/300x450/1a1a1a/ffffff?text=Anime+Poster+4" alt="Poster">
            <div class="card-info">
                <span>Sci-Fi / Mecha</span>
                <h3>Judul Anime Empat</h3>
            </div>
        </div>

        <div class="card">
            <img src="https://via.placeholder.com/300x450/1a1a1a/ffffff?text=Anime+Poster+5" alt="Poster">
            <div class="card-info">
                <span>Horror / Mystery</span>
                <h3>Judul Anime Lima</h3>
            </div>
        </div>
    </main>

    <footer>
        <p>&copy; 2026 Anime Vault Project | Dibuat dengan GitHub Pages</p>
    </footer>

</body>
</html>
