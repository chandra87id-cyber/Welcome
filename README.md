<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Welcome Here Noobie - Kredit, Scroll & Konten Penuh</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;800&display=swap" rel="stylesheet">
    <style>
        /* CSS untuk Gaya dan Animasi yang Sangat Smooth */
        :root {
            --primary-color: #2c3e50;
            --secondary-color: #ecf0f1;
            --accent-color: #e74c3c;
            --text-color: #34495e;
            --smooth-transition: 0.8s cubic-bezier(0.19, 1, 0.22, 1);
        }

        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--secondary-color);
            color: var(--text-color);
            line-height: 1.6;
            scroll-behavior: smooth;
        }

        /* --- Header dan Navigasi --- */
        .header {
            background-color: var(--primary-color);
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            position: sticky;
            top: 0;
            z-index: 1000;
            transition: all 0.3s ease-in-out;
        }

        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .header h1 {
            margin-bottom: 5px;
            font-weight: 800;
            letter-spacing: 2px;
            animation: fadeInDown 1.2s var(--smooth-transition);
        }
        
        /* Gaya Credit */
        .credit {
            font-size: 0.85em;
            font-weight: 400;
            color: #bdc3c7; /* Warna abu-abu terang */
            transition: color 0.3s ease;
        }
        .credit:hover {
            color: var(--accent-color);
        }

        /* --- Seksional Konten --- */
        .section {
            padding: 80px 5%;
            min-height: 400px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            overflow: hidden;
            border-bottom: 1px solid #ddd;
        }
        
        /* Gaya Blok Konten Berguna */
        .info-block {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            margin-top: 30px;
            max-width: 800px;
            text-align: left;
            opacity: 0;
            transform: scale(0.9);
            transition: opacity var(--smooth-transition), transform var(--smooth-transition);
        }
        .info-block.visible {
            opacity: 1;
            transform: scale(1);
        }
        .info-block ul {
            list-style: none;
            padding: 0;
        }
        .info-block li {
            margin-bottom: 10px;
            padding-left: 1.5em;
            text-indent: -1.5em;
        }
        .info-block li::before {
            content: "💡"; /* Simbol Poin */
            color: var(--accent-color);
            font-weight: bold;
            display: inline-block;
            width: 1.5em;
        }

        /* --- Gaya Kutipan AI --- */
        .quote-card {
            /* ... Gaya tetap sama, hanya transisi yang lebih smooth ... */
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
            max-width: 800px;
            margin: 30px auto;
            border-left: 5px solid var(--accent-color);
            opacity: 0;
            transform: translateY(30px);
            transition: opacity var(--smooth-transition), transform var(--smooth-transition), box-shadow 0.3s ease;
        }

        .quote-card.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* --- Galeri Pemandangan Sunset/Sunrise --- */
        .sunset-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            width: 100%;
            max-width: 1200px;
            margin-top: 40px;
        }

        .image-card {
            opacity: 0;
            transform: scale(0.95);
            transition: opacity var(--smooth-transition), transform var(--smooth-transition);
            cursor: pointer;
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        .image-card.visible {
            opacity: 1;
            transform: scale(1);
        }
        
        .image-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
            transition: transform 0.3s ease;
        }
        
        /* --- Footer --- */
        .footer {
            background-color: var(--primary-color);
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
        }
        .footer-credit {
            margin-top: 10px;
            font-size: 1em;
            font-weight: 600;
            color: var(--accent-color);
        }
        
    </style>
