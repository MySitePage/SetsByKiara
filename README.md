
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0, user-scalable=yes">
    <title>Sets by Kiara | Luxury Nail Artist | Midland, Texas</title>
    
    <!-- Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;1,400&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
    
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        /* ============================================
           DARK GREY THEME WITH PINK/PURPLE ACCENTS
        ============================================= */
        :root {
            /* Dark Grey Colors */
            --color-dark-base: #1a1a1a;       /* Dark grey background */
            --color-dark-card: #2a2a2a;       /* Dark grey cards */
            --color-dark-border: #3a3a3a;     /* Dark borders */
            --color-dark-text: #e0e0e0;       /* Light text on dark */
            --color-light-text: #ffffff;      /* White text */
            --color-muted-text: #aaaaaa;      /* Muted text */
            
            /* Accent Colors */
            --color-light-pink: #FF85A2;      /* Pink accent */
            --color-soft-pink: #F8C8DC;       /* Soft pink */
            --color-lavender: #E6CCFF;        /* Light lavender */
            --color-lilac: #D8B4FE;           /* Soft lilac */
            --color-light-purple: #B19CD9;    /* Purple accent */
            
            /* Gradients */
            --gradient-main: linear-gradient(135deg, var(--color-dark-card) 0%, var(--color-dark-base) 100%);
            --gradient-accent: linear-gradient(45deg, var(--color-light-pink), var(--color-light-purple));
            --gradient-card: linear-gradient(145deg, var(--color-dark-card) 0%, #252525 100%);
            
            /* Fonts */
            --font-heading: 'Playfair Display', Georgia, serif;
            --font-body: 'Poppins', -apple-system, BlinkMacSystemFont, sans-serif;
            
            /* Spacing */
            --space-xs: 0.5rem;
            --space-sm: 1rem;
            --space-md: 1.5rem;
            --space-lg: 2rem;
            --space-xl: 3rem;
            --space-xxl: 4rem;
            
            /* Mobile Spacing */
            --mobile-space-xs: 0.25rem;
            --mobile-space-sm: 0.75rem;
            --mobile-space-md: 1rem;
            --mobile-space-lg: 1.5rem;
            --mobile-space-xl: 2rem;
            
            /* Border Radius */
            --radius-sm: 8px;
            --radius-md: 12px;
            --radius-lg: 16px;
            --radius-xl: 24px;
            --radius-round: 50px;
            
            /* Shadows */
            --shadow-soft: 0 4px 20px rgba(0, 0, 0, 0.3);
            --shadow-medium: 0 8px 30px rgba(0, 0, 0, 0.4);
            --shadow-float: 0 15px 40px rgba(0, 0, 0, 0.5);
            
            /* Transitions */
            --transition-fast: 0.2s ease;
            --transition-normal: 0.3s ease;
            --transition-slow: 0.5s ease;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        html {
            scroll-behavior: smooth;
            font-size: 16px;
        }

        body {
            font-family: var(--font-body);
            font-weight: 400;
            line-height: 1.6;
            color: var(--color-dark-text);
            background-color: var(--color-dark-base);
            overflow-x: hidden;
            min-height: 100vh;
            -webkit-text-size-adjust: 100%;
            -webkit-font-smoothing: antialiased;
        }

        /* ============================================
           UTILITY CLASSES
        ============================================= */
        .hidden {
            display: none !important;
        }

        .page {
            min-height: 100vh;
            padding-top: 70px;
        }

        .img-placeholder {
            background: linear-gradient(135deg, var(--color-dark-card), var(--color-dark-border));
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--color-light-purple);
            font-weight: 500;
            font-size: 1rem;
            text-align: center;
            padding: 1rem;
        }

        /* ============================================
           TOUCH-FRIENDLY ELEMENTS
        ============================================= */
        button,
        a,
        .btn,
        .btn-nav,
        .btn-hero,
        .form-submit,
        .social-icon,
        .phone-number,
        .gallery-item,
        .time-slot {
            cursor: pointer;
            touch-action: manipulation;
            -webkit-touch-callout: none;
            -webkit-user-select: none;
            user-select: none;
        }

        input,
        select,
        textarea {
            font-size: 16px !important; /* Prevents iOS zoom on focus */
        }

        /* ============================================
           HEADER & NAVIGATION - MOBILE OPTIMIZED
        ============================================= */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(26, 26, 26, 0.98);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--color-dark-border);
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.3);
            height: 70px;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 100%;
        }

        .logo {
            font-family: var(--font-heading);
            font-size: 1.5rem;
            font-weight: 500;
            color: white;
            text-decoration: none;
            background: var(--gradient-accent);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            white-space: nowrap;
        }

        .nav-links {
            display: flex;
            gap: 1.5rem;
            align-items: center;
        }

        .nav-links a {
            color: var(--color-dark-text);
            text-decoration: none;
            font-weight: 500;
            padding: 0.5rem 0;
            position: relative;
            transition: color var(--transition-fast);
            font-size: 0.95rem;
        }

        .nav-links a:hover {
            color: white;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--gradient-accent);
            transition: width var(--transition-normal);
        }

        .nav-links a:hover::after,
        .nav-links a.active::after {
            width: 100%;
        }

        .btn-nav {
            padding: 0.6rem 1.25rem;
            background: var(--gradient-accent);
            color: white;
            border: none;
            border-radius: var(--radius-round);
            font-weight: 500;
            cursor: pointer;
            text-decoration: none;
            transition: all var(--transition-normal);
            font-size: 0.9rem;
            white-space: nowrap;
        }

        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--color-dark-text);
            cursor: pointer;
            padding: 0.5rem;
            margin-left: 1rem;
        }

        /* ============================================
           HOME PAGE - MOBILE OPTIMIZED
        ============================================= */
        #home-page {
            display: block;
        }

        /* Hero Section - Mobile Optimized */
        .hero {
            min-height: 85vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            background: var(--gradient-main);
            padding: 0 20px;
        }

        .hero-background {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 1;
            opacity: 0.4;
        }

        .hero-content {
            position: relative;
            z-index: 2;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
            padding: 2rem 0;
            width: 100%;
        }

        .hero h1 {
            font-size: clamp(2rem, 7vw, 3.5rem);
            color: white;
            margin-bottom: var(--space-sm);
            background: var(--gradient-accent);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            line-height: 1.2;
        }

        .hero-tagline {
            font-size: clamp(0.9rem, 3vw, 1.1rem);
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-bottom: var(--space-xl);
            color: white;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
            line-height: 1.4;
        }

        .btn-hero {
            padding: 0.9rem 2rem;
            background: var(--gradient-accent);
            color: white;
            border: none;
            border-radius: var(--radius-round);
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 1px;
            cursor: pointer;
            transition: all var(--transition-normal);
            text-decoration: none;
            display: inline-block;
            font-size: 0.9rem;
            min-width: 200px;
        }

        /* Booking Steps - Mobile Optimized */
        .booking-steps {
            padding: var(--space-xl) 20px;
            background: var(--color-dark-card);
        }

        .section-title {
            text-align: center;
            margin-bottom: var(--space-xl);
        }

        .section-title h2 {
            font-size: clamp(1.75rem, 5vw, 2.25rem);
            color: white;
            margin-bottom: var(--space-sm);
            position: relative;
            display: inline-block;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -8px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background: var(--gradient-accent);
            border-radius: 3px;
        }

        .section-title .lead {
            color: var(--color-muted-text);
            font-size: 0.95rem;
            line-height: 1.5;
            max-width: 600px;
            margin: 0 auto;
        }

        .steps-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: var(--space-lg);
            max-width: 1200px;
            margin: 0 auto;
        }

        @media (min-width: 768px) {
            .steps-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        .step-card {
            background: var(--gradient-card);
            padding: var(--space-lg);
            border-radius: var(--radius-xl);
            text-align: center;
            transition: all var(--transition-normal);
            box-shadow: var(--shadow-soft);
            border: 1px solid var(--color-dark-border);
            min-height: 280px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .step-number {
            width: 40px;
            height: 40px;
            background: var(--gradient-accent);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.25rem;
            font-weight: 600;
            margin: 0 auto var(--space-sm);
        }

        .step-icon {
            font-size: 2rem;
            color: var(--color-light-purple);
            margin-bottom: var(--space-sm);
        }

        .step-card h3 {
            color: white;
            margin-bottom: var(--space-sm);
            font-size: 1.25rem;
        }

        .step-card p {
            color: var(--color-muted-text);
            font-size: 0.9rem;
            line-height: 1.5;
        }

        /* Prices Section - Mobile Optimized */
        .prices {
            padding: var(--space-xl) 20px;
            background: var(--color-dark-base);
        }

        .price-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: var(--space-lg);
            max-width: 1200px;
            margin: 0 auto;
        }

        @media (min-width: 768px) {
            .price-grid {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        .price-category {
            background: var(--gradient-card);
            padding: var(--space-lg);
            border-radius: var(--radius-xl);
            box-shadow: var(--shadow-soft);
            border: 1px solid var(--color-dark-border);
        }

        .price-category h3 {
            color: white;
            margin-bottom: var(--space-md);
            padding-bottom: var(--space-sm);
            border-bottom: 2px solid var(--color-dark-border);
            font-size: 1.25rem;
        }

        .price-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.75rem 0;
            border-bottom: 1px solid var(--color-dark-border);
        }

        .price-item:last-child {
            border-bottom: none;
        }

        .price-item span:first-child {
            color: var(--color-dark-text);
            font-size: 0.9rem;
        }

        .price-amount {
            font-weight: 600;
            color: var(--color-light-purple);
            font-size: 1rem;
        }

        /* Policies - Mobile Optimized */
        .policies {
            padding: var(--space-xl) 20px;
            background: var(--color-dark-card);
        }

        .policy-card {
            background: var(--gradient-card);
            padding: var(--space-lg);
            border-radius: var(--radius-xl);
            box-shadow: var(--shadow-soft);
            border: 1px solid var(--color-dark-border);
            max-width: 800px;
            margin: 0 auto;
        }

        .policy-card h3 {
            color: var(--color-light-purple);
            margin-bottom: var(--space-md);
            font-size: 1.25rem;
        }

        /* Gallery Preview - Mobile Optimized */
        .gallery-preview {
            padding: var(--space-xl) 20px;
            background: var(--color-dark-base);
        }

        .gallery-grid-preview {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 15px;
            max-width: 1200px;
            margin: var(--space-lg) auto;
        }

        @media (min-width: 768px) {
            .gallery-grid-preview {
                grid-template-columns: repeat(4, 1fr);
                gap: 20px;
            }
        }

        .gallery-item {
            aspect-ratio: 1;
            border-radius: var(--radius-lg);
            overflow: hidden;
            position: relative;
            background: var(--color-dark-card);
            border: 1px solid var(--color-dark-border);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform var(--transition-slow);
        }

        .gallery-item:hover img {
            transform: scale(1.05);
        }

        /* Contact - Mobile Optimized */
        .contact {
            padding: var(--space-xl) 20px;
            background: var(--color-dark-card);
        }

        .contact-buttons {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: var(--space-sm);
            margin: var(--space-lg) 0;
        }

        @media (min-width: 768px) {
            .contact-buttons {
                flex-direction: row;
                justify-content: center;
                gap: var(--space-md);
            }
        }

        .contact p {
            margin-bottom: var(--space-sm);
            color: var(--color-muted-text);
            font-size: 0.9rem;
            line-height: 1.5;
        }

        .contact p i {
            color: var(--color-light-purple);
            margin-right: 8px;
            width: 16px;
            text-align: center;
        }

        /* Footer - Mobile Optimized */
        footer {
            background: #111111;
            color: var(--color-dark-text);
            padding: var(--space-lg) 20px;
            text-align: center;
        }

        .footer-contact {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: var(--space-md);
            margin-bottom: var(--space-md);
        }

        @media (min-width: 768px) {
            .footer-contact {
                flex-direction: row;
                justify-content: center;
                align-items: center;
                gap: var(--space-xl);
            }
        }

        .social-icons {
            display: flex;
            gap: var(--space-sm);
        }

        .social-icon {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: all var(--transition-normal);
            font-size: 1rem;
        }

        .phone-number {
            display: flex;
            align-items: center;
            gap: var(--space-sm);
            padding: 0.6rem 1.25rem;
            background: rgba(255, 255, 255, 0.1);
            border-radius: var(--radius-round);
            cursor: pointer;
            transition: background var(--transition-normal);
            font-size: 0.9rem;
        }

        /* ============================================
           BOOKING PAGE - MOBILE OPTIMIZED
        ============================================= */
        #booking-page {
            display: none;
            min-height: 100vh;
            background: var(--color-dark-base);
            padding-top: 70px;
        }

        .booking-hero {
            text-align: center;
            padding: var(--space-lg) 20px;
            background: var(--gradient-main);
        }

        .booking-hero h1 {
            color: white;
            margin-bottom: var(--space-sm);
            font-size: clamp(1.75rem, 5vw, 2.5rem);
        }

        .booking-hero p {
            color: var(--color-muted-text);
            font-size: 0.95rem;
            line-height: 1.5;
        }

        .availability-section {
            padding: var(--space-xl) 20px;
            max-width: 1000px;
            margin: 0 auto;
        }

        .availability-card {
            background: var(--gradient-card);
            padding: var(--space-lg);
            border-radius: var(--radius-xl);
            box-shadow: var(--shadow-soft);
            border: 1px solid var(--color-dark-border);
        }

        .availability-image {
            width: 100%;
            max-width: 800px;
            margin: var(--space-lg) auto;
            border-radius: var(--radius-lg);
            overflow: hidden;
            box-shadow: var(--shadow-medium);
            background: var(--color-dark-card);
            border: 1px solid var(--color-dark-border);
        }

        .availability-image img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Booking Form - Mobile Optimized */
        .booking-form-container {
            background: var(--gradient-card);
            padding: var(--space-lg);
            border-radius: var(--radius-xl);
            margin: var(--space-lg) auto;
            max-width: 600px;
            border: 1px solid var(--color-dark-border);
        }

        .booking-form {
            display: flex;
            flex-direction: column;
            gap: var(--space-md);
        }

        .form-group {
            display: flex;
            flex-direction: column;
            gap: 6px;
        }

        .form-group label {
            color: white;
            font-weight: 500;
            font-size: 0.9rem;
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            padding: 12px 16px;
            background: var(--color-dark-base);
            border: 1px solid var(--color-dark-border);
            border-radius: var(--radius-md);
            color: var(--color-dark-text);
            font-family: var(--font-body);
            font-size: 16px;
            transition: all var(--transition-fast);
            width: 100%;
            -webkit-appearance: none;
            appearance: none;
        }

        .form-group select {
            background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='12' fill='%23B19CD9' viewBox='0 0 16 16'%3E%3Cpath d='M7.247 11.14L2.451 5.658C1.885 5.013 2.345 4 3.204 4h9.592a1 1 0 0 1 .753 1.659l-4.796 5.48a1 1 0 0 1-1.506 0z'/%3E%3C/svg%3E");
            background-repeat: no-repeat;
            background-position: right 16px center;
            background-size: 12px;
            padding-right: 40px;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--color-light-purple);
            box-shadow: 0 0 0 2px rgba(177, 156, 217, 0.2);
        }

        .form-group input::placeholder,
        .form-group textarea::placeholder {
            color: var(--color-muted-text);
            opacity: 0.8;
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr;
            gap: var(--space-md);
        }

        @media (min-width: 768px) {
            .form-row {
                grid-template-columns: 1fr 1fr;
            }
        }

        .form-submit {
            padding: 14px 28px;
            background: var(--gradient-accent);
            color: white;
            border: none;
            border-radius: var(--radius-round);
            font-weight: 500;
            cursor: pointer;
            transition: all var(--transition-normal);
            font-size: 1rem;
            margin-top: var(--space-sm);
            min-height: 48px;
        }

        /* Success Message - Mobile Optimized */
        .success-message {
            background: linear-gradient(135deg, rgba(46, 204, 113, 0.1), rgba(39, 174, 96, 0.1));
            border: 1px solid rgba(46, 204, 113, 0.3);
            border-radius: var(--radius-lg);
            padding: var(--space-lg);
            text-align: center;
            display: none;
        }

        .success-icon {
            font-size: 2.5rem;
            color: #2ecc71;
            margin-bottom: var(--space-md);
        }

        .success-message h3 {
            color: white;
            margin-bottom: var(--space-sm);
            font-size: 1.25rem;
        }

        .success-message p {
            color: var(--color-muted-text);
            margin-bottom: var(--space-sm);
            font-size: 0.9rem;
            line-height: 1.5;
        }

        /* Time Slots - Mobile Optimized */
        .time-slots {
            display: grid;
            grid-template-columns: 1fr;
            gap: var(--space-sm);
            margin-top: var(--space-lg);
        }

        @media (min-width: 768px) {
            .time-slots {
                grid-template-columns: repeat(3, 1fr);
                gap: var(--space-md);
            }
        }

        .time-slot {
            background: var(--gradient-card);
            padding: var(--space-md);
            border-radius: var(--radius-lg);
            text-align: center;
            border: 1px solid var(--color-dark-border);
            min-height: 120px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .time-slot h4 {
            color: white;
            margin-bottom: var(--space-sm);
            font-size: 1rem;
        }

        .time-slot p {
            color: var(--color-muted-text);
            margin: 4px 0;
            font-size: 0.85rem;
        }

        /* ============================================
           GALLERY PAGE - MOBILE OPTIMIZED
        ============================================= */
        #gallery-page {
            display: none;
            min-height: 100vh;
            background: var(--color-dark-base);
            padding-top: 70px;
        }

        .gallery-full {
            padding: var(--space-lg) 20px;
        }

        .gallery-grid-full {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 12px;
            max-width: 1400px;
            margin: 0 auto;
        }

        @media (min-width: 768px) {
            .gallery-grid-full {
                grid-template-columns: repeat(3, 1fr);
                gap: 16px;
            }
        }

        @media (min-width: 1024px) {
            .gallery-grid-full {
                grid-template-columns: repeat(4, 1fr);
                gap: 20px;
            }
        }

        /* ============================================
           LIGHTBOX - MOBILE OPTIMIZED
        ============================================= */
        .lightbox {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.95);
            z-index: 2000;
            display: none;
            align-items: center;
            justify-content: center;
            padding: 20px;
            touch-action: pan-y pinch-zoom;
        }

        .lightbox-content {
            max-width: 95%;
            max-height: 85%;
            position: relative;
        }

        .lightbox-img {
            width: 100%;
            height: auto;
            border-radius: var(--radius-lg);
            box-shadow: 0 10px 50px rgba(0, 0, 0, 0.5);
            -webkit-user-drag: none;
            user-select: none;
        }

        .lightbox-close {
            position: absolute;
            top: -45px;
            right: 0;
            background: none;
            border: none;
            color: white;
            font-size: 1.75rem;
            cursor: pointer;
            z-index: 2001;
            padding: 8px;
        }

        /* ============================================
           BUTTON STYLES - MOBILE OPTIMIZED
        ============================================= */
        .btn {
            padding: 12px 24px;
            background: var(--gradient-accent);
            color: white;
            border: none;
            border-radius: var(--radius-round);
            font-weight: 500;
            cursor: pointer;
            text-decoration: none;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 8px;
            transition: all var(--transition-normal);
            font-size: 0.95rem;
            min-height: 44px;
            min-width: 140px;
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-medium);
        }

        .btn-secondary {
            background: transparent;
            color: var(--color-dark-text);
            border: 2px solid var(--color-light-purple);
        }

        /* ============================================
           MOBILE-SPECIFIC STYLES
        ============================================= */
        @media (max-width: 767px) {
            /* Header Mobile */
            .mobile-menu-btn {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 70px;
                left: 0;
                right: 0;
                background: var(--color-dark-card);
                flex-direction: column;
                padding: var(--space-md);
                gap: 0;
                transform: translateY(-100%);
                opacity: 0;
                visibility: hidden;
                transition: all var(--transition-normal);
                box-shadow: var(--shadow-float);
                border-radius: 0 0 var(--radius-lg) var(--radius-lg);
                border: 1px solid var(--color-dark-border);
                border-top: none;
                z-index: 999;
            }
            
            .nav-links.active {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }
            
            .nav-links a {
                padding: 14px 16px;
                width: 100%;
                text-align: center;
                border-bottom: 1px solid var(--color-dark-border);
                font-size: 1rem;
            }
            
            .nav-links a:last-child {
                border-bottom: none;
            }
            
            .btn-nav {
                width: 100%;
                margin-top: 8px;
                padding: 12px;
            }
            
            /* Hero Mobile */
            .hero {
                min-height: 80vh;
                padding: 0 16px;
            }
            
            .hero-content {
                padding: 1.5rem 0;
            }
            
            .btn-hero {
                width: 100%;
                max-width: 280px;
            }
            
            /* Sections Mobile */
            .booking-steps,
            .prices,
            .policies,
            .gallery-preview,
            .contact {
                padding: var(--space-lg) 16px;
            }
            
            .step-card {
                padding: var(--space-md);
                min-height: 240px;
            }
            
            .price-category,
            .policy-card {
                padding: var(--space-md);
            }
            
            /* Gallery Mobile */
            .gallery-grid-preview,
            .gallery-grid-full {
                gap: 10px;
            }
            
            /* Form Mobile */
            .booking-form-container {
                padding: var(--space-md);
            }
            
            .form-group input,
            .form-group select,
            .form-group textarea {
                padding: 14px 16px;
                font-size: 16px;
            }
            
            /* Footer Mobile */
            footer {
                padding: var(--space-md) 16px;
            }
            
            footer p {
                font-size: 0.85rem;
                line-height: 1.4;
            }
            
            /* Lightbox Mobile */
            .lightbox-close {
                top: -40px;
                font-size: 1.5rem;
            }
            
            /* Prevent horizontal scroll */
            body {
                overflow-x: hidden;
                width: 100%;
            }
            
            .page,
            section {
                width: 100%;
                overflow-x: hidden;
            }
            
            /* Touch-friendly scrolling */
            * {
                -webkit-overflow-scrolling: touch;
            }
        }

        /* Tablet Styles */
        @media (min-width: 768px) and (max-width: 1024px) {
            .gallery-grid-full {
                grid-template-columns: repeat(3, 1fr);
            }
            
            .steps-grid {
                gap: var(--space-md);
            }
            
            .step-card {
                padding: var(--space-md);
            }
        }

        /* ============================================
           ANIMATIONS
        ============================================= */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease, transform 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Loading Animation */
        .loading {
            animation: pulse 1.5s infinite;
        }

        @keyframes pulse {
            0% { opacity: 0.6; }
            50% { opacity: 1; }
            100% { opacity: 0.6; }
        }

        /* ============================================
           SAFARI/IOS SPECIFIC FIXES
        ============================================= */
        @supports (-webkit-touch-callout: none) {
            .hero {
                min-height: -webkit-fill-available;
                min-height: 85vh;
            }
            
            .page {
                min-height: -webkit-fill-available;
                min-height: 100vh;
            }
            
            .btn,
            .btn-nav,
            .btn-hero,
            .form-submit {
                -webkit-appearance: none;
                border-radius: var(--radius-round);
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="nav-container">
            <a href="#" onclick="showPage('home')" class="logo">Sets by Kiara</a>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn" aria-label="Toggle menu">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav class="nav-links" id="navLinks">
                <a href="#" onclick="showPage('home')" class="active">Home</a>
                <a href="#" onclick="showPage('gallery')">Gallery</a>
                <a href="#" onclick="showPage('booking')" class="btn-nav">Book Now</a>
            </nav>
        </div>
    </header>

    <!-- ============================================
        HOME PAGE
    ============================================= -->
    <div id="home-page" class="page">
        <!-- Hero -->
        <section class="hero">
            <img src="https://dl.dropboxusercontent.com/scl/fi/un71809vyxmjr3mssxb5w/resized-banner.jpg?rlkey=1sf82a7hp6akdjhovzc7ksijb&st=6ovmm1nu&raw=1" 
                 alt="Luxury nail set by Kiara" 
                 class="hero-background"
                 onerror="handleImageError(this)">
            
            <div class="hero-content">
                <h1>Sets by Kiara</h1>
                <p class="hero-tagline">Luxury nail sets • Home-based • Midland, TX</p>
                <a href="#" onclick="showPage('booking')" class="btn-hero">
                    <i class="fas fa-calendar-check"></i>
                    Book Your Appointment
                </a>
            </div>
        </section>

        <!-- Booking Steps -->
        <section class="booking-steps">
            <div class="section-title">
                <h2>How to Book</h2>
                <p class="lead">Simple steps to schedule your luxury nail appointment</p>
            </div>
            
            <div class="steps-grid">
                <div class="step-card fade-in">
                    <div class="step-number">1</div>
                    <div class="step-icon">
                        <i class="fas fa-calendar-alt"></i>
                    </div>
                    <h3>Check Availability</h3>
                    <p>View current availability on the booking page</p>
                </div>
                
                <div class="step-card fade-in">
                    <div class="step-number">2</div>
                    <div class="step-icon">
                        <i class="fas fa-comment-dots"></i>
                    </div>
                    <h3>Book Online</h3>
                    <p>Fill out our easy booking form with your preferences</p>
                </div>
                
                <div class="step-card fade-in">
                    <div class="step-number">3</div>
                    <div class="step-icon">
                        <i class="fas fa-money-bill-wave"></i>
                    </div>
                    <h3>Secure Deposit</h3>
                    <p>$10 deposit via Venmo, Zelle, or Apple Pay</p>
                </div>
            </div>
        </section>

        <!-- Prices -->
        <section class="prices">
            <div class="section-title">
                <h2>Price List</h2>
                <p class="lead">Transparent pricing for luxury nail services</p>
            </div>
            
            <div class="price-grid">
                <div class="price-category fade-in">
                    <h3>Base Price (Before Design)</h3>
                    <div class="price-item">
                        <span>SHORT</span>
                        <span class="price-amount">$40-$50</span>
                    </div>
                    <div class="price-item">
                        <span>MEDIUM</span>
                        <span class="price-amount">$60</span>
                    </div>
                    <div class="price-item">
                        <span>MEDIUM LONG</span>
                        <span class="price-amount">$70</span>
                    </div>
                    <div class="price-item">
                        <span>LONG</span>
                        <span class="price-amount">$90</span>
                    </div>
                    <div class="price-item">
                        <span>XXL</span>
                        <span class="price-amount">$100</span>
                    </div>
                    <div class="price-item">
                        <span>XXXL</span>
                        <span class="price-amount">$110</span>
                    </div>
                </div>
                
                <div class="price-category fade-in">
                    <h3>Fill Base Price</h3>
                    <div class="price-item">
                        <span>2 WEEK FILL</span>
                        <span class="price-amount">$50</span>
                    </div>
                    <div class="price-item">
                        <span>4 WEEK FILL</span>
                        <span class="price-amount">$60</span>
                    </div>
                </div>
                
                <div class="price-category fade-in">
                    <h3>Design Add-Ons</h3>
                    <div style="margin-top: var(--space-sm);">
                        <h4 style="color: var(--color-light-purple); margin-bottom: 8px; font-size: 0.95rem;">TIER 1 (Easy Designs)</h4>
                        <span class="price-amount">$15-$20</span>
                        <ul style="list-style: none; margin-top: 8px; color: var(--color-muted-text); font-size: 0.85rem; line-height: 1.4;">
                            <li>• French Tip</li>
                            <li>• Solid Color</li>
                            <li>• Cat Eye</li>
                            <li>• Minimal Design</li>
                            <li>• 1 Color Airbrush</li>
                        </ul>
                    </div>
                    
                    <div style="margin-top: var(--space-md);">
                        <h4 style="color: var(--color-light-purple); margin-bottom: 8px; font-size: 0.95rem;">TIER 2 (Full Design)</h4>
                        <span class="price-amount">$25-$45</span>
                        <ul style="list-style: none; margin-top: 8px; color: var(--color-muted-text); font-size: 0.85rem; line-height: 1.4;">
                            <li>• Multi Color Airbrush</li>
                            <li>• Multi Design</li>
                            <li>• 3D Art</li>
                            <li>• Charms, etc.</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Policies -->
        <section class="policies">
            <div class="section-title">
                <h2>Booking Policies</h2>
                <p class="lead">Important information for your appointment</p>
            </div>
            
            <div class="policy-card fade-in">
                <h3>Deposit & Booking</h3>
                <ul style="list-style: none; color: var(--color-muted-text); font-size: 0.9rem; line-height: 1.5;">
                    <li style="margin-bottom: 10px; padding-left: 1.5rem; position: relative;">
                        <span style="position: absolute; left: 0; color: var(--color-light-pink);">✓</span>
                        $10 deposit required to secure all appointments
                    </li>
                    <li style="margin-bottom: 10px; padding-left: 1.5rem; position: relative;">
                        <span style="position: absolute; left: 0; color: var(--color-light-pink);">✓</span>
                        Deposit is non-refundable but applies to your total
                    </li>
                    <li style="margin-bottom: 10px; padding-left: 1.5rem; position: relative;">
                        <span style="position: absolute; left: 0; color: var(--color-light-pink);">✓</span>
                        No deposit = appointment not confirmed
                    </li>
                    <li style="margin-bottom: 10px; padding-left: 1.5rem; position: relative;">
                        <span style="position: absolute; left: 0; color: var(--color-light-pink);">✓</span>
                        24-hour notice required for changes
                    </li>
                    <li style="padding-left: 1.5rem; position: relative;">
                        <span style="position: absolute; left: 0; color: var(--color-light-pink);">✓</span>
                        Late arrivals may require rescheduling
                    </li>
                </ul>
            </div>
        </section>

        <!-- Gallery Preview -->
        <section class="gallery-preview">
            <div class="section-title">
                <h2>Recent Work</h2>
                <p class="lead">A preview of luxury nail sets</p>
            </div>
            
            <div class="gallery-grid-preview">
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/ebaj5n1j50hu0smf1hsin/Photo-Jan-21-2026-10-42-23-AM-15.jpg?rlkey=j2q337degip3jev52zakxx55g&st=ox8noiy1&raw=1" 
                         alt="Floral nail design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/kp3nrtx6dbswmpitj770p/Photo-Jan-21-2026-10-42-23-AM-12.jpg?rlkey=wua1w2sr7w8w1mf0jcngk6nyg&st=zz2vqqtf&raw=1" 
                         alt="French tip nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/w2rmng78m168pnwq3grd9/Photo-Jan-21-2026-10-42-23-AM-11.jpg?rlkey=rhmduunfalpb919o1w7nopubg&st=rhi1vibh&raw=1" 
                         alt="Matte black design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/hdjediya433sl60hfkgqe/Photo-Jan-21-2026-10-42-23-AM-10.jpg?rlkey=0li9ffnolzycm0iu9ngfnk3jc&st=tgybly5n&raw=1" 
                         alt="Pink ombré nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
            </div>
            
            <div style="text-align: center; margin-top: var(--space-lg);">
                <a href="#" onclick="showPage('gallery')" class="btn">
                    View Full Gallery
                    <i class="fas fa-arrow-right"></i>
                </a>
            </div>
        </section>

        <!-- Contact -->
        <section class="contact">
            <div class="section-title">
                <h2>Ready to Book?</h2>
                <p class="lead">Connect with me to schedule your appointment</p>
            </div>
            
            <div class="contact-buttons">
                <a href="#" onclick="showPage('booking')" class="btn">
                    <i class="fas fa-calendar-alt"></i>
                    Book Appointment
                </a>
                <a href="https://instagram.com/setsbykiara" target="_blank" class="btn btn-secondary">
                    <i class="fab fa-instagram"></i>
                    Instagram DM
                </a>
            </div>
            
            <div style="text-align: center; margin-top: var(--space-lg); font-size: 0.9rem;">
                <p><i class="fas fa-map-marker-alt"></i> Midland, Texas • Home-based Studio</p>
                <p><i class="fas fa-phone"></i> Phone: 432-425-3341</p>
                <p><i class="fas fa-money-bill-wave"></i> Venmo: @Chelsea-Byrd-8</p>
                <p><i class="fas fa-mobile-alt"></i> Zelle & Apple Pay: 432-425-3341</p>
            </div>
        </section>
    </div>

    <!-- ============================================
        BOOKING PAGE
    ============================================= -->
    <div id="booking-page" class="page">
        <section class="booking-hero">
            <div class="container">
                <h1>Book Your Appointment</h1>
                <p>Check availability and book your luxury nail appointment online</p>
            </div>
        </section>

        <section class="availability-section">
            <div class="availability-card">
                <div class="section-title">
                    <h2>Current Availability</h2>
                    <p>Available times for February appointments</p>
                </div>
                
                <!-- Calendar Image -->
                <div class="availability-image">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/ivqhcgyywdvh1ogkksv4k/Photo-Jan-21-2026-11-28-07-AM.jpg?rlkey=c1c7lpr5a5zo75vkkrn80zcd9&st=sqeqdqp6&raw=1" 
                         alt="February Availability Calendar"
                         onerror="handleImageError(this)">
                </div>
                
                <!-- Booking Form -->
                <div class="booking-form-container fade-in">
                    <h3 style="color: white; margin-bottom: var(--space-md); text-align: center;">Book Your Appointment</h3>
                    
                    <div class="success-message" id="successMessage">
                        <div class="success-icon">
                            <i class="fas fa-check-circle"></i>
                        </div>
                        <h3>Booking Request Submitted!</h3>
                        <p>Thank you for your booking request. Kiara will contact you within 24 hours to confirm your appointment.</p>
                        <p><strong>Next Steps:</strong></p>
                        <p>1. Check your email for confirmation</p>
                        <p>2. Send $10 deposit to secure your spot</p>
                        <p>3. Receive studio address details</p>
                        <button onclick="resetForm()" class="btn" style="margin-top: var(--space-md);">
                            <i class="fas fa-plus"></i>
                            Book Another Appointment
                        </button>
                    </div>
                    
                    <form class="booking-form" id="bookingForm" onsubmit="submitBooking(event)">
                        <div class="form-row">
                            <div class="form-group">
                                <label for="firstName">First Name *</label>
                                <input type="text" id="firstName" name="firstName" required placeholder="Your first name">
                            </div>
                            <div class="form-group">
                                <label for="lastName">Last Name *</label>
                                <input type="text" id="lastName" name="lastName" required placeholder="Your last name">
                            </div>
                        </div>
                        
                        <div class="form-row">
                            <div class="form-group">
                                <label for="phone">Phone Number *</label>
                                <input type="tel" id="phone" name="phone" required placeholder="432-425-3341">
                            </div>
                            <div class="form-group">
                                <label for="email">Email Address *</label>
                                <input type="email" id="email" name="email" required placeholder="your@email.com">
                            </div>
                        </div>
                        
                        <div class="form-row">
                            <div class="form-group">
                                <label for="date">Preferred Date *</label>
                                <select id="date" name="date" required>
                                    <option value="">Select a date</option>
                                    <option value="feb-2">Monday, February 2</option>
                                    <option value="feb-3">Tuesday, February 3</option>
                                    <option value="feb-4">Wednesday, February 4</option>
                                    <option value="feb-5">Thursday, February 5</option>
                                    <option value="feb-6">Friday, February 6</option>
                                    <option value="feb-9">Monday, February 9</option>
                                    <option value="feb-10">Tuesday, February 10</option>
                                    <option value="feb-11">Wednesday, February 11</option>
                                    <option value="feb-12">Thursday, February 12</option>
                                    <option value="feb-13">Friday, February 13</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="time">Preferred Time *</label>
                                <select id="time" name="time" required>
                                    <option value="">Select a time</option>
                                    <option value="10am">10:00 AM</option>
                                    <option value="12pm">12:00 PM</option>
                                    <option value="5pm">5:00 PM</option>
                                </select>
                            </div>
                        </div>
                        
                        <div class="form-row">
                            <div class="form-group">
                                <label for="nailLength">Nail Length *</label>
                                <select id="nailLength" name="nailLength" required>
                                    <option value="">Select length</option>
                                    <option value="short">Short ($40-50)</option>
                                    <option value="medium">Medium ($60)</option>
                                    <option value="medium-long">Medium Long ($70)</option>
                                    <option value="long">Long ($90)</option>
                                    <option value="xxl">XXL ($100)</option>
                                    <option value="xxxl">XXXL ($110)</option>
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="designTier">Design Tier *</label>
                                <select id="designTier" name="designTier" required>
                                    <option value="">Select design tier</option>
                                    <option value="tier1">Tier 1: Simple Designs ($15-20)</option>
                                    <option value="tier2">Tier 2: Full Design ($25-45)</option>
                                    <option value="none">No Design</option>
                                </select>
                            </div>
                        </div>
                        
                        <div class="form-group">
                            <label for="designDetails">Design Details (Optional)</label>
                            <textarea id="designDetails" name="designDetails" rows="2" placeholder="Describe your design ideas..."></textarea>
                        </div>
                        
                        <div class="form-group">
                            <label for="specialRequests">Special Requests</label>
                            <textarea id="specialRequests" name="specialRequests" rows="2" placeholder="Any allergies or special requests..."></textarea>
                        </div>
                        
                        <div class="form-group" style="margin-top: var(--space-sm);">
                            <label style="display: flex; align-items: flex-start; gap: 8px; cursor: pointer; font-size: 0.85rem;">
                                <input type="checkbox" required style="margin-top: 3px; min-width: 16px;">
                                <span style="color: var(--color-muted-text);">
                                    I understand that a $10 deposit is required to secure my appointment and is non-refundable but will be applied to my total.
                                </span>
                            </label>
                        </div>
                        
                        <button type="submit" class="form-submit" id="submitBtn">
                            <i class="fas fa-paper-plane"></i>
                            Submit Booking Request
                        </button>
                    </form>
                </div>
                
                <div style="text-align: center; margin-top: var(--space-lg);">
                    <h3 style="color: var(--color-light-purple); margin-bottom: var(--space-md); font-size: 1.25rem;">Important Notes</h3>
                    
                    <div class="time-slots">
                        <div class="time-slot">
                            <h4>Deposit Information</h4>
                            <p>• $10 deposit required</p>
                            <p>• Venmo: @Chelsea-Byrd-8</p>
                            <p>• Zelle: 432-425-3341</p>
                        </div>
                        
                        <div class="time-slot">
                            <h4>Cancellation Policy</h4>
                            <p>• 24-hour notice</p>
                            <p>• Deposit non-refundable</p>
                            <p>• Applies to reschedules</p>
                        </div>
                        
                        <div class="time-slot">
                            <h4>Studio Information</h4>
                            <p>• Home-based studio</p>
                            <p>• Midland, Texas</p>
                            <p>• Address provided after booking</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <!-- ============================================
        GALLERY PAGE
    ============================================= -->
    <div id="gallery-page" class="page">
        <section class="booking-hero">
            <div class="container">
                <h1>Nail Art Gallery</h1>
                <p>Browse through a collection of luxury nail sets and custom designs</p>
            </div>
        </section>

        <section class="gallery-full">
            <div class="gallery-grid-full">
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/ebaj5n1j50hu0smf1hsin/Photo-Jan-21-2026-10-42-23-AM-15.jpg?rlkey=j2q337degip3jev52zakxx55g&st=ox8noiy1&raw=1" 
                         alt="Floral nail design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/8joe35pazes35rqlhv09c/Photo-Jan-21-2026-10-42-23-AM-14.jpg?rlkey=jnnk006znqoitusgdjrnwu2r3&st=dnli3ve9&raw=1" 
                         alt="Nail design 14" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/8joe35pazes35rqlhv09c/Photo-Jan-21-2026-10-42-23-AM-14.jpg?rlkey=jnnk006znqoitusgdjrnwu2r3&st=pevzufi9&raw=1" 
                         alt="Nail design 14b" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/kp3nrtx6dbswmpitj770p/Photo-Jan-21-2026-10-42-23-AM-12.jpg?rlkey=wua1w2sr7w8w1mf0jcngk6nyg&st=zz2vqqtf&raw=1" 
                         alt="French tip nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/w2rmng78m168pnwq3grd9/Photo-Jan-21-2026-10-42-23-AM-11.jpg?rlkey=rhmduunfalpb919o1w7nopubg&st=rhi1vibh&raw=1" 
                         alt="Matte black design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/hdjediya433sl60hfkgqe/Photo-Jan-21-2026-10-42-23-AM-10.jpg?rlkey=0li9ffnolzycm0iu9ngfnk3jc&st=tgybly5n&raw=1" 
                         alt="Pink ombré nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/ki2z4khg85grol1y8hs7o/Photo-Jan-21-2026-10-42-23-AM-9.jpg?rlkey=fr56oj0e3m35h6o5au1bo9iqu&st=v4290aop&raw=1" 
                         alt="Colorful abstract design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/0m68mwbqc1kivlrre3zbf/Photo-Jan-21-2026-10-42-23-AM-8.jpg?rlkey=0a8s2p4clps0n93ukj4n9bgm9&st=c4sj38pr&raw=1" 
                         alt="Burgundy luxury nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/cnsu1ucrxqnmvn34hwjzo/Photo-Jan-21-2026-10-42-23-AM-7.jpg?rlkey=20y73gvfoacg25bwor3l7flu2&st=enu6bs69&raw=1" 
                         alt="Minimalist nude nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/b6tkurhrwynez1z2sklsi/Photo-Jan-21-2026-10-42-23-AM-6.jpg?rlkey=9mog2c8gjt53wdlex3w4mho56&st=zxkxyll6&raw=1" 
                         alt="Marble effect nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/qo45lb7xlc10lbtcpvas0/Photo-Jan-21-2026-10-42-23-AM-5.jpg?rlkey=1rgk87k7ljpbf5v4gvcoo2j8x&st=gph4ozau&raw=1" 
                         alt="Glitter gradient nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/1z0csj4xk8vabye7hwhql/Photo-Jan-21-2026-10-42-23-AM-4-1.jpg?rlkey=2u1qkj2csi14ut6ihtt9v7p0g&st=ksshipm0&raw=1" 
                         alt="Colorful French tips" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/gpnsr62fh1s5jblkjm5le/Photo-Jan-21-2026-10-42-23-AM-4.jpg?rlkey=kzewzsnetlnyifffu3xqaixwb&st=43jtajea&raw=1" 
                         alt="Lavender chrome nails" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/6i9dzh70e9quymbcvvfh3/Photo-Jan-21-2026-10-42-23-AM-3.jpg?rlkey=cb8s28mvj86jwnsr5imw90ho8&st=a5c8ca18&raw=1" 
                         alt="Animal print design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/nifl5jjgbrdd195sh8sdj/Photo-Jan-21-2026-10-42-23-AM-2-1.jpg?rlkey=loztdzu0j4nrsalfjvburmkwm&st=ajzs9i4w&raw=1" 
                         alt="Nail design 2-1" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/lnwfb1yhhd9znh34zmdga/Photo-Jan-21-2026-10-42-23-AM-1.jpg?rlkey=o9uvn7s90zmm26d91hp74tsto&st=t5i36okl&raw=1" 
                         alt="Nail design 1" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
                <div class="gallery-item">
                    <img src="https://dl.dropboxusercontent.com/scl/fi/4rt2h8k12g77k89bu8rf9/Photo-Jan-21-2026-10-42-23-AM.jpg?rlkey=mkf12zh0bpjft2h1mj71nj2do&st=wy8aljes&raw=1" 
                         alt="Nail design" 
                         onclick="openLightbox(this.src)"
                         onerror="handleImageError(this)">
                </div>
            </div>
            
            <div style="text-align: center; margin-top: var(--space-lg);">
                <a href="#" onclick="showPage('home')" class="btn">
                    <i class="fas fa-arrow-left"></i>
                    Back to Home
                </a>
            </div>
        </section>
    </div>

    <!-- ============================================
        LIGHTBOX
    ============================================= -->
    <div class="lightbox" id="lightbox" onclick="if(event.target===this) closeLightbox()">
        <button class="lightbox-close" onclick="closeLightbox()" aria-label="Close lightbox">
            <i class="fas fa-times"></i>
        </button>
        <div class="lightbox-content">
            <img id="lightbox-img" class="lightbox-img" src="" alt="">
        </div>
    </div>

    <!-- ============================================
        FOOTER
    ============================================= -->
    <footer>
        <div class="footer-contact">
            <div class="social-icons">
                <a href="https://instagram.com/setsbykiara" target="_blank" class="social-icon" aria-label="Instagram">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://tiktok.com/@kikikuromi" target="_blank" class="social-icon" aria-label="TikTok">
                    <i class="fab fa-tiktok"></i>
                </a>
            </div>
            
            <div class="phone-number" onclick="copyPhoneNumber()" title="Click to copy">
                <i class="fas fa-phone"></i>
                <span>432-425-3341</span>
            </div>
        </div>
        
        <p style="opacity: 0.8; margin-top: var(--space-md); font-size: 0.9rem;">© <span id="currentYear"></span> Sets by Kiara. All rights reserved.</p>
        <p style="opacity: 0.8; font-size: 0.85rem;">Luxury nail artist • Midland, Texas • Home-based studio</p>
    </footer>

    <script>
        // ============================================
        // MOBILE-OPTIMIZED JAVASCRIPT
        // ============================================
        let currentPage = 'home';
        let isMobile = window.innerWidth <= 767;
        
        // ============================================
        // DETECT MOBILE
        // ============================================
        function checkMobile() {
            isMobile = window.innerWidth <= 767;
            // Update touch-friendly classes
            document.body.classList.toggle('mobile-view', isMobile);
        }
        
        // ============================================
        // IMAGE ERROR HANDLER
        // ============================================
        function handleImageError(img) {
            img.onerror = null;
            img.classList.add('img-placeholder');
            img.style.display = 'flex';
            img.style.alignItems = 'center';
            img.style.justifyContent = 'center';
            img.style.color = 'var(--color-light-purple)';
            img.style.fontWeight = '500';
            img.style.padding = '1rem';
            img.style.fontSize = isMobile ? '0.9rem' : '1rem';
            
            if (img.classList.contains('hero-background')) {
                img.innerHTML = 'Sets by Kiara';
            } else if (img.parentElement.classList.contains('gallery-item')) {
                img.innerHTML = 'Nail Design';
            } else {
                img.innerHTML = 'Image';
            }
        }
        
        // ============================================
        // PAGE NAVIGATION - TOUCH OPTIMIZED
        // ============================================
        function showPage(page) {
            // Hide all pages
            document.getElementById('home-page').style.display = 'none';
            document.getElementById('booking-page').style.display = 'none';
            document.getElementById('gallery-page').style.display = 'none';
            
            // Show selected page
            const pageElement = document.getElementById(page + '-page');
            if (pageElement) {
                pageElement.style.display = 'block';
            }
            
            currentPage = page;
            
            // Update active nav link
            document.querySelectorAll('.nav-links a').forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('onclick') && link.getAttribute('onclick').includes(page)) {
                    link.classList.add('active');
                }
            });
            
            // Scroll to top
            window.scrollTo({ top: 0, behavior: 'smooth' });
            
            // Close mobile menu
            closeMobileMenu();
            
            // Trigger animations
            setTimeout(triggerAnimations, 100);
            
            // Initialize form when booking page loads
            if (page === 'booking') {
                setTimeout(() => {
                    const form = document.getElementById('bookingForm');
                    const success = document.getElementById('successMessage');
                    if (form) form.style.display = 'flex';
                    if (success) success.classList.remove('active');
                }, 100);
            }
            
            // Fix image loading on mobile
            if (page === 'gallery') {
                setTimeout(preloadGalleryImages, 300);
            }
        }
        
        // ============================================
        // PRELOAD GALLERY IMAGES FOR MOBILE
        // ============================================
        function preloadGalleryImages() {
            if (!isMobile) return;
            
            const images = document.querySelectorAll('.gallery-item img');
            images.forEach((img, index) => {
                // Lazy load with delay for mobile performance
                setTimeout(() => {
                    if (img.src && !img.complete) {
                        img.loading = 'lazy';
                        // Force load with cache busting
                        const src = img.src.split('?')[0];
                        img.src = src + '?mobile=' + Date.now() + index;
                    }
                }, index * 100); // Stagger loading
            });
        }
        
        // ============================================
        // MOBILE MENU - TOUCH FRIENDLY
        // ============================================
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        if (mobileMenuBtn) {
            mobileMenuBtn.addEventListener('click', toggleMobileMenu);
            mobileMenuBtn.addEventListener('touchstart', function(e) {
                e.preventDefault();
                toggleMobileMenu();
            });
        }
        
        function toggleMobileMenu() {
            const navLinks = document.getElementById('navLinks');
            const icon = mobileMenuBtn.querySelector('i');
            
            navLinks.classList.toggle('active');
            icon.className = navLinks.classList.contains('active') ? 'fas fa-times' : 'fas fa-bars';
            
            // Prevent body scroll when menu is open
            document.body.style.overflow = navLinks.classList.contains('active') ? 'hidden' : '';
        }
        
        function closeMobileMenu() {
            const navLinks = document.getElementById('navLinks');
            const icon = mobileMenuBtn?.querySelector('i');
            
            if (navLinks) navLinks.classList.remove('active');
            if (icon) icon.className = 'fas fa-bars';
            document.body.style.overflow = '';
        }
        
        // Close menu when clicking outside on mobile
        document.addEventListener('click', function(e) {
            if (isMobile && !e.target.closest('.nav-container')) {
                closeMobileMenu();
            }
        });
        
        // ============================================
        // BOOKING FORM - MOBILE OPTIMIZED
        // ============================================
        function submitBooking(event) {
            event.preventDefault();
            
            if (!isMobile) {
                // Desktop submission
                submitBookingDesktop(event);
            } else {
                // Mobile submission with touch feedback
                submitBookingMobile(event);
            }
        }
        
        function submitBookingDesktop(event) {
            event.preventDefault();
            
            const submitBtn = document.getElementById('submitBtn');
            const form = document.getElementById('bookingForm');
            const successMessage = document.getElementById('successMessage');
            
            // Get form data
            const formData = {
                firstName: document.getElementById('firstName').value,
                lastName: document.getElementById('lastName').value,
                phone: document.getElementById('phone').value,
                email: document.getElementById('email').value,
                date: document.getElementById('date').value,
                time: document.getElementById('time').value,
                nailLength: document.getElementById('nailLength').value,
                designTier: document.getElementById('designTier').value,
                designDetails: document.getElementById('designDetails').value,
                specialRequests: document.getElementById('specialRequests').value,
                timestamp: new Date().toISOString()
            };
            
            // Validate
            if (!formData.firstName || !formData.lastName || !formData.phone || !formData.email || 
                !formData.date || !formData.time || !formData.nailLength || !formData.designTier) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Disable submit button
            submitBtn.disabled = true;
            submitBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Processing...';
            
            // Simulate form submission
            setTimeout(() => {
                // Store booking
                const bookings = JSON.parse(localStorage.getItem('setsbykiara_bookings') || '[]');
                bookings.push(formData);
                localStorage.setItem('setsbykiara_bookings', JSON.stringify(bookings));
                
                // Show success
                if (form) form.style.display = 'none';
                if (successMessage) successMessage.classList.add('active');
                
                // Send notification
                sendBookingEmail(formData);
                
                // Reset button
                submitBtn.disabled = false;
                submitBtn.innerHTML = '<i class="fas fa-paper-plane"></i> Submit Booking Request';
            }, 1500);
        }
        
        function submitBookingMobile(event) {
            event.preventDefault();
            
            const submitBtn = document.getElementById('submitBtn');
            const form = document.getElementById('bookingForm');
            const successMessage = document.getElementById('successMessage');
            
            // Get form data
            const formData = {
                firstName: document.getElementById('firstName').value,
                lastName: document.getElementById('lastName').value,
                phone: document.getElementById('phone').value,
                email: document.getElementById('email').value,
                date: document.getElementById('date').value,
                time: document.getElementById('time').value,
                nailLength: document.getElementById('nailLength').value,
                designTier: document.getElementById('designTier').value,
                designDetails: document.getElementById('designDetails').value,
                specialRequests: document.getElementById('specialRequests').value,
                timestamp: new Date().toISOString()
            };
            
            // Validate with mobile-friendly alerts
            let isValid = true;
            let errorMessage = '';
            
            if (!formData.firstName) errorMessage = 'First name is required';
            else if (!formData.lastName) errorMessage = 'Last name is required';
            else if (!formData.phone) errorMessage = 'Phone number is required';
            else if (!formData.email) errorMessage = 'Email is required';
            else if (!formData.date) errorMessage = 'Please select a date';
            else if (!formData.time) errorMessage = 'Please select a time';
            else if (!formData.nailLength) errorMessage = 'Please select nail length';
            else if (!formData.designTier) errorMessage = 'Please select design tier';
            
            if (errorMessage) {
                // Mobile-friendly alert
                alert(errorMessage);
                // Scroll to first error
                document.querySelector('.booking-form-container').scrollIntoView({ 
                    behavior: 'smooth',
                    block: 'center'
                });
                return;
            }
            
            // Add touch feedback
            submitBtn.classList.add('loading');
            submitBtn.disabled = true;
            submitBtn.innerHTML = '<i class="fas fa-spinner fa-spin"></i> Sending...';
            
            // Simulate network delay
            setTimeout(() => {
                // Store booking
                const bookings = JSON.parse(localStorage.getItem('setsbykiara_bookings') || '[]');
                bookings.push(formData);
                localStorage.setItem('setsbykiara_bookings', JSON.stringify(bookings));
                
                // Show success with animation
                if (form) {
                    form.style.opacity = '0.5';
                    setTimeout(() => {
                        form.style.display = 'none';
                        form.style.opacity = '1';
                        if (successMessage) {
                            successMessage.style.display = 'block';
                            setTimeout(() => {
                                successMessage.classList.add('active');
                                // Scroll to success message
                                successMessage.scrollIntoView({ 
                                    behavior: 'smooth',
                                    block: 'center'
                                });
                            }, 50);
                        }
                    }, 300);
                }
                
                // Send notification
                sendBookingEmail(formData);
                
                // Reset button
                setTimeout(() => {
                    submitBtn.classList.remove('loading');
                    submitBtn.disabled = false;
                    submitBtn.innerHTML = '<i class="fas fa-paper-plane"></i> Submit Booking Request';
                }, 1000);
            }, 2000);
        }
        
        function resetForm() {
            const form = document.getElementById('bookingForm');
            const successMessage = document.getElementById('successMessage');
            
            if (form) {
                form.reset();
                form.style.display = 'flex';
                // Scroll to form
                setTimeout(() => {
                    form.scrollIntoView({ 
                        behavior: 'smooth',
                        block: 'center'
                    });
                }, 100);
            }
            if (successMessage) {
                successMessage.classList.remove('active');
                setTimeout(() => {
                    successMessage.style.display = 'none';
                }, 300);
            }
        }
        
        // ============================================
        // EMAIL NOTIFICATION
        // ============================================
        function sendBookingEmail(bookingData) {
            // Simulated email - in production, this would send to a server
            console.log('Booking received:', bookingData);
            
            // For demo purposes, show a mobile-friendly notification
            if (isMobile && 'Notification' in window && Notification.permission === 'granted') {
                new Notification('Booking Confirmed!', {
                    body: 'Kiara will contact you within 24 hours.',
                    icon: 'https://cdn-icons-png.flaticon.com/512/3468/3468373.png'
                });
            }
        }
        
        // ============================================
        // COPY PHONE NUMBER - TOUCH OPTIMIZED
        // ============================================
        function copyPhoneNumber() {
            const text = '4324253341';
            
            if (navigator.clipboard && window.isSecureContext) {
                navigator.clipboard.writeText(text).then(() => {
                    showCopyFeedback();
                }).catch(err => {
                    fallbackCopy(text);
                });
            } else {
                fallbackCopy(text);
            }
        }
        
        function fallbackCopy(text) {
            const textArea = document.createElement('textarea');
            textArea.value = text;
            textArea.style.position = 'fixed';
            textArea.style.left = '-999999px';
            textArea.style.top = '-999999px';
            document.body.appendChild(textArea);
            textArea.focus();
            textArea.select();
            
            try {
                document.execCommand('copy');
                showCopyFeedback();
            } catch (err) {
                console.log('Failed to copy:', err);
                alert('Phone number: ' + text);
            }
            
            textArea.remove();
        }
        
        function showCopyFeedback() {
            const phoneEl = document.querySelector('.phone-number');
            if (!phoneEl) return;
            
            const original = phoneEl.innerHTML;
            phoneEl.innerHTML = '<i class="fas fa-check"></i> <span>Copied!</span>';
            phoneEl.style.background = 'rgba(255, 133, 162, 0.2)';
            
            // Haptic feedback on mobile
            if (isMobile && navigator.vibrate) {
                navigator.vibrate(50);
            }
            
            setTimeout(() => {
                phoneEl.innerHTML = original;
                phoneEl.style.background = '';
            }, 2000);
        }
        
        // ============================================
        // LIGHTBOX - TOUCH OPTIMIZED
        // ============================================
        function openLightbox(imgSrc) {
            const lightbox = document.getElementById('lightbox');
            const lightboxImg = document.getElementById('lightbox-img');
            
            if (!lightbox || !lightboxImg) return;
            
            // Set image
            lightboxImg.src = imgSrc;
            
            // Show lightbox
            lightbox.classList.add('active');
            document.body.style.overflow = 'hidden';
            
            // Prevent scrolling on mobile
            if (isMobile) {
                document.documentElement.style.overflow = 'hidden';
            }
            
            // Add touch gestures for mobile
            if (isMobile) {
                setupTouchGestures(lightboxImg);
            }
        }
        
        function closeLightbox() {
            const lightbox = document.getElementById('lightbox');
            if (!lightbox) return;
            
            lightbox.classList.remove('active');
            document.body.style.overflow = '';
            
            if (isMobile) {
                document.documentElement.style.overflow = '';
            }
        }
        
        function setupTouchGestures(img) {
            let scale = 1;
            let lastTouchDistance = 0;
            
            img.addEventListener('touchstart', handleTouchStart, { passive: false });
            img.addEventListener('touchmove', handleTouchMove, { passive: false });
            img.addEventListener('touchend', handleTouchEnd);
            
            function handleTouchStart(e) {
                if (e.touches.length === 2) {
                    lastTouchDistance = getTouchDistance(e.touches);
                }
            }
            
            function handleTouchMove(e) {
                if (e.touches.length === 2) {
                    e.preventDefault();
                    const touchDistance = getTouchDistance(e.touches);
                    const scaleChange = touchDistance / lastTouchDistance;
                    
                    scale = Math.max(1, Math.min(3, scale * scaleChange));
                    img.style.transform = `scale(${scale})`;
                    
                    lastTouchDistance = touchDistance;
                } else if (e.touches.length === 1 && scale === 1) {
                    // Allow single finger scroll when not zoomed
                }
            }
            
            function handleTouchEnd() {
                if (scale > 1.5) {
                    // Reset scale after a delay
                    setTimeout(() => {
                        scale = 1;
                        img.style.transform = 'scale(1)';
                        img.style.transition = 'transform 0.3s ease';
                        setTimeout(() => {
                            img.style.transition = '';
                        }, 300);
                    }, 1000);
                }
            }
            
            function getTouchDistance(touches) {
                const dx = touches[0].clientX - touches[1].clientX;
                const dy = touches[0].clientY - touches[1].clientY;
                return Math.sqrt(dx * dx + dy * dy);
            }
        }
        
        // Close lightbox with ESC key
        document.addEventListener('keydown', function(e) {
            if (e.key === 'Escape') {
                closeLightbox();
            }
        });
        
        // Close lightbox when tapping outside image on mobile
        document.getElementById('lightbox')?.addEventListener('click', function(e) {
            if (e.target === this || e.target.classList.contains('lightbox-close')) {
                closeLightbox();
            }
        });
        
        // ============================================
        // ANIMATIONS
        // ============================================
        function triggerAnimations() {
            const elements = document.querySelectorAll('.fade-in');
            elements.forEach(el => {
                el.classList.add('visible');
            });
        }
        
        // ============================================
        // MOBILE FORM UX IMPROVEMENTS
        // ============================================
        function setupMobileFormUX() {
            if (!isMobile) return;
            
            // Focus management for mobile
            const inputs = document.querySelectorAll('input, select, textarea');
            inputs.forEach(input => {
                input.addEventListener('focus', function() {
                    // Scroll input into view
                    setTimeout(() => {
                        this.scrollIntoView({ 
                            behavior: 'smooth',
                            block: 'center'
                        });
                    }, 300);
                });
                
                // Improve number input on mobile
                if (input.type === 'tel') {
                    input.setAttribute('inputmode', 'tel');
                    input.setAttribute('pattern', '[0-9]*');
                }
                
                if (input.type === 'email') {
                    input.setAttribute('inputmode', 'email');
                }
            });
            
            // Prevent zoom on focus in iOS
            document.addEventListener('focusin', function(e) {
                if (e.target.matches('input, select, textarea')) {
                    setTimeout(() => {
                        document.body.style.zoom = '1';
                    }, 100);
                }
            });
        }
        
        // ============================================
        // INITIALIZATION
        // ============================================
        document.addEventListener('DOMContentLoaded', function() {
            // Set current year
            document.getElementById('currentYear').textContent = new Date().getFullYear();
            
            // Check mobile
            checkMobile();
            window.addEventListener('resize', checkMobile);
            
            // Setup image error handlers
            document.querySelectorAll('img').forEach(img => {
                img.onerror = () => handleImageError(img);
            });
            
            // Initial animations
            setTimeout(triggerAnimations, 200);
            
            // Setup mobile form UX
            setupMobileFormUX();
            
            // Fix Dropbox URLs
            setTimeout(() => {
                document.querySelectorAll('img[src*="dropbox"]').forEach(img => {
                    let src = img.src;
                    if (src.includes('www.dropbox.com')) {
                        src = src.replace('www.dropbox.com', 'dl.dropboxusercontent.com');
                        if (!src.includes('raw=1')) {
                            src += (src.includes('?') ? '&' : '?') + 'raw=1';
                        }
                        // Add mobile-specific cache busting
                        if (isMobile) {
                            src += '&mobile=1';
                        }
                        img.src = src;
                    }
                });
            }, 500);
            
            // Request notification permission (for demo)
            if ('Notification' in window && Notification.permission === 'default') {
                Notification.requestPermission();
            }
            
            // Add touch feedback to buttons
            document.querySelectorAll('button, .btn, a[onclick]').forEach(btn => {
                btn.addEventListener('touchstart', function() {
                    this.style.opacity = '0.8';
                });
                btn.addEventListener('touchend', function() {
                    this.style.opacity = '1';
                });
            });
            
            // Prevent pull-to-refresh on mobile (optional)
            document.addEventListener('touchmove', function(e) {
                if (e.scale !== 1) {
                    e.preventDefault();
                }
            }, { passive: false });
        });
        
        // ============================================
        // FIX MOBILE VIEWPORT ON RESIZE
        // ============================================
        window.addEventListener('orientationchange', function() {
            // Fix viewport on orientation change
            setTimeout(() => {
                document.documentElement.style.height = 'initial';
                setTimeout(() => {
                    document.documentElement.style.height = '100%';
                }, 100);
            }, 300);
        });
        
        // ============================================
        // IMPROVE TOUCH SCROLLING
        // ============================================
        let touchStartY = 0;
        
        document.addEventListener('touchstart', function(e) {
            touchStartY = e.touches[0].clientY;
        }, { passive: true });
        
        document.addEventListener('touchmove', function(e) {
            // Prevent rubber-band scrolling at the top
            if (window.scrollY === 0 && e.touches[0].clientY > touchStartY) {
                e.preventDefault();
            }
        }, { passive: false });
    </script>
</body>
</html>
