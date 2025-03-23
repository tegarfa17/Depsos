<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Departemen Sosial - Himpunan Mahasiswa Administrasi Niaga</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <style>
        :root {
            --primary: #ff7700;
            --primary-dark: #e56b00;
            --secondary: #000000;
            --light: #f8f9fa;
            --dark: #212529;
            --accent: #2c80ff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: var(--dark);
            overflow-x: hidden;
        }
        
        header {
            background-color: var(--primary);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo img {
            height: 50px;
            margin-right: 10px;
        }
        
        .logo h1 {
            font-size: 1.2rem;
            font-weight: 600;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            padding: 0.5rem 1rem;
            border-radius: 4px;
            transition: all 0.3s ease;
        }
        
        nav ul li a:hover, nav ul li a.active {
            background-color: rgba(255,255,255,0.2);
        }
        
        .hamburger {
            display: none;
            cursor: pointer;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
        }
        
        main {
            margin-top: 80px;
            min-height: calc(100vh - 180px);
        }
        
        .hero {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('/api/placeholder/1200/600') center/cover no-repeat;
            color: white;
            padding: 100px 0;
            text-align: center;
        }
        
        .hero h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            line-height: 1.6;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--primary);
            color: white;
            padding: 0.8rem 1.5rem;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .btn-outline {
            background-color: transparent;
            border: 2px solid var(--primary);
            margin-left: 1rem;
        }
        
        .btn-outline:hover {
            background-color: var(--primary);
        }
        
        .section {
            padding: 80px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 2rem;
            display: inline-block;
            position: relative;
            padding-bottom: 10px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background-color: var(--primary);
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 40px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .about-text p {
            margin-bottom: 1rem;
            line-height: 1.6;
        }
        
        .about-image {
            flex: 1;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .mission-values {
            background-color: white;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-radius: 8px;
            padding: 30px;
            margin-top: 40px;
        }
        
        .mission-values h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            text-align: center;
            color: var(--primary);
        }
        
        .mission-values-content {
            display: flex;
            gap: 30px;
        }
        
        .mission-box, .values-box {
            flex: 1;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 8px;
        }
        
        .mission-box h4, .values-box h4 {
            margin-bottom: 1rem;
            color: var(--secondary);
        }
        
        .team {
            background-color: var(--light);
        }
        
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
        }
        
        .team-member {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
        }
        
        .team-member:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }
        
        .team-member img {
            width: 100%;
            height: 250px;
            object-fit: cover;
        }
        
        .team-info {
            padding: 20px;
            text-align: center;
        }
        
        .team-info h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }
        
        .team-info p {
            color: var(--primary);
            font-weight: 500;
            margin-bottom: 0.5rem;
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin-top: 15px;
        }
        
        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 35px;
            height: 35px;
            background-color: #f5f5f5;
            color: var(--dark);
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .social-icons a:hover {
            background-color: var(--primary);
            color: white;
        }
        
        .gallery {
            background-color: white;
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 8px;
            cursor: pointer;
        }
        
        .gallery-item img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: all 0.5s ease;
        }
        
        .gallery-item:hover img {
            transform: scale(1.1);
        }
        
        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background-color: rgba(0, 0, 0, 0.7);
            color: white;
            padding: 15px;
            transform: translateY(100%);
            transition: all 0.3s ease;
        }
        
        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }
        
        .gallery-overlay h3 {
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
        }
        
        .gallery-modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.9);
            z-index: 2000;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .modal-content {
            position: relative;
            max-width: 800px;
            width: 100%;
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
        }
        
        .modal-content img {
            width: 100%;
            height: auto;
        }
        
        .modal-info {
            padding: 20px;
        }
        
        .modal-info h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
            color: var(--primary);
        }
        
        .modal-info p {
            line-height: 1.6;
        }
        
        .close-modal {
            position: absolute;
            top: 15px;
            right: 15px;
            width: 35px;
            height: 35px;
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            font-size: 1.2rem;
        }
        
        .donation {
            background-color: var(--light);
        }
        
        .donation-content {
            display: flex;
            gap: 40px;
        }
        
        .donation-info {
            flex: 1;
        }
        
        .donation-info h3 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .donation-info p {
            margin-bottom: 1rem;
            line-height: 1.6;
        }
        
        .donation-methods {
            margin-top: 20px;
        }
        
        .donation-method {
            background-color: white;
            padding: 15px;
            border-radius: 8px;
            margin-bottom: 15px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.05);
        }
        
        .donation-method h4 {
            display: flex;
            align-items: center;
            gap: 10px;
            font-size: 1.2rem;
            margin-bottom: 0.5rem;
            color: var(--secondary);
        }
        
        .donation-method h4 i {
            color: var(--primary);
        }
        
        .donation-method p {
            margin-bottom: 0.5rem;
        }
        
        .donation-form {
            flex: 1;
            background-color: white;
            border-radius: 8px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
        }
        
        .form-control:focus {
            border-color: var(--primary);
            outline: none;
        }
        
        .testimonials {
            margin-top: 40px;
        }
        
        .testimonials h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
            text-align: center;
            color: var(--primary);
        }
        
        .testimonial-slider {
            display: flex;
            overflow-x: auto;
            scroll-snap-type: x mandatory;
            gap: 20px;
            padding: 20px 0;
            scrollbar-width: none;
        }
        
        .testimonial-slider::-webkit-scrollbar {
            display: none;
        }
        
        .testimonial {
            scroll-snap-align: start;
            min-width: 300px;
            background-color: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .testimonial-content {
            font-style: italic;
            margin-bottom: 15px;
            line-height: 1.6;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .testimonial-author img {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            object-fit: cover;
        }
        
        .author-info h4 {
            font-size: 1rem;
            margin-bottom: 0.2rem;
        }
        
        .author-info p {
            font-size: 0.9rem;
            color: #666;
        }
        
        .contact {
            background-color: white;
        }
        
        .contact-content {
            display: flex;
            gap: 40px;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .contact-info h3 {
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }
        
        .contact-info p {
            margin-bottom: 1rem;
            line-height: 1.6;
        }
        
        .contact-details {
            margin-top: 20px;
        }
        
        .contact-item {
            display: flex;
            align-items: flex-start;
            gap: 15px;
            margin-bottom: 15px;
        }
        
        .contact-item i {
            color: var(--primary);
            font-size: 1.2rem;
            margin-top: 3px;
        }
        
        .contact-text h4 {
            font-size: 1.1rem;
            margin-bottom: 0.3rem;
        }
        
        .contact-form {
            flex: 1;
            background-color: #f9f9f9;
            border-radius: 8px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        footer {
            background-color: var(--secondary);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            gap: 40px;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }
        
        .footer-column {
            flex: 1;
            min-width: 200px;
        }
        
        .footer-column h3 {
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 2px;
            background-color: var(--primary);
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #bbb;
            text-decoration: none;
            transition: all 0.3s ease;
        }
        
        .footer-column ul li a:hover {
            color: var(--primary);
            padding-left: 5px;
        }
        
        .footer-social {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .footer-social a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255,255,255,0.1);
            color: white;
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .footer-social a:hover {
            background-color: var(--primary);
            transform: translateY(-5px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255,255,255,0.1);
            font-size: 0.9rem;
            color: #bbb;
        }
        
        @media screen and (max-width: 992px) {
            .about-content, .donation-content, .contact-content {
                flex-direction: column;
            }
            
            .mission-values-content {
                flex-direction: column;
            }
            
            .team-grid {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            }
        }
        
        @media screen and (max-width: 768px) {
            .hamburger {
                display: block;
            }
            
            nav {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 80%;
                height: calc(100vh - 80px);
                background-color: var(--secondary);
                transition: all 0.4s ease;
            }
            
            nav.active {
                left: 0;
            }
            
            nav ul {
                flex-direction: column;
                padding: 20px;
            }
            
            nav ul li {
                margin: 10px 0;
            }
            
            .gallery-grid {
                grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <img src="https://pbs.twimg.com/profile_images/465820912780984320/kk-CVLkR_400x400.jpeg" alt="Logo HMAN">
                    <h1>Departemen Sosial HMAN</h1>
                </div>
                <button class="hamburger" id="hamburger">
                    <i class="fas fa-bars"></i>
                </button>
                <nav id="nav">
                    <ul>
                        <li><a href="#home" class="active">Beranda</a></li>
                        <li><a href="#about">Tentang Kami</a></li>
                        <li><a href="#team">Kepengurusan</a></li>
                        <li><a href="#gallery">Galeri</a></li>
                        <li><a href="#donation">Donasi</a></li>
                        <li><a href="#contact">Kontak</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <main>
        <section id="home" class="hero">
            <div class="container">
                <h2>Departemen Sosial HMAN</h2>
                <p>Menggerakkan perubahan sosial melalui kepedulian dan aksi nyata. Bersama kita bangun masyarakat yang lebih baik dan peduli terhadap sesama.</p>
                <a href="#donation" class="btn">Donasi Sekarang</a>
                <a href="#about" class="btn btn-outline">Pelajari Lebih Lanjut</a>
            </div>
        </section>

        <section id="about" class="section">
            <div class="container">
                <div class="section-title">
                    <h2>Tentang Kami</h2>
                </div>
                <div class="about-content">
                    <div class="about-text">
                        <h3>Departemen Sosial HMAN</h3>
                        <p>Departemen Sosial Himpunan Mahasiswa Administrasi Niaga (HMAN) merupakan badan yang bergerak dalam bidang sosial dan kemanusiaan di lingkungan kampus dan masyarakat. Kami berkomitmen untuk menjadi penggerak perubahan positif melalui berbagai program sosial yang berdampak langsung kepada masyarakat.</p>
                        <p>Kami percaya bahwa kepedulian sosial adalah kunci untuk membangun masyarakat yang lebih baik. Melalui berbagai program dan kegiatan, kami berusaha menyebarkan nilai-nilai kemanusiaan, kepedulian, dan kebermanfaatan kepada sesama.</p>
                    </div>
                    <div class="about-image">
                        <img src="/api/placeholder/600/400" alt="Kegiatan Sosial HMAN">
                    </div>
                </div>

                <div class="mission-values">
                    <h3>Visi, Misi & Tujuan</h3>
                    <div class="mission-values-content">
                        <div class="mission-box">
                            <h4>Visi</h4>
                            <p>Menjadi departemen yang mampu menggerakkan nilai-nilai sosial dan kemanusiaan di lingkungan kampus serta menjadi pusat inisiasi program sosial yang berdampak luas pada masyarakat.</p>
                            
                            <h4>Misi</h4>
                            <ul>
                                <li>Menyelenggarakan program sosial yang bermanfaat bagi masyarakat</li>
                                <li>Membangun kepekaan sosial mahasiswa terhadap isu-isu sosial</li>
                                <li>Menjalin kerjasama dengan berbagai pihak untuk memperluas dampak program sosial</li>
                                <li>Menggalang partisipasi aktif mahasiswa dalam kegiatan sosial</li>
                            </ul>
                        </div>
                        <div class="values-box">
                            <h4>Tujuan</h4>
                            <p>Departemen Sosial HMAN hadir dengan tujuan untuk:</p>
                            <ul>
                                <li>Meningkatkan kepedulian sosial mahasiswa terhadap lingkungan sekitar</li>
                                <li>Memberikan bantuan nyata kepada masyarakat yang membutuhkan</li>
                                <li>Membangun jejaring sosial yang kuat dengan berbagai komunitas dan lembaga sosial</li>
                                <li>Menanamkan nilai-nilai kemanusiaan dalam setiap kegiatan kemahasiswaan</li>
                                <li>Menjadi wadah bagi mahasiswa untuk mengembangkan kepekaan sosial dan jiwa kerelawanan</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="team" class="section team">
            <div class="container">
                <div class="section-title">
                    <h2>Struktur Kepengurusan</h2>
                </div>
                <div class="team-grid">
                    <div class="team-member">
                        <img src="/api/placeholder/300/300" alt="Ketua Departemen">
                        <div class="team-info">
                            <h3>Haifa Nurul Aini W</h3>
                            <p>Ketua Departemen</p>
                            <div class="social-icons">
                                <a href="#"><i class="fab fa-instagram"></i></a>
                                <a href="#"><i class="fab fa-linkedin"></i></a>
                                <a href="#"><i class="fab fa-twitter"></i></a>
                            </div>
                        </div>
                    </div>
                    <div class="team-member">
                        <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiDz879RUX8FgNvdJRFBY3AcqE4AT_EGd5W9MIjDNNwHFd7PQHfOUg__1jxzww-yPNMTbPvOJbvA6pOzFuTuj1HnCp7MtU0EWMqxwmgACBx4oaSvuhwSV2_kb5t14t99g3tZYX3Gx5q6sBF5cw1uJ2mI29UIKmfBZWUdqPu4ypdq4FVvopLso4YsZxvjWk/s320/WhatsApp%20Image%202025-03-22%20at%2011.03.43_191ba4a7.jpg" alt="Wakil Ketua Departemen">
                        <div class="team-info">
                            <h3>Raihan</h3>
                            <p>Wakil Ketua Departemen</p>
                            <div class="social-icons">
                                <a href="#"><i class="fab fa-instagram"></i></a>
                                <a href="#"><i class="fab fa-linkedin"></i></a>
                                <a href="#"><i class="fab fa-twitter"></i></a>
                            </div>
                        </div>
                    </div>
                    <div class="team-member">
                        <img src="/api/placeholder/300/300" alt="Ketua Divisi Rohani">
                        <div class="team-info">
                            <h3>Iqbal</h3>
                            <p>Ketua Divisi Rohani</p>
                            <div class="social-icons">
                                <a href="#"><i class="fab fa-instagram"></i></a>
                                <a href="#"><i class="fab fa-linkedin"></i></a>
                                <a href="#"><i class="fab fa-twitter"></i></a>
                            </div>
                        </div>
                    </div>
                    <div class="team-member">
                        <img src="/api/placeholder/300/300" alt="Ketua Divisi Pendidikan">
                        <div class="team-info">
                            <h3>Devita</h3>
                            <p>Ketua Divisi Pendidikan</p>
                            <div class="social-icons">
                                <a href="#"><i class="fab fa-instagram"></i></a>
                                <a href="#"><i class="fab fa-linkedin"></i></a>
                                <a href="#"><i class="fab fa-twitter"></i></a>
                            </div>
                        </div>
                    </div>
                    <div class="team-member">
                        <img src="/api/placeholder/300/300" alt="Ketua Divisi Lingkungan">
                        <div class="team-info">
                            <h3>Alya</h3>
                            <p>Ketua Divisi Lingkungan</p>
                            <div class="social-icons">
                                <a href="#"><i class="fab fa-instagram"></i></a>
                                <a href="#"><i class="fab fa-linkedin"></i></a>
                                <a href="#"><i class="fab fa-twitter"></i></a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="gallery" class="section gallery">
            <div class="container">
                <div class="section-title">
                    <h2>Galeri Kegiatan</h2>
                </div>
                <div class="gallery-grid">
                    <div class="gallery-item" data-id="1">
                        <img src="/api/placeholder/400/300" alt="Bakti Sosial">
                        <div class="gallery-overlay">
                            <h3>Bakti Sosial</h3>
                            <p>Klik untuk melihat detail</p>
                        </div>
                    </div>
                    <div