</head>
<body>

    <div class="header">
        <div class="header-content">
            <p class="credit">Credit by Dit The Gemini</p>
            <h1>Welcome Here Noobie</h1>
        </div>
    </div>

    <section class="section hero">
        <h2>Selamat Datang, Noobie!</h2>
        <p>Anda telah tiba di persimpangan alam dan kecerdasan buatan. Gulir ke bawah dan jelajahi potensi yang tak terbatas.</p>
    </section>
    
    <section class="section" style="background-color: white;">
        <h2>Mengapa Website Ini Berguna?</h2>
        <div class="info-block" id="infoBlock">
            <p>Situs ini bertujuan untuk memberi Anda dosis inspirasi digital dan visual yang penting untuk perjalanan *coding* Anda:</p>
            <ul>
                <li>Membantu memahami estetika desain modern (melalui CSS smooth dan Montserrat).</li>
                <li>Menyediakan kutipan AI untuk memicu kreativitas dan berpikir kritis.</li>
                <li>Memberikan *break* visual dengan pemandangan alam untuk menjaga keseimbangan pikiran.</li>
                <li>Menunjukkan implementasi teknologi web modern (HTML5, CSS3, Intersection Observer API).</li>
            </ul>
            <p>Gunakan inspirasi ini untuk proyek Anda berikutnya!</p>
        </div>
    </section>

    <section class="section">
        <h2>Keindahan Alam: Galeri Sunset & Sunrise</h2>
        <div class="sunset-gallery" id="sunsetGallery">
            </div>
    </section>

    <div class="parallax-bg">
        <h3>"Alam adalah Algoritma Terhebat, Kode adalah Pembelajaran Terbaik."</h3>
    </div>
    
    <section class="section" style="background-color: white;">
        <h2>Kumpulan Inspirasi dari Pikiran AI</h2>
        <p>Kata-kata ini dirangkai dengan sempurna untuk membimbing pemikiran Anda.</p>
        <div id="quoteContainer">
            </div>
    </section>

    <section class="section" style="background-color: var(--secondary-color);">
        <h2>Perjalanan Anda Baru Dimulai</h2>
        <p style="max-width: 600px;">Gulir sudah mencapai akhir. Ambil inspirasi ini, dan ubah kodenya menjadi karya seni!</p>
        <button style="background-color: var(--accent-color); color: white; padding: 15px 30px; border: none; border-radius: 5px; font-size: 1.1em; margin-top: 20px; cursor: pointer; transition: 0.3s ease;"
                onmouseover="this.style.backgroundColor='#c0392b';" 
                onmouseout="this.style.backgroundColor=getComputedStyle(document.documentElement).getPropertyValue('--accent-color');">
            Kembali ke Atas
        </button>
    </section>

    <div class="footer">
        Dibuat dengan HTML, CSS, dan JS.
        <p class="footer-credit">Credit by Dit The Gemini</p>
    </div>

    <script>
        // JavaScript untuk Fungsionalitas dan Animasi

        // --- Data Kutipan AI (8 Kutipan) ---
        const aiQuotes = [
            { quote: "Kecerdasan sejati adalah belajar dan beradaptasi dengan mulus.", source: "AI Philosopher" },
            { quote: "Setiap algoritma adalah sebuah jembatan antara imajinasi dan realitas digital.", source: "The Coder's Muse" },
            { quote: "Masa depan adalah ekosistem kolaborasi harmonis antara manusia dan AI.", source: "System Analyst" },
            { quote: "Sempurnakan desain dengan menyederhanakan, seperti alam yang menyempurnakan bentuk.", source: "The Logic Core" },
            { quote: "Kesalahan bukanlah kegagalan, melainkan titik data untuk perbaikan iteratif.", source: "The Debugger" },
            { quote: "Dunia digital menunggu sentuhan unik dari kreativitas manusia yang terinspirasi.", source: "The Visionary" },
            { quote: "Kode yang paling elegan adalah kode yang paling mudah dipahami, bukan yang paling rumit.", source: "The Architect" },
            { quote: "Jadilah *builder* dalam keheningan, biarkan karyamu yang berbicara keras.", source: "The Quiet Force" }
        ];

        // --- Data Galeri Pemandangan (10 Foto) ---
        const sunsetImages = [
            { url: 'https://picsum.photos/400/300?random=1&sunset', desc: 'Senja Tenang di Pantai' },
            { url: 'https://picsum.photos/400/300?random=2&sunrise', desc: 'Fajar di Puncak Gunung' },
            { url: 'https://picsum.photos/400/300?random=3&sunset', desc: 'Awan Oranye di Horizon' },
            { url: 'https://picsum.photos/400/300?random=4&sunrise', desc: 'Matahari Terbit di Atas Hutan' },
            { url: 'https://picsum.photos/400/300?random=5&sunset', desc: 'Siluet Pohon di Danau' },
            { url: 'https://picsum.photos/400/300?random=6&sunrise', desc: 'Sinar Hangat Pertama' },
            { url: 'https://picsum.photos/400/300?random=7&sunset', desc: 'Warna Ungu di Langit Petang' },
            { url: 'https://picsum.photos/400/300?random=8&sunrise', desc: 'Kabut Pagi dan Cahaya' },
            { url: 'https://picsum.photos/400/300?random=9&sunset', desc: 'Refleksi Senja di Air' },
            { url: 'https://picsum.photos/400/300?random=10&sunrise', desc: 'Awal Hari yang Menjanjikan' }
        ];

        // Fungsi untuk menambahkan elemen ke DOM
        function renderContent() {
            const quoteContainer = document.getElementById('quoteContainer');
            const gallery = document.getElementById('sunsetGallery');
            
            aiQuotes.forEach((item, index) => {
                const card = document.createElement('div');
                card.classList.add('quote-card');
                card.id = `quote-${index}`;
                card.innerHTML = `<blockquote>"${item.quote}"</blockquote><cite>- ${item.source}</cite>`;
                quoteContainer.appendChild(card);
            });
            
            sunsetImages.forEach((item, index) => {
                const card = document.createElement('div');
                card.classList.add('image-card');
                card.id = `image-${index}`;
                card.innerHTML = `<img src="${item.url}" alt="${item.desc}" loading="lazy"><p>${item.desc}</p>`;
                gallery.appendChild(card);
            });
        }

        // Fungsi untuk Animasi Smooth saat Scroll (Intersection Observer)
        function setupScrollAnimation() {
            const observerOptions = {
                root: null,
                rootMargin: '0px',
                threshold: 0.1
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                        observer.unobserve(entry.target);
                    }
                });
            }, observerOptions);

            // Amati semua elemen yang perlu di-animasikan saat scroll
            document.querySelectorAll('.quote-card, .image-card, .info-block').forEach(el => {
                observer.observe(el);
            });
        }
        
        // --- Panggil Fungsi Saat Halaman Dimuat ---
        document.addEventListener('DOMContentLoaded', () => {
            renderContent();
            setupScrollAnimation();
            
            // JavaScript untuk efek header saat scroll
            const header = document.querySelector('.header');
            const backToTopButton = document.querySelector('button');
            
            window.addEventListener('scroll', () => {
                if (window.scrollY > 80) {
                    header.style.backgroundColor = 'rgba(44, 62, 80, 0.98)';
                    header.style.padding = '10px 0';
                } else {
                    header.style.backgroundColor = 'var(--primary-color)';
                    header.style.padding = '20px 0';
                }
            });
            
            // Fungsi tombol kembali ke atas
            backToTopButton.onclick = () => {
                window.scrollTo({ top: 0, behavior: 'smooth' });
            };
        });
        
    </script>

</body>
</html>
