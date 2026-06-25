<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Veleta Adventure - Actividades de turismo activo profesionales. Senderismo, bicicleta, gymkanas y multiaventura en la naturaleza. ¡Descubre tus próximas aventuras!">
    <meta name="keywords" content="turismo activo, senderismo, bicicleta, aventura, naturaleza, outdoor">
    <meta name="author" content="Veleta Adventure">
    <meta property="og:title" content="Veleta Adventure - Descubre Nuestras Actividades">
    <meta property="og:description" content="Actividades variadas de turismo activo, pensadas para todos los públicos">
    <meta property="og:image" content="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=1200&h=630&fit=crop">
    <meta property="og:url" content="https://veleta-adventure.com">
    <meta property="og:type" content="website">
    <meta name="twitter:card" content="summary_large_image">
    <meta name="theme-color" content="#557117">
    <title>Veleta Adventure - Turismo Activo Premium</title>
    
    <style>
        /* ============================================
           RESET Y VARIABLES CSS
           ============================================ */
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            /* Colores Corporativos */
            --color-primary: #557117;
            --color-primary-light: #85ab2b;
            --color-accent: #ff8c00;
            --color-dark: #0f3d57;
            --color-white: #ffffff;
            --color-light-gray: #f5f5f5;
            --color-dark-gray: #2a2a2a;
            --color-text: #333333;
            
            /* Gradientes */
            --gradient-primary: linear-gradient(135deg, #557117 0%, #85ab2b 100%);
            --gradient-dark: linear-gradient(135deg, #0f3d57 0%, #1a5a7a 100%);
            --gradient-accent: linear-gradient(135deg, #ff8c00 0%, #ff7e00 100%);
            
            /* Sombras */
            --shadow-sm: 0 2px 8px rgba(0, 0, 0, 0.1);
            --shadow-md: 0 8px 24px rgba(0, 0, 0, 0.15);
            --shadow-lg: 0 20px 40px rgba(0, 0, 0, 0.2);
            --shadow-xl: 0 30px 60px rgba(0, 0, 0, 0.3);
            
            /* Tipografía */
            --font-display: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            --font-body: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            
            /* Espaciado */
            --spacing-xs: 0.5rem;
            --spacing-sm: 1rem;
            --spacing-md: 2rem;
            --spacing-lg: 3rem;
            --spacing-xl: 4rem;
            --spacing-2xl: 6rem;
            
            /* Transiciones */
            --transition-fast: 0.2s ease-out;
            --transition-normal: 0.3s ease-out;
            --transition-slow: 0.5s ease-out;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-body);
            color: var(--color-text);
            line-height: 1.6;
            overflow-x: hidden;
            background-color: var(--color-white);
        }

        /* ============================================
           TIPOGRAFÍA
           ============================================ */

        h1, h2, h3, h4, h5, h6 {
            font-family: var(--font-display);
            font-weight: 700;
            line-height: 1.2;
            letter-spacing: -0.5px;
        }

        h1 {
            font-size: clamp(2.5rem, 8vw, 4.5rem);
            margin-bottom: var(--spacing-md);
        }

        h2 {
            font-size: clamp(1.8rem, 5vw, 3rem);
            margin-bottom: var(--spacing-lg);
        }

        h3 {
            font-size: clamp(1.3rem, 3vw, 1.8rem);
            margin-bottom: var(--spacing-md);
        }

        p {
            font-size: 1rem;
            margin-bottom: var(--spacing-md);
            color: var(--color-text);
        }

        /* ============================================
           ELEMENTOS GLOBALES
           ============================================ */

        a {
            color: var(--color-primary);
            text-decoration: none;
            transition: all var(--transition-normal);
        }

        button, .btn {
            font-family: var(--font-body);
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-weight: 600;
            transition: all var(--transition-normal);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            font-size: 0.95rem;
            padding: 0.95rem 2rem;
            display: inline-block;
        }

        .btn-primary {
            background: var(--gradient-primary);
            color: var(--color-white);
            box-shadow: var(--shadow-md);
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
            background: linear-gradient(135deg, #6a8a20 0%, #9bc34a 100%);
        }

        .btn-secondary {
            background: transparent;
            color: var(--color-accent);
            border: 2px solid var(--color-accent);
        }

        .btn-secondary:hover {
            background: var(--color-accent);
            color: var(--color-white);
            transform: translateY(-2px);
            box-shadow: var(--shadow-md);
        }

        .btn-white {
            background: var(--color-white);
            color: var(--color-primary);
            border: 2px solid var(--color-white);
        }

        .btn-white:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
            background: transparent;
            color: var(--color-white);
        }

        /* ============================================
           CONTENEDOR Y LAYOUT
           ============================================ */

        .container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 var(--spacing-md);
        }

        .section {
            padding: var(--spacing-2xl) 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: var(--spacing-xl);
        }

        .section-title h2 {
            color: var(--color-dark);
            margin-bottom: var(--spacing-md);
        }

        .section-title p {
            font-size: 1.1rem;
            color: var(--color-text);
            max-width: 600px;
            margin: 0 auto;
        }

        .accent-line {
            width: 80px;
            height: 4px;
            background: var(--gradient-primary);
            margin: 0 auto var(--spacing-lg);
            border-radius: 2px;
        }

        /* ============================================
           HEADER Y NAVEGACIÓN
           ============================================ */

        header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            transition: all var(--transition-normal);
            background: transparent;
            backdrop-filter: blur(0px);
        }

        header.sticky {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: var(--shadow-md);
            padding: 0.75rem 0;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 0;
            position: relative;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            letter-spacing: 1px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            color: var(--color-primary);
            transition: all var(--transition-normal);
        }

        header.sticky .logo {
            color: var(--color-dark);
        }

        .logo span {
            color: var(--color-accent);
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2.5rem;
            align-items: center;
        }

        .nav-menu a {
            color: var(--color-white);
            font-weight: 500;
            position: relative;
            transition: color var(--transition-normal);
        }

        header.sticky .nav-menu a {
            color: var(--color-text);
        }

        .nav-menu a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--color-accent);
            transition: width var(--transition-normal);
        }

        .nav-menu a:hover::after {
            width: 100%;
        }

        .nav-menu .cta-btn {
            background: var(--color-accent);
            color: var(--color-white);
            padding: 0.75rem 1.5rem;
            border-radius: 6px;
            transition: all var(--transition-normal);
            font-size: 0.9rem;
        }

        .nav-menu .cta-btn:hover {
            background: #ff7e00;
            transform: translateY(-2px);
            box-shadow: var(--shadow-md);
        }

        .hamburger {
            display: none;
            flex-direction: column;
            cursor: pointer;
            gap: 5px;
        }

        .hamburger span {
            width: 25px;
            height: 3px;
            background: var(--color-white);
            border-radius: 2px;
            transition: all var(--transition-normal);
        }

        header.sticky .hamburger span {
            background: var(--color-dark);
        }

        .hamburger.active span:nth-child(1) {
            transform: rotate(45deg) translate(10px, 10px);
        }

        .hamburger.active span:nth-child(2) {
            opacity: 0;
        }

        .hamburger.active span:nth-child(3) {
            transform: rotate(-45deg) translate(7px, -7px);
        }

        /* ============================================
           HERO SECTION
           ============================================ */

        .hero {
            height: 100vh;
            min-height: 600px;
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--color-white);
            overflow: hidden;
            margin-top: 0;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, rgba(85, 113, 23, 0.7) 0%, rgba(15, 61, 87, 0.7) 100%),
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><defs><linearGradient id="grad" x1="0%" y1="0%" x2="100%" y2="100%"><stop offset="0%" style="stop-color:%23557117;stop-opacity:0.3"/><stop offset="100%" style="stop-color:%230f3d57;stop-opacity:0.3"/></linearGradient></linearGradient><rect width="1200" height="600" fill="url(%23grad)"/></svg>');
            background-attachment: fixed;
            background-position: center;
            background-size: cover;
            z-index: -2;
        }

        .hero-content {
            z-index: 1;
            max-width: 800px;
            animation: fadeInUp 1s ease-out;
            padding: 0 var(--spacing-md);
        }

        .hero h1 {
            font-size: clamp(2.5rem, 10vw, 5rem);
            margin-bottom: var(--spacing-md);
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 800;
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.3);
            line-height: 1.1;
        }

        .hero-subtitle {
            font-size: clamp(1rem, 3vw, 1.5rem);
            margin-bottom: var(--spacing-xl);
            font-weight: 300;
            letter-spacing: 0.5px;
            text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.3);
        }

        .hero-buttons {
            display: flex;
            gap: var(--spacing-md);
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: var(--spacing-xl);
        }

        .scroll-indicator {
            position: absolute;
            bottom: 30px;
            left: 50%;
            transform: translateX(-50%);
            z-index: 10;
            animation: bounce 2s infinite;
        }

        .scroll-indicator svg {
            width: 30px;
            height: 30px;
            stroke: var(--color-white);
            stroke-width: 2;
        }

        /* ============================================
           SECCIÓN QUIÉNES SOMOS
           ============================================ */

        .about {
            background: linear-gradient(135deg, #ffffff 0%, #f9f9f9 100%);
            position: relative;
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: var(--spacing-xl);
            align-items: center;
        }

        .about-text h2 {
            color: var(--color-dark);
        }

        .about-text p {
            font-size: 1.05rem;
            color: #555;
            margin-bottom: var(--spacing-md);
            line-height: 1.8;
        }

        .about-features {
            display: flex;
            flex-direction: column;
            gap: var(--spacing-md);
            margin-top: var(--spacing-lg);
        }

        .feature-item {
            display: flex;
            gap: var(--spacing-md);
            padding: var(--spacing-md);
            background: rgba(255, 255, 255, 0.5);
            border-left: 4px solid var(--color-primary);
            border-radius: 6px;
            transition: all var(--transition-normal);
            backdrop-filter: blur(10px);
        }

        .feature-item:hover {
            background: rgba(255, 255, 255, 0.8);
            transform: translateX(10px);
            box-shadow: var(--shadow-md);
        }

        .feature-icon {
            font-size: 2rem;
            flex-shrink: 0;
            min-width: 40px;
        }

        .feature-item h4 {
            color: var(--color-primary);
            margin-bottom: var(--spacing-xs);
        }

        .feature-item p {
            margin: 0;
            font-size: 0.95rem;
            color: #666;
        }

        .about-image {
            position: relative;
            height: 500px;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: var(--shadow-xl);
            background: linear-gradient(135deg, var(--color-primary), var(--color-dark));
        }

        .about-image::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 500"><defs><pattern id="mountains" x="0" y="0" width="400" height="500" patternUnits="userSpaceOnUse"><path d="M0,300 Q50,200 100,250 T200,200 T300,250 T400,200 L400,500 L0,500" fill="white" opacity="0.1"/><path d="M0,350 Q75,250 150,300 T300,250 T400,300 L400,500 L0,500" fill="white" opacity="0.08"/></pattern></defs><rect width="400" height="500" fill="url(%23mountains)"/></svg>');
            background-size: 100% 100%;
        }

        /* ============================================
           SECCIÓN ACTIVIDADES
           ============================================ */

        .activities {
            background: var(--color-light-gray);
        }

        .activities-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: var(--spacing-lg);
            margin-bottom: var(--spacing-xl);
        }

        .activity-card {
            background: var(--color-white);
            border-radius: 12px;
            overflow: hidden;
            box-shadow: var(--shadow-md);
            transition: all var(--transition-normal);
            display: flex;
            flex-direction: column;
            height: 100%;
            transform: translateY(0);
        }

        .activity-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-xl);
        }

        .activity-image {
            width: 100%;
            height: 250px;
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
            position: relative;
            overflow: hidden;
        }

        .activity-image::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 300 250"><defs><pattern id="dots" x="0" y="0" width="30" height="30" patternUnits="userSpaceOnUse"><circle cx="15" cy="15" r="2" fill="white" opacity="0.1"/></pattern></defs><rect width="300" height="250" fill="url(%23dots)"/></svg>');
            background-size: 100% 100%;
        }

        .activity-image.special {
            background: linear-gradient(135deg, var(--color-accent), #ff7e00);
        }

        .activity-content {
            padding: var(--spacing-lg);
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .activity-header {
            display: flex;
            align-items: center;
            gap: var(--spacing-md);
            margin-bottom: var(--spacing-md);
        }

        .activity-icon {
            font-size: 2.5rem;
            flex-shrink: 0;
        }

        .activity-content h3 {
            color: var(--color-dark);
            margin-bottom: var(--spacing-sm);
        }

        .activity-description {
            color: #666;
            font-size: 0.95rem;
            line-height: 1.6;
            margin-bottom: auto;
            margin-bottom: var(--spacing-md);
        }

        .activity-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: var(--spacing-md);
            border-top: 1px solid #eee;
        }

        .activity-badge {
            background: var(--color-primary);
            color: var(--color-white);
            padding: 0.35rem 0.75rem;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 600;
            text-transform: uppercase;
        }

        .activity-badge.special {
            background: var(--color-accent);
        }

        .activity-link {
            color: var(--color-accent);
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            transition: all var(--transition-normal);
        }

        .activity-link:hover {
            gap: 1rem;
            color: var(--color-primary);
        }

        /* ============================================
           SECCIÓN VELETA EXPERIENCE
           ============================================ */

        .veleta-experience {
            background: linear-gradient(135deg, var(--color-dark) 0%, #1a5a7a 100%);
            color: var(--color-white);
            position: relative;
            overflow: hidden;
        }

        .veleta-experience::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 1000px;
            height: 1000px;
            background: radial-gradient(circle, rgba(255, 140, 0, 0.1) 0%, transparent 70%);
            border-radius: 50%;
            pointer-events: none;
        }

        .veleta-experience-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: var(--spacing-xl);
            align-items: center;
            position: relative;
            z-index: 1;
        }

        .veleta-text h2 {
            color: var(--color-white);
        }

        .veleta-text p {
            color: rgba(255, 255, 255, 0.9);
            font-size: 1.05rem;
            line-height: 1.8;
        }

        .veleta-highlights {
            display: flex;
            flex-direction: column;
            gap: var(--spacing-md);
            margin-top: var(--spacing-lg);
        }

        .veleta-highlight {
            display: flex;
            align-items: center;
            gap: var(--spacing-md);
            padding: var(--spacing-md);
            background: rgba(255, 255, 255, 0.1);
            border-radius: 8px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all var(--transition-normal);
        }

        .veleta-highlight:hover {
            background: rgba(255, 255, 255, 0.15);
            transform: translateX(8px);
        }

        .veleta-highlight-icon {
            font-size: 2rem;
            flex-shrink: 0;
            min-width: 50px;
        }

        .veleta-highlight h4 {
            color: var(--color-accent);
            margin-bottom: 0.25rem;
        }

        .veleta-highlight p {
            margin: 0;
            font-size: 0.9rem;
        }

        .calendar-preview {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 12px;
            padding: var(--spacing-lg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .calendar-grid {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: var(--spacing-sm);
            margin-bottom: var(--spacing-md);
        }

        .calendar-month {
            background: var(--color-accent);
            color: var(--color-white);
            padding: var(--spacing-md);
            border-radius: 8px;
            text-align: center;
            font-weight: 600;
            cursor: pointer;
            transition: all var(--transition-normal);
            min-height: 80px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }

        .calendar-month:hover {
            transform: scale(1.05);
            box-shadow: var(--shadow-lg);
        }

        /* ============================================
           SECCIÓN POR QUÉ ELEGIRNOS
           ============================================ */

        .why-choose {
            background: var(--color-light-gray);
        }

        .why-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: var(--spacing-lg);
        }

        .why-card {
            background: var(--color-white);
            padding: var(--spacing-lg);
            border-radius: 12px;
            text-align: center;
            box-shadow: var(--shadow-sm);
            transition: all var(--transition-normal);
            border-top: 4px solid var(--color-primary);
        }

        .why-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-lg);
            border-top-color: var(--color-accent);
        }

        .why-card-icon {
            font-size: 3rem;
            margin-bottom: var(--spacing-md);
        }

        .why-card h3 {
            color: var(--color-dark);
            margin-bottom: var(--spacing-md);
        }

        .why-card p {
            color: #666;
            font-size: 0.95rem;
            margin: 0;
        }

        /* ============================================
           SECCIÓN ESTADÍSTICAS
           ============================================ */

        .stats {
            background: linear-gradient(135deg, var(--color-dark) 0%, #1a5a7a 100%);
            color: var(--color-white);
            position: relative;
            overflow: hidden;
        }

        .stats::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="50" cy="50" r="40" fill="none" stroke="white" stroke-width="0.5" opacity="0.1"/><circle cx="50" cy="50" r="30" fill="none" stroke="white" stroke-width="0.5" opacity="0.1"/></svg>');
            background-size: 50px 50px;
            opacity: 0.05;
            pointer-events: none;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: var(--spacing-xl);
            position: relative;
            z-index: 1;
        }

        .stat-card {
            text-align: center;
            padding: var(--spacing-lg);
        }

        .stat-number {
            font-size: clamp(2.5rem, 8vw, 4rem);
            font-weight: 800;
            color: var(--color-accent);
            line-height: 1;
            margin-bottom: var(--spacing-sm);
            font-variant-numeric: tabular-nums;
        }

        .stat-label {
            font-size: 1.1rem;
            color: rgba(255, 255, 255, 0.9);
            font-weight: 500;
        }

        /* ============================================
           SECCIÓN GALERÍA
           ============================================ */

        .gallery {
            background: var(--color-light-gray);
        }

        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: var(--spacing-md);
            margin-bottom: var(--spacing-xl);
        }

        .gallery-item {
            position: relative;
            overflow: hidden;
            border-radius: 12px;
            aspect-ratio: 1;
            cursor: pointer;
            box-shadow: var(--shadow-md);
            transition: all var(--transition-normal);
        }

        .gallery-item:nth-child(n+5):nth-child(-n+8) {
            grid-column: span 1;
        }

        .gallery-item-image {
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, var(--color-primary), var(--color-dark));
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            transition: all var(--transition-normal);
            position: relative;
        }

        .gallery-item:hover .gallery-item-image {
            transform: scale(1.1);
            filter: brightness(1.1);
        }

        .gallery-overlay {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(85, 113, 23, 0.8);
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity var(--transition-normal);
        }

        .gallery-item:hover .gallery-overlay {
            opacity: 1;
        }

        .gallery-icon {
            font-size: 2rem;
            color: var(--color-white);
        }

        /* ============================================
           SECCIÓN TESTIMONIOS
           ============================================ */

        .testimonials {
            background: var(--color-white);
        }

        .testimonial-carousel {
            position: relative;
            max-width: 900px;
            margin: 0 auto;
        }

        .testimonial-card {
            background: linear-gradient(135deg, #f9f9f9 0%, #ffffff 100%);
            padding: var(--spacing-xl);
            border-radius: 12px;
            box-shadow: var(--shadow-md);
            border-left: 4px solid var(--color-primary);
            opacity: 0;
            transition: opacity var(--transition-normal);
            pointer-events: none;
            position: absolute;
            width: 100%;
        }

        .testimonial-card.active {
            opacity: 1;
            pointer-events: auto;
            position: relative;
        }

        .testimonial-header {
            display: flex;
            align-items: center;
            gap: var(--spacing-md);
            margin-bottom: var(--spacing-md);
        }

        .testimonial-avatar {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--color-white);
            font-weight: 700;
            font-size: 1.5rem;
            flex-shrink: 0;
        }

        .testimonial-info h4 {
            color: var(--color-dark);
            margin-bottom: 0.25rem;
        }

        .testimonial-info p {
            margin: 0;
            color: #999;
            font-size: 0.85rem;
        }

        .stars {
            color: var(--color-accent);
            margin-bottom: var(--spacing-md);
            font-size: 1.1rem;
            letter-spacing: 2px;
        }

        .testimonial-text {
            color: #666;
            font-style: italic;
            font-size: 1rem;
            line-height: 1.8;
        }

        .carousel-nav {
            display: flex;
            justify-content: center;
            gap: var(--spacing-md);
            margin-top: var(--spacing-xl);
        }

        .carousel-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: #ddd;
            cursor: pointer;
            transition: all var(--transition-normal);
            border: 2px solid transparent;
        }

        .carousel-dot.active {
            background: var(--color-primary);
            width: 32px;
            border-radius: 6px;
        }

        /* ============================================
           SECCIÓN FAQ
           ============================================ */

        .faq {
            background: var(--color-light-gray);
        }

        .faq-container {
            max-width: 800px;
            margin: 0 auto;
        }

        .faq-item {
            background: var(--color-white);
            margin-bottom: var(--spacing-md);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: var(--shadow-sm);
            transition: all var(--transition-normal);
        }

        .faq-item:hover {
            box-shadow: var(--shadow-md);
        }

        .faq-question {
            padding: var(--spacing-lg);
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: all var(--transition-normal);
            background: linear-gradient(135deg, #ffffff 0%, #f9f9f9 100%);
        }

        .faq-question:hover {
            background: linear-gradient(135deg, #f9f9f9 0%, #ffffff 100%);
        }

        .faq-question h4 {
            color: var(--color-dark);
            margin: 0;
            font-size: 1rem;
        }

        .faq-toggle {
            color: var(--color-primary);
            font-size: 1.5rem;
            transition: transform var(--transition-normal);
            flex-shrink: 0;
            margin-left: var(--spacing-md);
        }

        .faq-item.active .faq-toggle {
            transform: rotate(180deg);
        }

        .faq-answer {
            padding: 0 var(--spacing-lg) var(--spacing-lg);
            color: #666;
            line-height: 1.8;
            max-height: 0;
            overflow: hidden;
            transition: max-height var(--transition-normal);
        }

        .faq-item.active .faq-answer {
            max-height: 500px;
            padding: var(--spacing-lg);
            padding-top: 0;
        }

        /* ============================================
           SECCIÓN FORMULARIO DE CONTACTO
           ============================================ */

        .contact {
            background: linear-gradient(135deg, var(--color-primary) 0%, var(--color-dark) 100%);
            color: var(--color-white);
        }

        .contact .section-title h2,
        .contact .section-title p {
            color: var(--color-white);
        }

        .form-container {
            max-width: 600px;
            margin: 0 auto;
        }

        .form-group {
            margin-bottom: var(--spacing-lg);
        }

        label {
            display: block;
            margin-bottom: var(--spacing-sm);
            font-weight: 500;
            color: rgba(255, 255, 255, 0.9);
            font-size: 0.95rem;
        }

        input, select, textarea {
            width: 100%;
            padding: 0.95rem;
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 8px;
            font-family: var(--font-body);
            background: rgba(255, 255, 255, 0.1);
            color: var(--color-white);
            transition: all var(--transition-normal);
            font-size: 1rem;
            backdrop-filter: blur(10px);
        }

        input::placeholder, select::placeholder, textarea::placeholder {
            color: rgba(255, 255, 255, 0.6);
        }

        input:focus, select:focus, textarea:focus {
            border-color: var(--color-accent);
            background: rgba(255, 255, 255, 0.15);
            outline: none;
            box-shadow: 0 0 0 3px rgba(255, 140, 0, 0.1);
        }

        textarea {
            resize: vertical;
            min-height: 140px;
            font-family: var(--font-body);
        }

        .form-submit {
            width: 100%;
            background: var(--color-accent);
            color: var(--color-white);
            padding: 1rem;
            border: none;
            border-radius: 8px;
            font-weight: 600;
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            cursor: pointer;
            transition: all var(--transition-normal);
            margin-top: var(--spacing-md);
        }

        .form-submit:hover {
            background: #ff7e00;
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
        }

        .form-message {
            padding: var(--spacing-md);
            border-radius: 8px;
            margin-top: var(--spacing-md);
            display: none;
        }

        .form-message.success {
            background: rgba(85, 113, 23, 0.3);
            color: var(--color-white);
            border: 1px solid rgba(85, 113, 23, 0.6);
            display: block;
        }

        .form-message.error {
            background: rgba(255, 50, 50, 0.3);
            color: var(--color-white);
            border: 1px solid rgba(255, 50, 50, 0.6);
            display: block;
        }

        .form-error {
            color: #ffcccc;
            font-size: 0.85rem;
            margin-top: 0.5rem;
            display: none;
        }

        input.error, select.error, textarea.error {
            border-color: #ff5555 !important;
        }

        input.error ~ .form-error,
        select.error ~ .form-error,
        textarea.error ~ .form-error {
            display: block;
        }

        /* ============================================
           SECCIÓN CTA FINAL
           ============================================ */

        .cta-final {
            background: linear-gradient(135deg, var(--color-accent) 0%, #ff7e00 100%);
            color: var(--color-white);
            position: relative;
            overflow: hidden;
            text-align: center;
        }

        .cta-final::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 800px;
            height: 800px;
            background: radial-gradient(circle, rgba(255, 255, 255, 0.1) 0%, transparent 70%);
            border-radius: 50%;
            pointer-events: none;
        }

        .cta-final-content {
            position: relative;
            z-index: 1;
        }

        .cta-final h2 {
            color: var(--color-white);
            margin-bottom: var(--spacing-lg);
        }

        .cta-final p {
            color: rgba(255, 255, 255, 0.95);
            font-size: 1.15rem;
            margin-bottom: var(--spacing-xl);
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* ============================================
           FOOTER
           ============================================ */

        footer {
            background: var(--color-dark);
            color: var(--color-white);
            padding: var(--spacing-xl) 0 var(--spacing-md);
        }

        footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: var(--spacing-xl);
            margin-bottom: var(--spacing-xl);
        }

        .footer-section h4 {
            color: var(--color-accent);
            margin-bottom: var(--spacing-md);
        }

        .footer-section p {
            color: rgba(255, 255, 255, 0.8);
            font-size: 0.95rem;
            margin-bottom: var(--spacing-sm);
        }

        .footer-links {
            display: flex;
            flex-direction: column;
            gap: var(--spacing-sm);
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
            transition: all var(--transition-normal);
        }

        .footer-links a:hover {
            color: var(--color-accent);
            padding-left: 5px;
        }

        .social-links {
            display: flex;
            gap: var(--spacing-md);
        }

        .social-links a {
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--color-accent);
            font-size: 1.2rem;
            transition: all var(--transition-normal);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .social-links a:hover {
            background: var(--color-accent);
            color: var(--color-white);
            transform: translateY(-3px);
        }

        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: var(--spacing-lg);
            text-align: center;
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.9rem;
        }

        /* ============================================
           ANIMACIONES Y EFECTOS
           ============================================ */

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeInLeft {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes fadeInRight {
            from {
                opacity: 0;
                transform: translateX(30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }

        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateX(-50%) translateY(0);
            }
            50% {
                transform: translateX(-50%) translateY(-10px);
            }
        }

        @keyframes countUp {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        .animate-in {
            animation: fadeInUp 0.8s ease-out forwards;
        }

        .animate-in-left {
            animation: fadeInLeft 0.8s ease-out forwards;
        }

        .animate-in-right {
            animation: fadeInRight 0.8s ease-out forwards;
        }

        .animate-in-stagger-1 { animation-delay: 0.1s; }
        .animate-in-stagger-2 { animation-delay: 0.2s; }
        .animate-in-stagger-3 { animation-delay: 0.3s; }
        .animate-in-stagger-4 { animation-delay: 0.4s; }
        .animate-in-stagger-5 { animation-delay: 0.5s; }
        .animate-in-stagger-6 { animation-delay: 0.6s; }

        /* ============================================
           RESPONSIVE DESIGN
           ============================================ */

        @media (max-width: 768px) {
            .hamburger {
                display: flex;
            }

            .nav-menu {
                position: fixed;
                left: -100%;
                top: 70px;
                flex-direction: column;
                background-color: rgba(0, 0, 0, 0.95);
                width: 100%;
                text-align: center;
                transition: 0.3s;
                box-shadow: var(--shadow-lg);
                padding: var(--spacing-lg) 0;
                gap: var(--spacing-md);
                z-index: 999;
                backdrop-filter: blur(10px);
            }

            .nav-menu.active {
                left: 0;
            }

            header.sticky .nav-menu a {
                color: var(--color-white);
            }

            .about-content,
            .veleta-experience-content {
                grid-template-columns: 1fr;
            }

            .about-image {
                height: 350px;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: center;
            }

            .hero-buttons .btn {
                width: 100%;
                max-width: 300px;
            }

            .gallery-grid {
                grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            }

            .calendar-grid {
                grid-template-columns: repeat(2, 1fr);
            }

            h1 {
                font-size: 2rem;
            }

            h2 {
                font-size: 1.5rem;
            }

            .section {
                padding: var(--spacing-xl) 0;
            }

            .hero {
                min-height: 500px;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .hero-subtitle {
                font-size: 1rem;
            }

            .activity-card {
                margin-bottom: var(--spacing-md);
            }

            input, select, textarea {
                font-size: 16px;
            }
        }

        @media (max-width: 480px) {
            .container {
                padding: 0 var(--spacing-sm);
            }

            .hero h1 {
                font-size: 1.5rem;
                text-transform: none;
            }

            .hero-subtitle {
                font-size: 0.9rem;
            }

            .hero-buttons {
                gap: var(--spacing-sm);
            }

            .btn {
                padding: 0.75rem 1.25rem;
                font-size: 0.85rem;
            }

            .section {
                padding: var(--spacing-lg) 0;
            }

            .section-title h2 {
                font-size: 1.3rem;
            }

            .stat-number {
                font-size: 2rem;
            }

            .stat-label {
                font-size: 0.9rem;
            }

            .why-grid {
                grid-template-columns: 1fr;
            }

            .testimonial-card {
                padding: var(--spacing-md);
            }

            .faq-question {
                padding: var(--spacing-md);
            }

            .form-group {
                margin-bottom: var(--spacing-md);
            }

            footer-content {
                grid-template-columns: 1fr;
            }
        }

        /* ============================================
           PRINT STYLES
           ============================================ */

        @media print {
            header, .hero, .cta-final, .contact {
                display: none;
            }

            body {
                font-size: 12pt;
                color: #000;
            }

            a {
                color: #000;
                text-decoration: underline;
            }
        }

        /* ============================================
           ACCESIBILIDAD
           ============================================ */

        @media (prefers-reduced-motion: reduce) {
            * {
                animation-duration: 0.01ms !important;
                animation-iteration-count: 1 !important;
                transition-duration: 0.01ms !important;
                scroll-behavior: auto !important;
            }
        }

        .visually-hidden {
            position: absolute;
            width: 1px;
            height: 1px;
            padding: 0;
            margin: -1px;
            overflow: hidden;
            clip: rect(0, 0, 0, 0);
            white-space: nowrap;
            border-width: 0;
        }

        :focus-visible {
            outline: 3px solid var(--color-accent);
            outline-offset: 2px;
        }
    </style>
</head>
<body>
    <!-- HEADER Y NAVEGACIÓN -->
    <header id="header">
        <div class="container">
            <nav>
                <div class="logo">
                    🏔️ VELETA<span>ADVENTURE</span>
                </div>
                <ul class="nav-menu" id="nav-menu">
                    <li><a href="#inicio">Inicio</a></li>
                    <li><a href="#quienes-somos">Quiénes Somos</a></li>
                    <li><a href="#actividades">Actividades</a></li>
                    <li><a href="#experiencias">Experiencias</a></li>
                    <li><a href="#galeria">Galería</a></li>
                    <li><a href="#contacto">Contacto</a></li>
                    <li><a href="#contacto" class="cta-btn">Reservar</a></li>
                </ul>
                <div class="hamburger" id="hamburger">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </nav>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section class="hero" id="inicio">
        <div class="hero-content">
            <h1>Descubre Nuestras Actividades</h1>
            <p class="hero-subtitle">Actividades variadas, pensadas para todos los públicos</p>
            <div class="hero-buttons">
                <a href="#contacto" class="btn btn-primary">Reservar Ahora</a>
                <a href="#actividades" class="btn btn-secondary">Descubrir Actividades</a>
            </div>
        </div>
        <div class="scroll-indicator">
            <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M12 5V19M19 12L12 19L5 12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
        </div>
    </section>

    <!-- SECCIÓN QUIÉNES SOMOS -->
    <section class="section about" id="quienes-somos">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>Quiénes Somos</h2>
                    <p>Veleta Adventure es una empresa especializada en turismo activo y experiencias de naturaleza. Desde 2015, hemos llevado a miles de personas a vivir aventuras inolvidables en los paisajes más hermosos de España.</p>
                    
                    <p>Nuestra misión es democratizar el acceso a actividades de aventura de calidad, garantizando la máxima seguridad y profesionalidad en cada experiencia. Creemos que la naturaleza es el mejor aula para aprender, crecer y conectar con nosotros mismos.</p>

                    <div class="about-features">
                        <div class="feature-item">
                            <div class="feature-icon">🎯</div>
                            <div>
                                <h4>Filosofía de Aventura</h4>
                                <p>Cada salida es cuidadosamente diseñada para maximizar la seguridad sin comprometer la emoción.</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">🌿</div>
                            <div>
                                <h4>Respeto por la Naturaleza</h4>
                                <p>Practicamos un turismo responsable y sostenible que preserva nuestros ecosistemas.</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">👥</div>
                            <div>
                                <h4>Comunidad Global</h4>
                                <p>Hemos creado una comunidad de amantes de la aventura que comparten nuestros valores.</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="about-image"></div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN ACTIVIDADES -->
    <section class="section activities" id="actividades">
        <div class="container">
            <div class="section-title">
                <div class="accent-line"></div>
                <h2>Nuestras Actividades</h2>
                <p>Elige la aventura que mejor se adapta a ti. Todas nuestras actividades están diseñadas con estándares internacionales de seguridad.</p>
            </div>

            <div class="activities-grid">
                <div class="activity-card">
                    <div class="activity-image">🥾</div>
                    <div class="activity-content">
                        <div class="activity-header">
                            <div class="activity-icon">🏔️</div>
                            <div>
                                <h3>Rutas de Senderismo</h3>
                            </div>
                        </div>
                        <p class="activity-description">Explora nuestras rutas guiadas por profesionales. Desde caminatas suaves hasta rutas desafiantes de montaña. Adecuado para todos los niveles.</p>
                        <div class="activity-footer">
                            <span class="activity-badge">Popular</span>
                            <a href="#contacto" class="activity-link">Más Info →</a>
                        </div>
                    </div>
                </div>

                <div class="activity-card">
                    <div class="activity-image">🚴</div>
                    <div class="activity-content">
                        <div class="activity-header">
                            <div class="activity-icon">🚵</div>
                            <div>
                                <h3>Rutas en Bicicleta</h3>
                            </div>
                        </div>
                        <p class="activity-description">Aventuras sobre dos ruedas por senderos y caminos de tierra. Desde bici de montaña hasta cicloturismo. Material profesional incluido.</p>
                        <div class="activity-footer">
                            <span class="activity-badge">Emocionante</span>
                            <a href="#contacto" class="activity-link">Más Info →</a>
                        </div>
                    </div>
                </div>

                <div class="activity-card">
                    <div class="activity-image">🧩</div>
                    <div class="activity-content">
                        <div class="activity-header">
                            <div class="activity-icon">🎪</div>
                            <div>
                                <h3>Gymkanas</h3>
                            </div>
                        </div>
                        <p class="activity-description">Competiciones divertidas y desafiantes para grupos. Pruebas de orientación, equilibrio y trabajo en equipo en entornos naturales.</p>
                        <div class="activity-footer">
                            <span class="activity-badge">Grupos</span>
                            <a href="#contacto" class="activity-link">Más Info →</a>
                        </div>
                    </div>
                </div>

                <div class="activity-card">
                    <div class="activity-image">🏕️</div>
                    <div class="activity-content">
                        <div class="activity-header">
                            <div class="activity-icon">⛺</div>
                            <div>
                                <h3>Packs Multiaventura</h3>
                            </div>
                        </div>
                        <p class="activity-description">Experiencias combinadas: senderismo, escalada, rappel y más. Ideal para grupos corporativos y eventos especiales.</p>
                        <div class="activity-footer">
                            <span class="activity-badge">Premium</span>
                            <a href="#contacto" class="activity-link">Más Info →</a>
                        </div>
                    </div>
                </div>

                <div class="activity-card">
                    <div class="activity-image special">⭐</div>
                    <div class="activity-content">
                        <div class="activity-header">
                            <div class="activity-icon">✨</div>
                            <div>
                                <h3>Veleta Experience</h3>
                            </div>
                        </div>
                        <p class="activity-description">Actividades mensuales exclusivas y únicas. Experiencias especiales diseñadas por nuestro equipo con elementos sorpresa y experiencias premium.</p>
                        <div class="activity-footer">
                            <span class="activity-badge special">Exclusiva</span>
                            <a href="#experiencias" class="activity-link">Descubrir →</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN VELETA EXPERIENCE -->
    <section class="section veleta-experience" id="experiencias">
        <div class="container">
            <div class="veleta-experience-content">
                <div class="veleta-text">
                    <h2>Veleta Experience</h2>
                    <p>Nuestro programa de experiencias exclusivas te ofrece actividades mensuales diseñadas especialmente para amantes de la aventura que buscan algo diferente.</p>
                    
                    <div class="veleta-highlights">
                        <div class="veleta-highlight">
                            <div class="veleta-highlight-icon">🌟</div>
                            <div>
                                <h4>Actividades Exclusivas</h4>
                                <p>Acceso a experiencias no disponibles al público general.</p>
                            </div>
                        </div>
                        <div class="veleta-highlight">
                            <div class="veleta-highlight-icon">🎁</div>
                            <div>
                                <h4>Sorpresas Premium</h4>
                                <p>Cada mes traemos experiencias nuevas y emocionantes.</p>
                            </div>
                        </div>
                        <div class="veleta-highlight">
                            <div class="veleta-highlight-icon">👑</div>
                            <div>
                                <h4>Atención VIP</h4>
                                <p>Grupos reducidos y atención personalizada garantizada.</p>
                            </div>
                        </div>
                        <div class="veleta-highlight">
                            <div class="veleta-highlight-icon">🏆</div>
                            <div>
                                <h4>Beneficios Extras</h4>
                                <p>Descuentos, eventos exclusivos y comunidad privada.</p>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="calendar-preview">
                    <h3 style="color: white; text-align: center; margin-bottom: var(--spacing-lg);">Próximas Experiencias</h3>
                    <div class="calendar-grid">
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">01</div>
                            <div style="font-size: 0.8rem;">ENERO</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">02</div>
                            <div style="font-size: 0.8rem;">FEBRERO</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">03</div>
                            <div style="font-size: 0.8rem;">MARZO</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">04</div>
                            <div style="font-size: 0.8rem;">ABRIL</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">05</div>
                            <div style="font-size: 0.8rem;">MAYO</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">06</div>
                            <div style="font-size: 0.8rem;">JUNIO</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">07</div>
                            <div style="font-size: 0.8rem;">JULIO</div>
                        </div>
                        <div class="calendar-month">
                            <div style="font-size: 1.5rem; margin-bottom: 0.5rem;">08</div>
                            <div style="font-size: 0.8rem;">AGOSTO</div>
                        </div>
                    </div>
                    <p style="text-align: center; color: rgba(255,255,255,0.8); margin-top: var(--spacing-lg); font-size: 0.9rem;">¡Consulta nuestro calendario completo en tu área personal!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN POR QUÉ ELEGIRNOS -->
    <section class="section why-choose">
        <div class="container">
            <div class="section-title">
                <div class="accent-line"></div>
                <h2>Por Qué Elegirnos</h2>
                <p>Descubre qué nos diferencia del resto en el turismo activo.</p>
            </div>

            <div class="why-grid">
                <div class="why-card animate-in animate-in-stagger-1">
                    <div class="why-card-icon">🛡️</div>
                    <h3>Seguridad Garantizada</h3>
                    <p>Certificaciones internacionales y revisión constante de equipos y procedimientos de seguridad.</p>
                </div>

                <div class="why-card animate-in animate-in-stagger-2">
                    <div class="why-card-icon">🎓</div>
                    <h3>Monitores Especializados</h3>
                    <p>Profesionales con años de experiencia y formación continua en seguridad y técnica.</p>
                </div>

                <div class="why-card animate-in animate-in-stagger-3">
                    <div class="why-card-icon">👨‍👩‍👧‍👦</div>
                    <h3>Para Todos los Públicos</h3>
                    <p>Actividades adaptadas desde niños hasta adultos, y para todos los niveles de experiencia.</p>
                </div>

                <div class="why-card animate-in animate-in-stagger-4">
                    <div class="why-card-icon">🌍</div>
                    <h3>Respeto Ambiental</h3>
                    <p>Práctica del turismo responsable y contribución a la conservación de espacios naturales.</p>
                </div>

                <div class="why-card animate-in animate-in-stagger-5">
                    <div class="why-card-icon">💫</div>
                    <h3>Experiencias Únicas</h3>
                    <p>Vivencias personalizadas que te marcarán para siempre. Momentos inolvidables.</p>
                </div>

                <div class="why-card animate-in animate-in-stagger-6">
                    <div class="why-card-icon">🏢</div>
                    <h3>Grupos y Empresas</h3>
                    <p>Soluciones especiales para team building, eventos corporativos y grupos grandes.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN ESTADÍSTICAS -->
    <section class="section stats" id="stats">
        <div class="container">
            <div class="stats-grid">
                <div class="stat-card">
                    <div class="stat-number" data-target="500">0</div>
                    <div class="stat-label">Clientes Satisfechos</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number" data-target="150">0</div>
                    <div class="stat-label">Experiencias Realizadas</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number" data-target="100">0</div>
                    <div class="stat-label">% de Diversión</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number" data-target="365">0</div>
                    <div class="stat-label">Días de Aventura al Año</div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN GALERÍA -->
    <section class="section gallery" id="galeria">
        <div class="container">
            <div class="section-title">
                <div class="accent-line"></div>
                <h2>Galería de Aventuras</h2>
                <p>Mira los momentos más emocionantes capturados en nuestras expediciones.</p>
            </div>

            <div class="gallery-grid">
                <div class="gallery-item">
                    <div class="gallery-item-image">🏔️</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🚵</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🌲</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🧗</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">⛺</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🏞️</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🌅</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🎒</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🌊</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🦅</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🌸</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
                <div class="gallery-item">
                    <div class="gallery-item-image">🌙</div>
                    <div class="gallery-overlay">
                        <div class="gallery-icon">🔍</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN TESTIMONIOS -->
    <section class="section testimonials">
        <div class="container">
            <div class="section-title">
                <div class="accent-line"></div>
                <h2>Lo Que Dicen Nuestros Clientes</h2>
                <p>Descubre las experiencias reales de quienes ya han vivido una aventura con nosotros.</p>
            </div>

            <div class="testimonial-carousel">
                <div class="testimonial-card active">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">MC</div>
                        <div class="testimonial-info">
                            <h4>María Católo</h4>
                            <p>Madrid, España</p>
                        </div>
                    </div>
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Una experiencia increíble. Los monitores fueron excepcionales, atentos y profesionales. La seguridad fue primordial pero sin perder la diversión. ¡Repetiremos seguro!"</p>
                </div>

                <div class="testimonial-card">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">JG</div>
                        <div class="testimonial-info">
                            <h4>Juan García</h4>
                            <p>Barcelona, España</p>
                        </div>
                    </div>
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Veleta Adventure superó todas mis expectativas. Una compañía realmente comprometida con la excelencia y la naturaleza. Gracias por esta aventura."</p>
                </div>

                <div class="testimonial-card">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">SL</div>
                        <div class="testimonial-info">
                            <h4>Sandra López</h4>
                            <p>Valencia, España</p>
                        </div>
                    </div>
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Mi familia disfrutó muchísimo. Actividades para todos los niveles y momentos memorables. El mejor dinero invertido en una experiencia familiar."</p>
                </div>

                <div class="testimonial-card">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">PM</div>
                        <div class="testimonial-info">
                            <h4>Pedro Martínez</h4>
                            <p>Sevilla, España</p>
                        </div>
                    </div>
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Para nuestro evento corporativo fue perfecto. Equipo profesional, organización impecable y una experiencia que unió a nuestro equipo como nunca."</p>
                </div>

                <div class="testimonial-card">
                    <div class="testimonial-header">
                        <div class="testimonial-avatar">AB</div>
                        <div class="testimonial-info">
                            <h4>Ana Blanco</h4>
                            <p>Bilbao, España</p>
                        </div>
                    </div>
                    <div class="stars">★★★★★</div>
                    <p class="testimonial-text">"Recomiendo Veleta Adventure a todos mis amigos. Es una empresa que entiende el turismo activo como debe ser: seguro, divertido y responsable."</p>
                </div>
            </div>

            <div class="carousel-nav">
                <div class="carousel-dot active" onclick="changeTestimonial(0)"></div>
                <div class="carousel-dot" onclick="changeTestimonial(1)"></div>
                <div class="carousel-dot" onclick="changeTestimonial(2)"></div>
                <div class="carousel-dot" onclick="changeTestimonial(3)"></div>
                <div class="carousel-dot" onclick="changeTestimonial(4)"></div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN FAQ -->
    <section class="section faq">
        <div class="container">
            <div class="section-title">
                <div class="accent-line"></div>
                <h2>Preguntas Frecuentes</h2>
                <p>Resolvemos tus dudas sobre nuestras actividades y servicios.</p>
            </div>

            <div class="faq-container">
                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Cuál es la edad mínima para participar?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        La edad mínima depende de la actividad. Nuestras rutas de senderismo son aptas desde los 5 años, bicicleta desde los 8 años, y actividades más técnicas desde los 12 años. Siempre bajo supervisión de padres o tutores cuando es necesario.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Qué debo llevar a una actividad?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        Proveemos una lista de recomendaciones específica para cada actividad. Generalmente necesitarás ropa cómoda, calzado apropiado, protector solar y agua. El equipo técnico lo proporcionamos nosotros.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Son las actividades aptas para principiantes?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        Absolutamente. Ofrecemos actividades para todos los niveles. Nuestros monitores adaptarán la intensidad y ritmo según la capacidad del grupo. No se requiere experiencia previa.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Cuál es vuestra política de cancelación?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        Ofrecemos reembolso completo si cancelas con 7 días de anticipación. Si cancelas con menos tiempo, se aplica un descuento según los días previos al evento. En caso de mal tiempo extremo, rescheduleamos sin costo adicional.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Hacen actividades para grupos corporativos?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        Sí, somos expertos en eventos corporativos. Ofrecemos packs personalizados de team building, actividades de motivación y experiencias únicas. Consúltanos sobre precios especiales para grupos grandes.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Cuál es la duración típica de una actividad?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        Depende de la actividad elegida. Las rutas de senderismo oscilan entre 3-8 horas, las de bicicleta 3-6 horas, y las actividades de multiaventura 5-10 horas. Consulta los detalles específicos de cada experiencia.
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">
                        <h4>¿Qué pasa si hay mal tiempo?</h4>
                        <span class="faq-toggle">▼</span>
                    </div>
                    <div class="faq-answer">
                        La seguridad es nuestra prioridad. Si las condiciones climáticas son peligrosas, ofrecemos reprogramar sin costo adicional. Las ligeras lluvias no impiden nuestras actividades si son seguras.
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- SECCIÓN CONTACTO -->
    <section class="section contact" id="contacto">
        <div class="container">
            <div class="section-title">
                <div class="accent-line" style="background: rgba(255,255,255,0.3);"></div>
                <h2>¿Preparado para Tu Próxima Aventura?</h2>
                <p>Contáctanos hoy mismo. Nuestro equipo responderá en menos de 24 horas.</p>
            </div>

            <div class="form-container">
                <form id="contactForm">
                    <div class="form-group">
                        <label for="nombre">Nombre Completo *</label>
                        <input type="text" id="nombre" name="nombre" required>
                        <span class="form-error">Por favor introduce tu nombre</span>
                    </div>

                    <div class="form-group">
                        <label for="email">Correo Electrónico *</label>
                        <input type="email" id="email" name="email" required>
                        <span class="form-error">Por favor introduce un correo válido</span>
                    </div>

                    <div class="form-group">
                        <label for="telefono">Teléfono *</label>
                        <input type="tel" id="telefono" name="telefono" required>
                        <span class="form-error">Por favor introduce un teléfono válido</span>
                    </div>

                    <div class="form-group">
                        <label for="actividad">¿Qué actividad te interesa? *</label>
                        <select id="actividad" name="actividad" required>
                            <option value="">Selecciona una actividad</option>
                            <option value="senderismo">Rutas de Senderismo</option>
                            <option value="bicicleta">Rutas en Bicicleta</option>
                            <option value="gymkanas">Gymkanas</option>
                            <option value="multiaventura">Packs Multiaventura</option>
                            <option value="experience">Veleta Experience</option>
                            <option value="otro">Otra / Consulta</option>
                        </select>
                        <span class="form-error">Por favor selecciona una actividad</span>
                    </div>

                    <div class="form-group">
                        <label for="mensaje">Mensaje *</label>
                        <textarea id="mensaje" name="mensaje" required></textarea>
                        <span class="form-error">Por favor introduce un mensaje</span>
                    </div>

                    <button type="submit" class="form-submit">Enviar Solicitud</button>
                    <div class="form-message"></div>
                </form>
            </div>
        </div>
    </section>

    <!-- SECCIÓN CTA FINAL -->
    <section class="section cta-final">
        <div class="container">
            <div class="cta-final-content">
                <h2>¿Preparado para Tu Próxima Aventura?</h2>
                <p>Únete a cientos de exploradores que ya han vivido experiencias inolvidables con Veleta Adventure. El próximo capítulo de tu historia de aventura te espera.</p>
                <a href="#contacto" class="btn btn-white">Reservar Ahora</a>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="container">
            <footer-content>
                <div class="footer-section">
                    <h4>🏔️ Veleta Adventure</h4>
                    <p>Tu puerta a las más emocionantes aventuras en la naturaleza. Profesionalidad, seguridad y diversión garantizadas.</p>
                </div>

                <div class="footer-section">
                    <h4>Enlaces Rápidos</h4>
                    <div class="footer-links">
                        <a href="#inicio">Inicio</a>
                        <a href="#quienes-somos">Quiénes Somos</a>
                        <a href="#actividades">Actividades</a>
                        <a href="#experiencias">Experiencias</a>
                        <a href="#contacto">Contacto</a>
                    </div>
                </div>

                <div class="footer-section">
                    <h4>Síguenos</h4>
                    <div class="social-links">
                        <a href="#" title="Facebook">f</a>
                        <a href="#" title="Instagram">📷</a>
                        <a href="#" title="Twitter">𝕏</a>
                        <a href="#" title="YouTube">▶</a>
                    </div>
                </div>

                <div class="footer-section">
                    <h4>Contacto</h4>
                    <p>📧 info@veleta-adventure.com</p>
                    <p>📞 +34 600 000 000</p>
                    <p>📍 Granada, España</p>
                </div>
            </footer-content>

            <div class="footer-bottom">
                <p>&copy; 2024 Veleta Adventure. Todos los derechos reservados. | Política de Privacidad | Términos de Servicio</p>
            </div>
        </div>
    </footer>

    <script>
        // ============================================
        // JAVASCRIPT VANILLA - FUNCIONALIDADES
        // ============================================

        // ============================================
        // HEADER STICKY Y MENÚ MÓVIL
        // ============================================

        const header = document.getElementById('header');
        const hamburger = document.getElementById('hamburger');
        const navMenu = document.getElementById('nav-menu');

        // Sticky header al hacer scroll
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                header.classList.add('sticky');
            } else {
                header.classList.remove('sticky');
            }
        });

        // Menú hamburguesa
        hamburger.addEventListener('click', () => {
            hamburger.classList.toggle('active');
            navMenu.classList.toggle('active');
        });

        // Cerrar menú al hacer click en un link
        document.querySelectorAll('.nav-menu a').forEach(link => {
            link.addEventListener('click', () => {
                hamburger.classList.remove('active');
                navMenu.classList.remove('active');
            });
        });

        // ============================================
        // INTERSECTION OBSERVER - ANIMACIONES AL SCROLL
        // ============================================

        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -100px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('animate-in');
                    observer.unobserve(entry.target);
                }
            });
        }, observerOptions);

        // Observar elementos con clase animate-in
        document.querySelectorAll('.animate-in').forEach(element => {
            observer.observe(element);
        });

        // ============================================
        // CONTADORES ANIMADOS - ESTADÍSTICAS
        // ============================================

        function animateCounter(element) {
            const target = parseInt(element.dataset.target);
            const duration = 2000;
            const start = Date.now();

            function update() {
                const progress = (Date.now() - start) / duration;
                if (progress < 1) {
                    const current = Math.floor(target * progress);
                    element.textContent = current;
                    requestAnimationFrame(update);
                } else {
                    element.textContent = target;
                }
            }

            update();
        }

        // Observar cuando llegan a viewport los contadores
        const statsObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    document.querySelectorAll('[data-target]').forEach(element => {
                        if (element.textContent === '0') {
                            animateCounter(element);
                        }
                    });
                    statsObserver.unobserve(entry.target);
                }
            });
        }, { threshold: 0.5 });

        const statsSection = document.getElementById('stats');
        if (statsSection) {
            statsObserver.observe(statsSection);
        }

        // ============================================
        // CARRUSEL DE TESTIMONIOS
        // ============================================

        let currentTestimonial = 0;
        const testimonialCards = document.querySelectorAll('.testimonial-card');
        const testimonialDots = document.querySelectorAll('.carousel-dot');

        function showTestimonial(index) {
            testimonialCards.forEach(card => card.classList.remove('active'));
            testimonialDots.forEach(dot => dot.classList.remove('active'));
            
            testimonialCards[index].classList.add('active');
            testimonialDots[index].classList.add('active');
        }

        function changeTestimonial(index) {
            currentTestimonial = index;
            showTestimonial(index);
        }

        // Auto-rotar testimonios cada 5 segundos
        setInterval(() => {
            currentTestimonial = (currentTestimonial + 1) % testimonialCards.length;
            showTestimonial(currentTestimonial);
        }, 5000);

        // ============================================
        // PREGUNTAS FAQ - ACORDEÓN
        // ============================================

        document.querySelectorAll('.faq-question').forEach(question => {
            question.addEventListener('click', () => {
                const faqItem = question.parentElement;
                const isActive = faqItem.classList.contains('active');

                // Cerrar todos los demás
                document.querySelectorAll('.faq-item').forEach(item => {
                    if (item !== faqItem) {
                        item.classList.remove('active');
                    }
                });

                // Toggle actual
                faqItem.classList.toggle('active');
            });
        });

        // ============================================
        // VALIDACIÓN Y ENVÍO DE FORMULARIO
        // ============================================

        const contactForm = document.getElementById('contactForm');
        const formMessage = contactForm.querySelector('.form-message');

        // Validación en tiempo real
        contactForm.querySelectorAll('input, select, textarea').forEach(field => {
            field.addEventListener('blur', () => {
                validateField(field);
            });

            field.addEventListener('input', () => {
                if (field.classList.contains('error')) {
                    validateField(field);
                }
            });
        });

        function validateField(field) {
            let isValid = true;

            if (field.type === 'email') {
                const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
                isValid = emailRegex.test(field.value);
            } else if (field.type === 'tel') {
                const phoneRegex = /^[\d\s\-\+\(\)]{7,}$/;
                isValid = phoneRegex.test(field.value) || field.value === '';
            } else if (field.required) {
                isValid = field.value.trim() !== '';
            }

            if (isValid) {
                field.classList.remove('error');
            } else {
                field.classList.add('error');
            }

            return isValid;
        }

        function validateForm() {
            let isFormValid = true;
            contactForm.querySelectorAll('[required]').forEach(field => {
                if (!validateField(field)) {
                    isFormValid = false;
                }
            });
            return isFormValid;
        }

        // Envío del formulario
        contactForm.addEventListener('submit', async (e) => {
            e.preventDefault();

            if (!validateForm()) {
                formMessage.classList.remove('success');
                formMessage.classList.add('error');
                formMessage.textContent = '⚠️ Por favor completa todos los campos correctamente.';
                formMessage.style.display = 'block';
                return;
            }

            // Simular envío (en producción, enviar a servidor)
            const submitBtn = contactForm.querySelector('.form-submit');
            submitBtn.disabled = true;
            submitBtn.textContent = 'Enviando...';

            setTimeout(() => {
                formMessage.classList.remove('error');
                formMessage.classList.add('success');
                formMessage.textContent = '✅ ¡Gracias por tu solicitud! Nos pondremos en contacto en las próximas 24 horas.';
                contactForm.reset();
                document.querySelectorAll('input, select, textarea').forEach(field => {
                    field.classList.remove('error');
                });

                submitBtn.disabled = false;
                submitBtn.textContent = 'Enviar Solicitud';

                setTimeout(() => {
                    formMessage.style.display = 'none';
                }, 5000);
            }, 1000);
        });

        // ============================================
        // EFECTO PARALLAX
        // ============================================

        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('.hero');
            
            if (hero) {
                hero.style.backgroundPosition = `center ${scrolled * 0.5}px`;
            }
        });

        // ============================================
        // SMOOTH SCROLL BEHAVIOR
        // ============================================

        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // ============================================
        // LAZY LOADING SIMULATION
        // ============================================

        const lazyImages = document.querySelectorAll('[data-src]');
        const imageObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const img = entry.target;
                    img.src = img.dataset.src;
                    img.removeAttribute('data-src');
                    imageObserver.unobserve(img);
                }
            });
        });

        lazyImages.forEach(img => imageObserver.observe(img));

        // ============================================
        // INICIALIZACIÓN
        // ============================================

        console.log('🏔️ Veleta Adventure - Web Premium Cargada Correctamente');
        console.log('Todas las animaciones y funcionalidades están activas.');
    </script>

---
---
/* Esto importa el tema original de GitHub Pages */
@import "{{ site.theme }}";

/* Sobrescribe el ancho máximo de las páginas para que ocupen todo el viewport */
.container-lg, .container-xl, .container {
    max-width: 100% !important;
    padding-left: 0 !important;
    padding-right: 0 !important;
}


</body>
</html>
