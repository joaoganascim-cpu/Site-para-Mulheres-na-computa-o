<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mulheres na Computação | Transformando o Futuro da Tecnologia</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;600;800&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #7c3aed;
            --primary-hover: #6d28d9;
            --secondary: #ec4899;
            --accent: #f43f5e;
            --dark-bg: #0f172a;
            --card-bg: #1e293b;
            --text-light: #f8fafc;
            --text-muted: #94a3b8;
            --gradient: linear-gradient(135deg, #7c3aed 0%, #ec4899 100%);
            --glass-bg: rgba(30, 41, 59, 0.7);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Plus Jakarta Sans', sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--dark-bg);
            color: var(--text-light);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Navbar */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(15, 23, 42, 0.85);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            z-index: 1000;
        }

        nav {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1.2rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.4rem;
            font-weight: 800;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .nav-links {
            display: flex;
            gap: 2rem;
            list-style: none;
        }

        .nav-links a {
            color: var(--text-muted);
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s ease;
        }

        .nav-links a:hover {
            color: var(--text-light);
        }

        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 8rem 2rem 4rem;
            background: radial-gradient(circle at 50% 20%, rgba(124, 58, 237, 0.15) 0%, transparent 50%);
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
        }

        .badge {
            display: inline-block;
            padding: 0.5rem 1.2rem;
            background: rgba(124, 58, 237, 0.2);
            border: 1px solid var(--primary);
            border-radius: 50px;
            color: #c084fc;
            font-weight: 600;
            font-size: 0.9rem;
            margin-bottom: 1.5rem;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 800;
            line-height: 1.15;
            margin-bottom: 1.5rem;
        }

        .hero h1 span {
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.2rem;
            color: var(--text-muted);
            margin-bottom: 2.5rem;
        }

        .btn-primary {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 0.9rem 2.2rem;
            background: var(--gradient);
            color: white;
            text-decoration: none;
            font-weight: 600;
            border-radius: 50px;
            box-shadow: 0 10px 25px -5px rgba(236, 72, 153, 0.4);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px -5px rgba(236, 72, 153, 0.6);
        }

        /* Stats Section */
        .stats {
            max-width: 1200px;
            margin: -3rem auto 6rem;
            padding: 0 2rem;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .stat-card {
            background: var(--glass-bg);
            border: 1px solid rgba(255, 255, 255, 0.08);
            backdrop-filter: blur(10px);
            padding: 2rem;
            border-radius: 20px;
            text-align: center;
        }

        .stat-card h3 {
            font-size: 2.5rem;
            font-weight: 800;
            color: var(--secondary);
            margin-bottom: 0.5rem;
        }

        .stat-card p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        /* Sections Common */
        .section-padding {
            padding: 6rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-title h2 {
            font-size: 2.5rem;
            font-weight: 800;
            margin-bottom: 1rem;
        }

        .section-title p {
            color: var(--text-muted);
            font-size: 1.1rem;
        }

        /* Pioneers Grid */
        .pioneers-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .pioneer-card {
            background: var(--card-bg);
            border-radius: 24px;
            padding: 2rem;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: transform 0.3s ease, border-color 0.3s ease;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .pioneer-card:hover {
            transform: translateY(-8px);
            border-color: var(--primary);
        }

        .pioneer-icon {
            width: 60px;
            height: 60px;
            background: rgba(124, 58, 237, 0.15);
            color: var(--secondary);
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
        }

        .pioneer-card h3 {
            font-size: 1.4rem;
            margin-bottom: 0.5rem;
        }

        .pioneer-card .role {
            color: var(--primary);
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        .pioneer-card p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        /* Timeline Section */
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            width: 2px;
            height: 100%;
            background: rgba(255, 255, 255, 0.1);
            transform: translateX(-50%);
        }

        .timeline-item {
            margin-bottom: 3rem;
            position: relative;
            width: 50%;
            padding-right: 3rem;
        }

        .timeline-item:nth-child(even) {
            margin-left: 50%;
            padding-right: 0;
            padding-left: 3rem;
        }

        .timeline-content {
            background: var(--card-bg);
            padding: 1.8rem;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        .timeline-date {
            color: var(--secondary);
            font-weight: 800;
            margin-bottom: 0.5rem;
        }

        /* Footer */
        footer {
            background: #090d16;
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            padding: 4rem 2rem 2rem;
            text-align: center;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 2rem;
        }

        .social-links {
            display: flex;
            gap: 1.5rem;
        }

        .social-links a {
            color: var(--text-muted);
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }

        .social-links a:hover {
            color: var(--primary);
        }

        .copyright {
            color: var(--text-muted);
            font-size: 0.9rem;
            border-top: 1px solid rgba(255, 255, 255, 0.05);
            padding-top: 2rem;
            width: 100%;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.4rem;
            }

            .nav-links {
                display: none;
            }

            .timeline::before {
                left: 20px;
            }

            .timeline-item, .timeline-item:nth-child(even) {
                width: 100%;
                padding-left: 3rem;
                padding-right: 0;
                margin-left: 0;
            }
        }
    </style>
</head>
<body>

    <!-- Header / Navbar -->
    <header>
        <nav>
            <div class="logo">
                <i class="fa-solid fa-code-branch"></i> WomenInTech
            </div>
            <ul class="nav-links">
                <li><a href="#inicio">Início</a></li>
                <li><a href="#pioneiras">Pioneiras</a></li>
                <li><a href="#historia">História</a></li>
                <li><a href="#iniciativas">Iniciativas</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="hero">
        <div class="hero-content">
            <span class="badge"><i class="fa-solid fa-sparkles"></i> Empoderando Gerações</span>
            <h1>Mulheres que Moldaram e Reorganizam a <span>Computação</span></h1>
            <p>Conheça as histórias, o impacto e a relevância fundamental das mulheres na criação da tecnologia moderna e no desenvolvimento do futuro digital.</p>
            <a href="#pioneiras" class="btn-primary">
                Explorar Pioneiras <i class="fa-solid fa-arrow-right"></i>
            </a>
        </div>
    </section>

    <!-- Stat Cards -->
    <section class="stats">
        <div class="stat-card">
            <h3>1ª</h3>
            <p>Programadora da história foi uma mulher (Ada Lovelace)</p>
        </div>
        <div class="stat-card">
            <h3>1946</h3>
            <p>Ano do ENIAC, programado por 6 mulheres visionárias</p>
        </div>
        <div class="stat-card">
            <h3>100%</h3>
            <p>Inspirador para as futuras gerações de devas e engenheiras</p>
        </div>
    </section>

    <!-- Pioneiras Grid -->
    <section id="pioneiras" class="section-padding">
        <div class="section-title">
            <h2>Grandes Pioneiras</h2>
            <p>As mentes brilhantes que abriram o caminho da programação e inovação.</p>
        </div>

        <div class="pioneers-grid">
            <div class="pioneer-card">
                <div>
                    <div class="pioneer-icon"><i class="fa-solid fa-scroll"></i></div>
                    <h3>Ada Lovelace</h3>
                    <p class="role">A Primeira Programadora</p>
                    <p>Escreveu o primeiro algoritmo da história para ser processado por uma máquina, a Máquina Analítica de Babbage, em 1843.</p>
                </div>
            </div>

            <div class="pioneer-card">
                <div>
                    <div class="pioneer-icon"><i class="fa-solid fa-terminal"></i></div>
                    <h3>Grace Hopper</h3>
                    <p class="role">Mãe do Compilador e COBOL</p>
                    <p>Criou o primeiro compilador para linguagens de programação e popularizou o termo "bug" após encontrar uma mariposa no computador.</p>
                </div>
            </div>

            <div class="pioneer-card">
                <div>
                    <div class="pioneer-icon"><i class="fa-solid fa-rocket"></i></div>
                    <h3>Margaret Hamilton</h3>
                    <p class="role">Diretora da Apollo / NASA</p>
                    <p>Liderou o time de desenvolvimento do software de navegação da missão Apollo 11, garantindo o pouso seguro do homem na Lua.</p>
                </div>
            </div>

            <div class="pioneer-card">
                <div>
                    <div class="pioneer-icon"><i class="fa-solid fa-calculator"></i></div>
                    <h3>Katherine Johnson</h3>
                    <p class="role">Matemática da NASA</p>
