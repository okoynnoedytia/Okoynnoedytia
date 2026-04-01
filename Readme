<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover, user-scalable=yes">
    <title>Окоянное дитя | Бесовские ритуалы</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: #03030a;
            color: #e8e6e3;
            line-height: 1.5;
            scroll-behavior: smooth;
            overflow-x: hidden;
            cursor: default;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 0%; }
            50% { background-position: 100% 100%; }
            100% { background-position: 0% 0%; }
        }

        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at 20% 30%, rgba(80, 20, 20, 0.4), rgba(10, 5, 15, 0.9)),
                        repeating-linear-gradient(45deg, rgba(100, 30, 30, 0.1) 0px, rgba(100, 30, 30, 0.1) 2px, transparent 2px, transparent 20px);
            background-size: 200% 200%, 30px 30px;
            animation: gradientShift 15s ease infinite;
            pointer-events: none;
            z-index: 0;
        }

        .smoke-container {
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 2;
            overflow: hidden;
        }

        .smoke {
            position: absolute;
            bottom: 0;
            left: 50%;
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, rgba(80, 40, 30, 0.4) 0%, rgba(30, 20, 15, 0.2) 50%, transparent 80%);
            border-radius: 50%;
            filter: blur(30px);
            animation: smokeDrift 12s ease-in-out infinite;
            opacity: 0;
        }

        @keyframes smokeDrift {
            0% {
                transform: translateX(-50%) translateY(0) scale(0.8);
                opacity: 0;
            }
            20% {
                opacity: 0.6;
            }
            80% {
                opacity: 0.4;
            }
            100% {
                transform: translateX(-50%) translateY(-300px) scale(2);
                opacity: 0;
            }
        }

        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
            overflow: hidden;
        }

        .particle {
            position: absolute;
            background: rgba(170, 90, 58, 0.3);
            border-radius: 50%;
            pointer-events: none;
            animation: floatParticle linear infinite;
        }

        @keyframes floatParticle {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 0.5;
            }
            90% {
                opacity: 0.5;
            }
            100% {
                transform: translateY(-20vh) rotate(360deg);
                opacity: 0;
            }
        }

        .container {
            width: 100%;
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 32px;
            position: relative;
            z-index: 10;
        }

        .glass {
            backdrop-filter: blur(12px);
            background: rgba(10, 10, 20, 0.4);
            border: 1px solid rgba(170, 90, 58, 0.2);
        }

        .animate-on-scroll {
            opacity: 0;
            transform: translateY(40px);
            transition: all 0.8s cubic-bezier(0.2, 0.9, 0.4, 1.1);
        }

        .animate-on-scroll.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .navbar {
            position: sticky;
            top: 0;
            background: rgba(3, 3, 10, 0.85);
            backdrop-filter: blur(20px);
            z-index: 1000;
            padding: 18px 0;
            border-bottom: 1px solid rgba(170, 90, 58, 0.3);
            transition: all 0.3s;
        }

        .nav-flex {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 16px;
        }

        .logo-icon {
            width: 52px;
            height: 52px;
            border-radius: 50%;
            object-fit: cover;
            border: 1.5px solid #aa5a3a;
            background: #0f0f14;
            transition: all 0.3s;
        }

        .logo-icon:hover {
            box-shadow: 0 0 25px rgba(170, 90, 58, 0.6);
            transform: scale(1.02);
        }

        .logo-text h1 {
            font-size: 1.5rem;
            font-weight: 600;
            letter-spacing: 0.5px;
            color: #e0cfb0;
        }

        .logo-text p {
            font-size: 0.65rem;
            color: #aa5a3a;
            letter-spacing: 1px;
        }

        .nav-links {
            display: flex;
            gap: 32px;
            align-items: center;
            flex-wrap: wrap;
        }

        .nav-links a {
            text-decoration: none;
            font-weight: 500;
            font-size: 0.9rem;
            color: #cdc6bc;
            transition: all 0.3s;
            position: relative;
        }

        .nav-links a::before {
            content: '';
            position: absolute;
            bottom: -4px;
            left: 0;
            width: 0;
            height: 2px;
            background: linear-gradient(90deg, #aa5a3a, #cc8855);
            transition: width 0.3s;
        }

        .nav-links a:hover::before {
            width: 100%;
        }

        .nav-links a:hover {
            color: #bc6f4a;
            text-shadow: 0 0 10px rgba(170, 90, 58, 0.5);
        }

        .btn-outline {
            border: 1px solid #aa5a3a;
            padding: 8px 22px;
            border-radius: 40px;
            font-weight: 500;
            font-size: 0.8rem;
            background: transparent;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .btn-outline::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(170, 90, 58, 0.4), transparent);
            transition: left 0.5s;
        }

        .btn-outline:hover::before {
            left: 100%;
        }

        .btn-outline:hover {
            background: rgba(170, 90, 58, 0.2);
            box-shadow: 0 0 20px rgba(170, 90, 58, 0.4);
            transform: translateY(-2px);
        }

        .hero {
            padding: 100px 0 70px;
        }

        .hero-grid {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 60px;
        }

        .hero-text {
            text-align: center;
            width: 100%;
            max-width: 900px;
            margin: 0 auto;
        }

        .hero-badge {
            display: inline-block;
            padding: 8px 20px;
            font-size: 0.75rem;
            font-weight: 500;
            color: #bc6f4a;
            margin-bottom: 24px;
            letter-spacing: 2px;
            background: rgba(170, 90, 58, 0.15);
            border-radius: 40px;
            animation: pulseGlow 2s infinite;
        }

        @keyframes pulseGlow {
            0%, 100% { box-shadow: 0 0 5px rgba(170, 90, 58, 0.3); }
            50% { box-shadow: 0 0 20px rgba(170, 90, 58, 0.6); }
        }

        .hero-text h2 {
            font-size: 3.2rem;
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 24px;
            background: linear-gradient(135deg, #e0cfb0, #bc6f4a);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .hero-text p {
            font-size: 1.05rem;
            color: #b8aa9a;
            max-width: 100%;
            margin-bottom: 36px;
            font-weight: 400;
        }

        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 60px;
            flex-wrap: wrap;
        }

        .stat-item {
            font-weight: 700;
            font-size: 1.8rem;
            color: #bc6f4a;
            text-align: center;
            transition: all 0.3s;
            cursor: default;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 6px;
        }

        .stat-item i {
            font-size: 1.6rem;
            color: #aa5a3a;
            margin-bottom: 2px;
        }

        .stat-item:hover {
            transform: scale(1.1);
            text-shadow: 0 0 20px rgba(170, 90, 58, 0.6);
        }

        .stat-item span {
            font-size: 0.8rem;
            font-weight: 400;
            color: #8f7a66;
            display: block;
        }

        .hero-image {
            background: rgba(15, 15, 25, 0.5);
            backdrop-filter: blur(10px);
            border-radius: 50%;
            padding: 40px;
            text-align: center;
            border: 1px solid rgba(170, 90, 58, 0.4);
            width: 100%;
            max-width: 450px;
            margin: 0 auto;
            transition: all 0.4s;
        }

        .svg-container {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 30px;
            flex-wrap: wrap;
        }

        .effect-svg {
            filter: drop-shadow(0 0 8px rgba(170, 90, 58, 0.6));
            transition: all 0.3s ease;
        }

        .effect-svg:hover {
            filter: drop-shadow(0 0 20px rgba(255, 80, 40, 0.8));
            transform: scale(1.02);
        }

        .rotating {
            animation: rotatePentagram 20s linear infinite;
        }

        @keyframes rotatePentagram {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .moon-wave {
            animation: moonFloat 4s ease-in-out infinite;
        }

        @keyframes moonFloat {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }

        .wave-line {
            animation: waveMove 3s ease-in-out infinite;
        }

        @keyframes waveMove {
            0%, 100% { d: path("M 10 80 L 30 78 L 50 82 L 70 80 L 90 78 L 110 82"); }
            50% { d: path("M 10 82 L 30 80 L 50 84 L 70 82 L 90 80 L 110 84"); }
        }

        .about {
            padding: 90px 0;
            background: rgba(10, 10, 18, 0.6);
            backdrop-filter: blur(8px);
            border-top: 1px solid rgba(170, 90, 58, 0.2);
            border-bottom: 1px solid rgba(170, 90, 58, 0.2);
        }

        .about-grid {
            display: flex;
            flex-direction: column;
            gap: 50px;
        }

        .about-text h3 {
            font-size: 2rem;
            font-weight: 700;
            color: #e0cfb0;
            margin-bottom: 28px;
            text-align: center;
        }

        .about-text p {
            color: #b8aa9a;
            margin-bottom: 24px;
            font-size: 1rem;
            text-align: center;
            max-width: 900px;
            margin-left: auto;
            margin-right: auto;
        }

        .about-stats {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-top: 40px;
            justify-content: center;
        }

        .about-stat {
            background: rgba(10, 10, 20, 0.6);
            backdrop-filter: blur(8px);
            padding: 24px 28px;
            border-radius: 20px;
            border: 1px solid rgba(170, 90, 58, 0.3);
            flex: 1;
            min-width: 160px;
            text-align: center;
            transition: all 0.3s;
        }

        .about-stat:hover {
            transform: translateY(-8px);
            border-color: #aa5a3a;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3), 0 0 20px rgba(170, 90, 58, 0.3);
        }

        .about-stat h4 {
            font-size: 2rem;
            font-weight: 700;
            color: #bc6f4a;
        }

        .about-stat p {
            font-size: 0.8rem;
            margin-bottom: 0;
            text-align: center;
        }

        .terms {
            padding: 60px 0;
            background: #03030a;
        }

        .terms-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .term-card {
            background: rgba(15, 15, 25, 0.6);
            backdrop-filter: blur(8px);
            border-radius: 24px;
            padding: 32px;
            text-align: center;
            border: 1px solid rgba(170, 90, 58, 0.2);
            transition: all 0.3s;
        }

        .term-card:hover {
            transform: translateY(-8px);
            border-color: #aa5a3a;
            box-shadow: 0 20px 35px rgba(0, 0, 0, 0.3), 0 0 20px rgba(170, 90, 58, 0.3);
        }

        .term-icon {
            font-size: 48px;
            color: #aa5a3a;
            margin-bottom: 20px;
        }

        .term-card h4 {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 12px;
            color: #e0cfb0;
        }

        .term-card p {
            color: #b8aa9a;
            font-size: 0.9rem;
            line-height: 1.5;
        }

        .price-highlight {
            font-size: 1.8rem;
            font-weight: 700;
            color: #bc6f4a;
            margin: 15px 0 5px;
        }

        .services {
            padding: 90px 0;
            background: rgba(10, 10, 18, 0.4);
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-header h3 {
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 15px;
            background: linear-gradient(135deg, #e0cfb0, #bc6f4a);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .section-header p {
            color: #9a8a76;
            font-size: 0.95rem;
        }

        .services-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }

        .service-card {
            background: rgba(15, 15, 25, 0.6);
            backdrop-filter: blur(8px);
            border-radius: 24px;
            padding: 32px;
            transition: all 0.4s;
            border: 1px solid rgba(170, 90, 58, 0.2);
            position: relative;
            overflow: hidden;
            text-align: center;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(170, 90, 58, 0.1), transparent);
            transition: left 0.6s;
        }

        .service-card:hover::before {
            left: 100%;
        }

        .service-card:hover {
            transform: translateY(-10px);
            border-color: #aa5a3a;
            box-shadow: 0 25px 45px rgba(0, 0, 0, 0.4), 0 0 25px rgba(170, 90, 58, 0.3);
        }

        .service-icon-wrapper {
            width: 80px;
            height: 80px;
            margin: 0 auto 24px auto;
            background: linear-gradient(135deg, rgba(170, 90, 58, 0.2), rgba(10, 10, 20, 0.6));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 1px solid rgba(170, 90, 58, 0.4);
            transition: all 0.4s cubic-bezier(0.2, 0.9, 0.4, 1.1);
        }

        .service-icon {
            font-size: 38px;
            color: #bc6f4a;
            filter: drop-shadow(0 0 5px rgba(170, 90, 58, 0.5));
            transition: all 0.3s;
        }

        .service-card:hover .service-icon-wrapper {
            transform: scale(1.05) rotate(3deg);
            border-color: #aa5a3a;
            box-shadow: 0 0 25px rgba(170, 90, 58, 0.5);
            background: linear-gradient(135deg, rgba(170, 90, 58, 0.35), rgba(10, 10, 20, 0.7));
        }

        .service-card:hover .service-icon {
            transform: scale(1.1);
            filter: drop-shadow(0 0 12px rgba(170, 90, 58, 0.8));
            color: #d47a4e;
        }

        .service-card h4 {
            font-size: 1.3rem;
            font-weight: 600;
            margin-bottom: 12px;
            color: #e0cfb0;
        }

        .service-card p {
            color: #b8aa9a;
            margin-bottom: 18px;
            font-size: 0.85rem;
            line-height: 1.5;
        }

        .price-ls {
            font-weight: 500;
            font-size: 0.8rem;
            color: #bc6f4a;
            background: rgba(170, 90, 58, 0.15);
            display: inline-block;
            padding: 6px 16px;
            border-radius: 40px;
            transition: all 0.3s;
        }

        .service-card:hover .price-ls {
            background: rgba(170, 90, 58, 0.3);
            box-shadow: 0 0 12px rgba(170, 90, 58, 0.4);
        }

        .warning-note {
            background: rgba(15, 15, 25, 0.6);
            backdrop-filter: blur(8px);
            border-left: 3px solid #aa5a3a;
            padding: 22px 32px;
            border-radius: 20px;
            margin-top: 50px;
            font-size: 0.85rem;
            color: #b8aa9a;
            text-align: center;
            transition: all 0.3s;
        }

        .warning-note:hover {
            border-left-width: 5px;
            background: rgba(15, 15, 25, 0.8);
        }

        .features {
            padding: 90px 0;
            background: rgba(10, 10, 18, 0.6);
            backdrop-filter: blur(8px);
            border-top: 1px solid rgba(170, 90, 58, 0.2);
            border-bottom: 1px solid rgba(170, 90, 58, 0.2);
        }

        .feature-list {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 50px;
            margin-top: 50px;
        }

        .feature-item {
            text-align: center;
            max-width: 200px;
            transition: all 0.3s;
            cursor: default;
        }

        .feature-item:hover {
            transform: translateY(-8px);
        }

        .feature-item i {
            font-size: 42px;
            background: rgba(170, 90, 58, 0.15);
            padding: 20px;
            border-radius: 50%;
            color: #aa5a3a;
            margin-bottom: 18px;
            transition: all 0.3s;
            display: inline-block;
        }

        .feature-item:hover i {
            background: rgba(170, 90, 58, 0.3);
            box-shadow: 0 0 25px rgba(170, 90, 58, 0.4);
            transform: scale(1.05);
        }

        .feature-item h4 {
            font-size: 1rem;
            font-weight: 600;
            margin-bottom: 8px;
            color: #e0cfb0;
        }

        .feature-item p {
            font-size: 0.75rem;
            color: #9a8a76;
        }

        .reviews-channel {
            padding: 70px 0;
            background: #03030a;
        }

        .channel-card {
            background: rgba(15, 15, 25, 0.7);
            backdrop-filter: blur(12px);
            border-radius: 32px;
            padding: 48px 32px;
            text-align: center;
            border: 1px solid rgba(170, 90, 58, 0.4);
            transition: all 0.4s ease;
            max-width: 700px;
            margin: 0 auto;
        }

        .channel-card:hover {
            transform: translateY(-8px);
            border-color: #aa5a3a;
            box-shadow: 0 25px 45px rgba(0, 0, 0, 0.4), 0 0 30px rgba(170, 90, 58, 0.3);
        }

        .channel-icon {
            font-size: 58px;
            color: #aa5a3a;
            margin-bottom: 20px;
            filter: drop-shadow(0 0 12px rgba(170, 90, 58, 0.5));
        }

        .channel-card h3 {
            font-size: 1.8rem;
            font-weight: 700;
            margin-bottom: 16px;
            background: linear-gradient(135deg, #e0cfb0, #bc6f4a);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .channel-card p {
            color: #b8aa9a;
            font-size: 1rem;
            margin-bottom: 28px;
        }

        .channel-btn {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: rgba(170, 90, 58, 0.2);
            padding: 14px 36px;
            border-radius: 60px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1rem;
            color: #e0cfb0;
            transition: all 0.3s;
            border: 1px solid #aa5a3a;
        }

        .channel-btn:hover {
            transform: scale(1.03);
            box-shadow: 0 0 25px rgba(170, 90, 58, 0.5);
            background: rgba(170, 90, 58, 0.35);
            color: #fff;
        }

        .channel-btn i {
            font-size: 1.2rem;
        }

        .channel-footer {
            margin-top: 24px;
            font-size: 0.75rem;
            color: #7a6a5a;
        }

        .contact {
            background: #03030a;
            padding: 90px 0;
        }

        .contact-flex {
            display: flex;
            flex-direction: column;
            gap: 45px;
        }

        .contact-text {
            text-align: center;
        }

        .contact-text h3 {
            font-size: 1.8rem;
            font-weight: 700;
            margin-bottom: 15px;
            color: #e0cfb0;
        }

        .contact-text p {
            color: #b8aa9a;
            font-size: 0.95rem;
        }

        .managers-list {
            margin-top: 35px;
            background: rgba(15, 15, 25, 0.6);
            backdrop-filter: blur(8px);
            padding: 32px 35px;
            border-radius: 24px;
            border: 1px solid rgba(170, 90, 58, 0.3);
            transition: all 0.3s;
        }

        .managers-list:hover {
            border-color: #aa5a3a;
            box-shadow: 0 0 30px rgba(170, 90, 58, 0.2);
        }

        .managers-list h4 {
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 20px;
            color: #bc6f4a;
            text-align: center;
        }

        .manager-tags {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 18px;
        }

        .manager-tag {
            background: rgba(10, 10, 20, 0.6);
            padding: 10px 22px;
            border-radius: 40px;
            font-size: 0.85rem;
            font-weight: 500;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            text-decoration: none;
            color: #cdc6bc;
            border: 1px solid rgba(170, 90, 58, 0.3);
            transition: all 0.3s;
        }

        .manager-tag:hover {
            background: rgba(170, 90, 58, 0.2);
            color: #bc6f4a;
            border-color: #aa5a3a;
            transform: translateY(-3px);
            box-shadow: 0 0 20px rgba(170, 90, 58, 0.3);
        }

        .owner-badge {
            border-color: #aa5a3a;
        }

        .contact-btn {
            background: rgba(170, 90, 58, 0.15);
            padding: 14px 38px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            color: #e0cfb0;
            display: inline-block;
            border: 1px solid #aa5a3a;
            text-align: center;
            width: fit-content;
            margin: 0 auto;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .contact-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s;
        }

        .contact-btn:hover::before {
            left: 100%;
        }

        .contact-btn:hover {
            background: rgba(170, 90, 58, 0.3);
            box-shadow: 0 0 30px rgba(170, 90, 58, 0.5);
            transform: translateY(-2px);
        }

        .legal-notice {
            background: rgba(15, 15, 25, 0.5);
            backdrop-filter: blur(8px);
            border: 1px solid rgba(170, 90, 58, 0.2);
            border-radius: 20px;
            padding: 30px 35px;
            margin: 50px 0 25px;
            font-size: 0.7rem;
            color: #9a8a76;
            line-height: 1.6;
            transition: all 0.3s;
        }

        .legal-notice:hover {
            border-color: rgba(170, 90, 58, 0.4);
        }

        .legal-notice h4 {
            color: #bc6f4a;
            margin-bottom: 18px;
            font-size: 0.85rem;
            font-weight: 600;
        }

        footer {
            background: #03030a;
            color: #7a6a5a;
            text-align: center;
            padding: 35px;
            font-size: 0.75rem;
            border-top: 1px solid rgba(170, 90, 58, 0.2);
        }

        .divider {
            width: 60px;
            height: 2px;
            background: linear-gradient(90deg, transparent, #aa5a3a, transparent);
            margin: 20px auto;
        }

        /* Стили для блока Бес-гид и история */
        .imp-story {
            padding: 80px 0;
            background: linear-gradient(135deg, rgba(10, 5, 15, 0.9), rgba(3, 3, 10, 0.95));
            border-top: 1px solid rgba(170, 90, 58, 0.3);
            border-bottom: 1px solid rgba(170, 90, 58, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .imp-story::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: repeating-linear-gradient(45deg, rgba(170, 90, 58, 0.03) 0px, rgba(170, 90, 58, 0.03) 2px, transparent 2px, transparent 20px);
            pointer-events: none;
        }
        
        .story-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 50px;
            align-items: center;
        }
        
        @media (min-width: 900px) {
            .story-grid {
                grid-template-columns: 0.8fr 1.2fr;
                gap: 60px;
            }
        }
        
        .story-avatar {
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
        }
        
        .avatar-container {
            position: relative;
            width: 280px;
            height: 280px;
        }
        
        .story-imp-svg {
            width: 100%;
            height: 100%;
            filter: drop-shadow(0 0 20px rgba(170, 90, 58, 0.6));
            animation: impFloat 3s ease-in-out infinite;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .story-imp-svg:hover {
            filter: drop-shadow(0 0 35px rgba(255, 80, 40, 0.9));
            transform: scale(1.02);
        }
        
        @keyframes impFloat {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .avatar-glow {
            position: absolute;
            top: 50%;
            left: 50%;
            width: 100%;
            height: 100%;
            transform: translate(-50%, -50%);
            background: radial-gradient(circle, rgba(170, 90, 58, 0.3), transparent 70%);
            border-radius: 50%;
            z-index: -1;
            animation: glowPulse 2s ease-in-out infinite;
        }
        
        @keyframes glowPulse {
            0%, 100% { opacity: 0.3; transform: translate(-50%, -50%) scale(0.9); }
            50% { opacity: 0.8; transform: translate(-50%, -50%) scale(1.1); }
        }
        
        .story-content {
            text-align: center;
        }
        
        @media (min-width: 900px) {
            .story-content {
                text-align: left;
            }
        }
        
        .story-badge {
            display: inline-block;
            background: rgba(170, 90, 58, 0.2);
            padding: 6px 16px;
            border-radius: 40px;
            font-size: 0.75rem;
            font-weight: 600;
            color: #ff8866;
            letter-spacing: 1px;
            margin-bottom: 20px;
            border: 1px solid rgba(170, 90, 58, 0.4);
        }
        
        .story-content h3 {
            font-size: 1.8rem;
            font-weight: 700;
            margin: 20px 0 16px;
            background: linear-gradient(135deg, #e0cfb0, #bc6f4a);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }
        
        .story-content p {
            color: #b8aa9a;
            font-size: 0.95rem;
            line-height: 1.6;
            margin-bottom: 18px;
        }
        
        .story-divider {
            width: 60px;
            height: 2px;
            background: linear-gradient(90deg, #aa5a3a, transparent);
            margin: 25px 0;
        }
        
        @media (min-width: 900px) {
            .story-divider {
                margin: 25px 0;
            }
        }
        
        .story-fact {
            background: rgba(170, 90, 58, 0.1);
            border-left: 3px solid #aa5a3a;
            padding: 18px 22px;
            border-radius: 16px;
            margin: 25px 0;
            display: flex;
            gap: 12px;
            align-items: flex-start;
            transition: all 0.3s;
        }
        
        .story-fact:hover {
            background: rgba(170, 90, 58, 0.2);
            transform: translateX(5px);
        }
        
        .story-fact i {
            font-size: 24px;
            color: #aa5a3a;
            margin-top: 2px;
        }
        
        .story-fact span {
            color: #d0c0aa;
            font-size: 0.85rem;
            line-height: 1.5;
        }
        
        .story-stats {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }
        
        @media (min-width: 900px) {
            .story-stats {
                justify-content: flex-start;
            }
        }
        
        .story-stat {
            text-align: center;
            background: rgba(10, 10, 20, 0.5);
            padding: 15px 20px;
            border-radius: 20px;
            min-width: 100px;
            border: 1px solid rgba(170, 90, 58, 0.3);
            transition: all 0.3s;
        }
        
        .story-stat:hover {
            transform: translateY(-5px);
            border-color: #aa5a3a;
            background: rgba(170, 90, 58, 0.1);
        }
        
        .story-stat i {
            font-size: 28px;
            color: #aa5a3a;
            display: block;
            margin-bottom: 8px;
        }
        
        .story-stat span {
            font-size: 1.6rem;
            font-weight: 700;
            color: #bc6f4a;
            display: block;
        }
        
        .story-stat p {
            font-size: 0.7rem;
            margin: 5px 0 0;
            color: #9a8a76;
        }

        /* Стили для беса-гида */
        .imp-guide {
            position: fixed;
            bottom: 30px;
            right: 30px;
            width: 120px;
            height: 120px;
            cursor: pointer;
            z-index: 1000;
            transition: all 0.3s ease;
            filter: drop-shadow(0 0 10px rgba(170, 90, 58, 0.5));
            animation: bounceGuide 2s ease-in-out infinite;
            display: none;
        }
        
        .imp-guide:hover {
            transform: scale(1.1);
            filter: drop-shadow(0 0 20px rgba(255, 80, 40, 0.8));
        }
        
        @keyframes bounceGuide {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-8px); }
        }
        
        .imp-tooltip {
            position: absolute;
            bottom: 130px;
            right: 0;
            background: rgba(0, 0, 0, 0.95);
            backdrop-filter: blur(10px);
            padding: 10px 18px;
            border-radius: 25px;
            font-size: 0.75rem;
            font-weight: 500;
            color: #ff8866;
            white-space: nowrap;
            border: 1px solid #aa5a3a;
            opacity: 0;
            transition: opacity 0.3s;
            pointer-events: none;
            box-shadow: 0 0 15px rgba(170, 90, 58, 0.3);
            font-family: monospace;
            z-index: 1001;
        }
        
        .imp-guide:hover .imp-tooltip {
            opacity: 1;
        }
        
        /* Стили для игрового модального окна */
        .game-modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            backdrop-filter: blur(10px);
            z-index: 2000;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .game-container {
            background: #0a0a18;
            border: 2px solid #aa5a3a;
            border-radius: 32px;
            width: 90%;
            max-width: 900px;
            height: 80%;
            max-height: 600px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 50px rgba(170, 90, 58, 0.5);
        }
        
        .game-area {
            position: relative;
            width: 100%;
            height: 100%;
            background: rgba(20, 10, 20, 0.95);
            overflow: hidden;
            cursor: crosshair;
        }
        
        .game-imp {
            position: absolute;
            width: 80px;
            height: 80px;
            cursor: pointer;
            transition: all 0.05s linear;
            filter: drop-shadow(0 0 8px #aa5a3a);
            z-index: 10;
        }
        
        .game-imp.real {
            filter: drop-shadow(0 0 15px #ff5533);
        }
        
        .game-message {
            position: absolute;
            bottom: 20px;
            left: 0;
            right: 0;
            text-align: center;
            background: rgba(0, 0, 0, 0.8);
            color: #ff8866;
            padding: 12px;
            font-size: 0.9rem;
            z-index: 20;
            font-weight: 500;
        }
        
        .game-stats {
            position: absolute;
            top: 15px;
            right: 20px;
            background: rgba(0, 0, 0, 0.7);
            padding: 8px 18px;
            border-radius: 30px;
            font-size: 0.9rem;
            color: #ffaa77;
            z-index: 20;
            font-weight: bold;
        }
        
        .close-game {
            position: absolute;
            top: 15px;
            left: 20px;
            background: #aa5a3a;
            border: none;
            color: white;
            width: 36px;
            height: 36px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 20px;
            z-index: 20;
            transition: all 0.3s;
        }
        
        .close-game:hover {
            transform: scale(1.1);
            background: #ff5533;
        }
        
        .quiz-area {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: #0a0a18;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 30px;
            z-index: 30;
        }
        
        .quiz-question {
            font-size: 1.3rem;
            margin-bottom: 30px;
            text-align: center;
            color: #e0cfb0;
            font-weight: 600;
        }
        
        .quiz-options {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        
        .quiz-option {
            background: rgba(170, 90, 58, 0.2);
            border: 1px solid #aa5a3a;
            padding: 12px 28px;
            border-radius: 60px;
            cursor: pointer;
            transition: all 0.2s;
            color: #e0cfb0;
            font-size: 1rem;
        }
        
        .quiz-option:hover {
            background: rgba(170, 90, 58, 0.5);
            transform: scale(1.02);
        }
        
        .quiz-feedback {
            margin-top: 30px;
            font-size: 1rem;
            color: #ff8866;
            text-align: center;
        }
        
        .discount-badge {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            background: linear-gradient(135deg, #aa5a3a, #ff3300);
            color: white;
            padding: 20px 40px;
            border-radius: 20px;
            font-size: 1.8rem;
            font-weight: bold;
            z-index: 2000;
            animation: discountPulse 0.5s ease-out;
            box-shadow: 0 0 50px rgba(255, 51, 0, 0.8);
            text-align: center;
            white-space: nowrap;
            font-family: monospace;
        }
        
        @keyframes discountPulse {
            0% { transform: translate(-50%, -50%) scale(0); opacity: 0; }
            50% { transform: translate(-50%, -50%) scale(1.2); }
            100% { transform: translate(-50%, -50%) scale(1); opacity: 1; }
        }

        @media (min-width: 768px) {
            .hero-grid {
                flex-direction: row;
                text-align: left;
            }
            .hero-text {
                text-align: left;
                margin: 0;
            }
            .hero-stats {
                justify-content: flex-start;
            }
            .services-grid {
                grid-template-columns: repeat(2, 1fr);
            }
            .contact-flex {
                flex-direction: row;
                justify-content: space-between;
                align-items: center;
            }
            .contact-text {
                text-align: left;
                flex: 1;
            }
            .managers-list h4 {
                text-align: left;
            }
            .manager-tags {
                justify-content: flex-start;
            }
            .contact-btn {
                margin: 0;
            }
        }

        @media (min-width: 1200px) {
            .services-grid {
                grid-template-columns: repeat(3, 1fr);
            }
            .hero-text h2 {
                font-size: 3.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="smoke-container" id="smokeContainer"></div>
    <div class="particles" id="particles"></div>

    <!-- Бес-гид -->
    <div class="imp-guide" id="impGuide">
        <svg viewBox="0 0 100 100" style="width: 100%; height: 100%;">
            <defs>
                <radialGradient id="impBodyDark" cx="50%" cy="50%" r="50%">
                    <stop offset="0%" stop-color="#5a2a2a"/>
                    <stop offset="100%" stop-color="#2a0a0a"/>
                </radialGradient>
                <radialGradient id="impFace" cx="40%" cy="40%" r="60%">
                    <stop offset="0%" stop-color="#3a1a1a"/>
                    <stop offset="100%" stop-color="#1a0505"/>
                </radialGradient>
                <linearGradient id="hornGradient" x1="0%" y1="0%" x2="100%" y2="0%">
                    <stop offset="0%" stop-color="#aa5a3a"/>
                    <stop offset="100%" stop-color="#6a2a1a"/>
                </linearGradient>
            </defs>
            
            <ellipse cx="50" cy="85" rx="35" ry="12" fill="rgba(0,0,0,0.5)" opacity="0.5"/>
            
            <path d="M 35 55 L 35 75 Q 35 82 42 83 L 58 83 Q 65 82 65 75 L 65 55 Q 65 48 58 48 L 42 48 Q 35 48 35 55 Z" 
                  fill="url(#impBodyDark)" stroke="#aa5a3a" stroke-width="1.5"/>
            
            <path d="M 45 58 L 50 62 L 55 58" stroke="#ff6644" stroke-width="2" fill="none" opacity="0.7"/>
            
            <circle cx="50" cy="32" r="22" fill="url(#impFace)" stroke="#aa5a3a" stroke-width="2"/>
            
            <path d="M 35 25 L 42 28 M 65 25 L 58 28" stroke="#ff8866" stroke-width="3" stroke-linecap="round" fill="none"/>
            <path d="M 33 27 L 40 30 M 67 27 L 60 30" stroke="#aa5a3a" stroke-width="2" stroke-linecap="round" fill="none"/>
            
            <path d="M 32 18 L 22 5 L 32 14" fill="url(#hornGradient)" stroke="#cc6633" stroke-width="1.5"/>
            <path d="M 68 18 L 78 5 L 68 14" fill="url(#hornGradient)" stroke="#cc6633" stroke-width="1.5"/>
            <path d="M 28 15 L 24 8" stroke="#ffaa77" stroke-width="1" fill="none"/>
            <path d="M 72 15 L 76 8" stroke="#ffaa77" stroke-width="1" fill="none"/>
            
            <circle cx="38" cy="31" r="5" fill="#ff3300" opacity="0.9">
                <animate attributeName="r" values="5;5.5;5" dur="1s" repeatCount="indefinite"/>
            </circle>
            <circle cx="62" cy="31" r="5" fill="#ff3300" opacity="0.9">
                <animate attributeName="r" values="5;5.5;5" dur="1s" repeatCount="indefinite"/>
            </circle>
            <ellipse cx="38" cy="31" rx="2.2" ry="3.5" fill="black"/>
            <ellipse cx="62" cy="31" rx="2.2" ry="3.5" fill="black"/>
            
            <path d="M 42 42 Q 50 48 58 42" stroke="#ff8866" stroke-width="2.5" fill="none" stroke-linecap="round"/>
            <path d="M 44 41 L 42 45 L 46 43" fill="#ccaa88" stroke="#aa5a3a" stroke-width="1"/>
            <path d="M 56 41 L 58 45 L 54 43" fill="#ccaa88" stroke="#aa5a3a" stroke-width="1"/>
            
            <circle cx="44" cy="38" r="2" fill="rgba(170,90,58,0.4)">
                <animate attributeName="r" values="2;3;2" dur="1.2s" repeatCount="indefinite"/>
            </circle>
            <circle cx="56" cy="38" r="2" fill="rgba(170,90,58,0.4)">
                <animate attributeName="r" values="2;3;2" dur="1.2s" repeatCount="indefinite"/>
            </circle>
            
            <path d="M 28 28 L 20 35 L 26 32" fill="#3a1a1a" stroke="#aa5a3a" stroke-width="1"/>
            <path d="M 72 28 L 80 35 L 74 32" fill="#3a1a1a" stroke="#aa5a3a" stroke-width="1"/>
        </svg>
        <div class="imp-tooltip" id="impTooltip">😈 ХОЧЕШЬ СКИДКУ? ЖМИ! 😈</div>
    </div>

    <div class="navbar">
        <div class="container nav-flex">
            <div class="logo">
                <img class="logo-icon" src="https://i.ibb.co/hxWYZNN9/IMG-20260330-151743-780.jpg" alt="Окоянное дитя лого">
                <div class="logo-text">
                    <h1>Окоянное дитя</h1>
                    <p>бесовские ритуалы</p>
                </div>
            </div>
            <div class="nav-links">
                <a href="#">Главная</a>
                <a href="#about">О нас</a>
                <a href="#services">Услуги</a>
                <a href="#terms">Условия</a>
                <a href="#contact">Контакты</a>
                <a href="#" class="btn-outline">Запись</a>
            </div>
        </div>
    </div>

    <main>
        <div class="container hero">
            <div class="hero-grid">
                <div class="hero-text animate-on-scroll">
                    <div class="hero-badge">✦ бесовские ритуалы ✦</div>
                    <h2>Бесовские ритуалы<br>и работа с миром мёртвых</h2>
                    <p>Присушки, привязки, порча через семиотрядных бесов, работа с бесовыми князьями и духами. Полная конфиденциальность. Результат подтверждён более чем 1000 клиентов.</p>
                    <div class="hero-stats">
                        <div class="stat-item">1000+ <span>ритуалов</span></div>
                        <div class="stat-item">5 лет <span>практики</span></div>
                        <div class="stat-item">
                            <i class="fas fa-eye-slash"></i>
                            анонимность
                            <span>полная конфиденциальность</span>
                        </div>
                    </div>
                </div>
                <div class="hero-image animate-on-scroll">
                    <div class="svg-container">
                        <svg class="effect-svg rotating" width="120" height="120" viewBox="0 0 100 100">
                            <defs>
                                <radialGradient id="pentagramGlow" cx="50%" cy="50%" r="50%">
                                    <stop offset="0%" stop-color="#ff5533" stop-opacity="0.8"/>
                                    <stop offset="100%" stop-color="#aa3300" stop-opacity="0.3"/>
                                </radialGradient>
                            </defs>
                            <circle cx="50" cy="50" r="45" fill="none" stroke="#aa5a3a" stroke-width="1.5" stroke-dasharray="5 5"/>
                            <polygon points="50,15 65,40 85,45 70,65 75,90 50,78 25,90 30,65 15,45 35,40 50,15" 
                                     fill="url(#pentagramGlow)" stroke="#aa5a3a" stroke-width="2"/>
                            <circle cx="50" cy="50" r="8" fill="#ff4422">
                                <animate attributeName="r" values="8;10;8" dur="1.5s" repeatCount="indefinite"/>
                            </circle>
                        </svg>

                        <svg class="effect-svg moon-wave" width="120" height="120" viewBox="0 0 100 100">
                            <defs>
                                <radialGradient id="moonGradient" cx="30%" cy="30%" r="60%">
                                    <stop offset="0%" stop-color="#ffdd99"/>
                                    <stop offset="100%" stop-color="#aa8866"/>
                                </radialGradient>
                            </defs>
                            <path d="M 70 20 Q 85 30 75 45 Q 90 55 70 65 Q 80 75 65 80 Q 70 90 55 85 Q 40 95 35 80 Q 20 85 25 70 Q 10 55 25 45 Q 15 30 30 35 Q 35 20 50 25 Q 60 10 70 20" 
                                  fill="url(#moonGradient)" stroke="#aa5a3a" stroke-width="1.5"/>
                            <path class="wave-line" d="M 10 80 L 30 78 L 50 82 L 70 80 L 90 78 L 110 82" stroke="#aa5a3a" stroke-width="2" fill="none" stroke-linecap="round" opacity="0.7"/>
                            <path class="wave-line" d="M 10 88 L 30 86 L 50 90 L 70 88 L 90 86 L 110 90" stroke="#cc8866" stroke-width="1.5" fill="none" stroke-linecap="round" opacity="0.5"/>
                        </svg>

                        <svg class="effect-svg" width="100" height="100" viewBox="0 0 100 100">
                            <defs>
                                <radialGradient id="eyeGradient" cx="35%" cy="40%" r="50%">
                                    <stop offset="0%" stop-color="#2a0a0a"/>
                                    <stop offset="100%" stop-color="#0a0101"/>
                                </radialGradient>
                                <radialGradient id="irisGradient" cx="40%" cy="45%" r="50%">
                                    <stop offset="0%" stop-color="#ff5500"/>
                                    <stop offset="100%" stop-color="#aa3300"/>
                                </radialGradient>
                            </defs>
                            <ellipse cx="50" cy="50" rx="45" ry="48" fill="url(#eyeGradient)" stroke="#aa5a3a" stroke-width="2"/>
                            <ellipse cx="50" cy="50" rx="35" ry="38" fill="#3a0f0f" stroke="#aa5a3a" stroke-width="1"/>
                            <circle cx="50" cy="52" r="22" fill="url(#irisGradient)"/>
                            <circle id="pupilAnim" cx="47" cy="50" r="12" fill="#000000">
                                <animate attributeName="r" values="12;13;11;12" dur="3s" repeatCount="indefinite" />
                                <animate attributeName="cx" values="47;48;46;47" dur="4s" repeatCount="indefinite" />
                                <animate attributeName="cy" values="50;51;49;50" dur="3.5s" repeatCount="indefinite" />
                            </circle>
                            <circle cx="38" cy="42" r="4" fill="white" opacity="0.9"/>
                            <circle cx="42" cy="44" r="1.5" fill="white" opacity="0.7"/>
                            <path d="M 70 35 L 85 28 M 68 45 L 82 42 M 30 35 L 15 28 M 32 45 L 18 42 M 50 70 L 50 88 M 50 30 L 50 12" stroke="#aa3a2a" stroke-width="2" stroke-linecap="round" opacity="0.7"/>
                        </svg>
                    </div>
                    <div class="divider"></div>
                </div>
            </div>
        </div>

        <div class="about" id="about">
            <div class="container about-grid">
                <div class="about-text animate-on-scroll">
                    <h3>О практике «Окоянное дитя»</h3>
                    <p>Мы — специалисты по бесовским ритуалам, работающие с мелкими бесами, бесовыми князьями и миром мёртвых. За 5 лет проведено более 1000 обрядов без единого отката.</p>
                    <p>Каждый ритуал сопровождается диагностикой и индивидуальным подходом. Работаем только через Telegram, гарантируем полную анонимность и соблюдение сроков.</p>
                    <div class="about-stats">
                        <div class="about-stat">
                            <h4>5 лет</h4>
                            <p>практики с бесами</p>
                        </div>
                        <div class="about-stat">
                            <h4>1000+</h4>
                            <p>успешных обрядов</p>
                        </div>
                        <div class="about-stat">
                            <h4>Бесовые князи</h4>
                            <p>высший уровень</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="terms" id="terms">
            <div class="container">
                <div class="section-header animate-on-scroll">
                    <h3>Условия работы</h3>
                    <p>Порядок проведения ритуалов и стоимость</p>
                </div>
                <div class="terms-grid">
                    <div class="term-card animate-on-scroll">
                        <div class="term-icon"><i class="fas fa-stethoscope"></i></div>
                        <h4>Диагностика</h4>
                        <p>Обязательная бесплатная диагностика перед любым ритуалом для определения точного воздействия и отсутствия противопоказаний.</p>
                        <div class="price-highlight">2 500 ₽</div>
                        <p style="font-size: 0.7rem; margin-top: 5px;">фиксированная цена</p>
                    </div>
                    <div class="term-card animate-on-scroll">
                        <div class="term-icon"><i class="fas fa-calendar-check"></i></div>
                        <h4>Сроки выполнения</h4>
                        <p>Работа будет поставлена в день, когда всё будет обговорено и согласовано. Оперативность без потери качества.</p>
                    </div>
                    <div class="term-card animate-on-scroll">
                        <div class="term-icon"><i class="fas fa-gem"></i></div>
                        <h4>Цены на ритуалы</h4>
                        <p>Все ритуалы проводятся только после бесплатной диагностики. Цены индивидуальны и зависят от сложности задачи.</p>
                        <div class="price-highlight">индивидуально</div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Блок: Бес-гид и история (ИСПРАВЛЕНО: "тому" вместо "той") -->
        <div class="imp-story" id="impStory">
            <div class="container">
                <div class="story-grid">
                    <div class="story-avatar animate-on-scroll">
                        <div class="avatar-container">
                            <svg viewBox="0 0 200 200" class="story-imp-svg">
                                <defs>
                                    <radialGradient id="storyImpBody" cx="50%" cy="50%" r="50%">
                                        <stop offset="0%" stop-color="#6a2a2a"/>
                                        <stop offset="100%" stop-color="#2a0a0a"/>
                                    </radialGradient>
                                    <radialGradient id="storyImpFace" cx="40%" cy="40%" r="60%">
                                        <stop offset="0%" stop-color="#4a2a2a"/>
                                        <stop offset="100%" stop-color="#1a0505"/>
                                    </radialGradient>
                                </defs>
                                
                                <circle cx="100" cy="100" r="95" fill="none" stroke="#aa5a3a" stroke-width="1" stroke-dasharray="5 5" opacity="0.5">
                                    <animate attributeName="r" values="95;98;95" dur="3s" repeatCount="indefinite"/>
                                </circle>
                                
                                <path d="M 70 110 L 70 150 Q 70 165 85 166 L 115 166 Q 130 165 130 150 L 130 110 Q 130 95 115 95 L 85 95 Q 70 95 70 110 Z" 
                                      fill="url(#storyImpBody)" stroke="#aa5a3a" stroke-width="2"/>
                                
                                <circle cx="100" cy="65" r="35" fill="url(#storyImpFace)" stroke="#aa5a3a" stroke-width="2.5"/>
                                
                                <path d="M 65 40 L 45 10 L 65 30" fill="#aa5a3a" stroke="#cc6633" stroke-width="2"/>
                                <path d="M 135 40 L 155 10 L 135 30" fill="#aa5a3a" stroke="#cc6633" stroke-width="2"/>
                                
                                <circle cx="75" cy="60" r="8" fill="#ff4422">
                                    <animate attributeName="r" values="8;9;8" dur="1s" repeatCount="indefinite"/>
                                </circle>
                                <circle cx="125" cy="60" r="8" fill="#ff4422">
                                    <animate attributeName="r" values="8;9;8" dur="1s" repeatCount="indefinite"/>
                                </circle>
                                <ellipse cx="75" cy="60" rx="3" ry="5" fill="black"/>
                                <ellipse cx="125" cy="60" rx="3" ry="5" fill="black"/>
                                
                                <path d="M 85 85 Q 100 95 115 85" stroke="#ff8866" stroke-width="3" fill="none" stroke-linecap="round"/>
                                <path d="M 88 82 L 85 88 L 92 84" fill="#ccaa88" stroke="#aa5a3a"/>
                                <path d="M 112 82 L 115 88 L 108 84" fill="#ccaa88" stroke="#aa5a3a"/>
                                
                                <path d="M 60 45 L 72 52 M 140 45 L 128 52" stroke="#ff8866" stroke-width="4" stroke-linecap="round"/>
                                
                                <path d="M 55 55 L 68 60 L 62 70" stroke="#aa5a3a" stroke-width="2.5" fill="none"/>
                                
                                <circle cx="100" cy="92" r="6" fill="rgba(170,90,58,0.5)">
                                    <animate attributeName="r" values="6;10;6" dur="1.5s" repeatCount="indefinite"/>
                                    <animate attributeName="opacity" values="0.5;0.2;0.5" dur="1.5s" repeatCount="indefinite"/>
                                </circle>
                            </svg>
                            <div class="avatar-glow"></div>
                        </div>
                    </div>
                    
                    <div class="story-content animate-on-scroll">
                        <div class="story-badge">🔥 БЕС-ГИД 🔥</div>
                        <h3>Кто такой этот бесёнок?</h3>
                        <p>— А вот и я, собственной персоной! <strong>Маленький, злой, но справедливый бес-гид</strong>. Меня приставили к этому сайту, чтобы всякие сомневающиеся не убегали, а сразу задавали вопросы.</p>
                        <p>Я тут главный по <strong>навигации, подсказкам и скидкам</strong>. Если хочешь получить скидку на расклад Таро — жми на меня и проходи испытание!</p>
                        
                        <div class="story-divider"></div>
                        
                        <h3>📜 История «Окоянного дитя»</h3>
                        <p>Началось всё <strong>пять лет назад</strong> в глухой деревне, где старуха-знахарка передала свои знания <strong>тому</strong>, кто оказался способен видеть <strong>мир мёртвых и бесов</strong>. Со временем практика выросла в мощный канал работы с <strong>семиотрядными бесами, бесовыми князьями и духами умерших</strong>.</p>
                        <p>Сегодня «Окоянное дитя» — это <strong>более 1000 успешных ритуалов</strong>, полная анонимность и никаких откатов. Каждый обряд проходит диагностику, чтобы удар был точным, а результат — быстрым.</p>
                        <p>— А я, бес-гид, тут для того, чтобы <strong>клиент не заблудился</strong> и вовремя получил своё. Жми на меня, если хочешь получить скидку — я хоть и вредный, но помогу тем, кто пройдёт испытание!</p>
                        
                        <div class="story-fact">
                            <i class="fas fa-fire"></i>
                            <span><strong>Забавный факт:</strong> Самый нетерпеливый клиент пытался поймать меня 47 раз. На 48-й я сдался и дал ему шанс на скидку. Так что настойчивость вознаграждается!</span>
                        </div>
                        
                        <div class="story-stats">
                            <div class="story-stat">
                                <i class="fas fa-skull"></i>
                                <span>1000+</span>
                                <p>ритуалов</p>
                            </div>
                            <div class="story-stat">
                                <i class="fas fa-cat"></i>
                                <span>5 лет</span>
                                <p>с бесами</p>
                            </div>
                            <div class="story-stat">
                                <i class="fas fa-mask"></i>
                                <span>анонимно</span>
                                <p>100%</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="services" id="services">
            <div class="container">
                <div class="section-header animate-on-scroll">
                    <h3>Перечень услуг</h3>
                    <p>Все ритуалы проводятся только после бесплатной диагностики. Цены индивидуальны.</p>
                </div>
                <div class="services-grid">
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-heart-broken service-icon"></i>
                        </div>
                        <h4>Присушка</h4>
                        <p>Любовная привязка, мягкое воздействие на чувства. Бесовская присушка на тоску и влечение.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-link service-icon"></i>
                        </div>
                        <h4>Бесовская привязка</h4>
                        <p>Крепкая привязка человека к вам, к дому или месту. Морок на неотступность.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-snowplow service-icon"></i>
                        </div>
                        <h4>Отворот</h4>
                        <p>Остуда чувств, отворот от соперника или ненужных отношений.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-users-slash service-icon"></i>
                        </div>
                        <h4>Рассорка</h4>
                        <p>Разрушение отношений между людьми, ссоры, конфликты через мелких бесов.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-skull service-icon"></i>
                        </div>
                        <h4>Порча через семиотрядных бесов</h4>
                        <p>Мощный ритуал на поражение врага через семерых бесов-разрушителей.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-ghost service-icon"></i>
                        </div>
                        <h4>Работа с миром мёртвых</h4>
                        <p>Вызов духов умерших, получение информации, родовые вопросы, некро-канал.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-crown service-icon"></i>
                        </div>
                        <h4>Бесовые князи</h4>
                        <p>Работа с высшими бесовскими сущностями. Ритуалы для особо сложных задач.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-eye service-icon"></i>
                        </div>
                        <h4>Диагностика магических способностей</h4>
                        <p>Проверка вашего канала, видят ли бесы, сила рода, скрытые задатки.</p>
                        <div class="price-ls">2 500 ₽</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-coins service-icon"></i>
                        </div>
                        <h4>Морок на удачу и деньги</h4>
                        <p>Бесовский напуск на прибыль, везение в делах, открытие денежного канала.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-chalkboard-user service-icon"></i>
                        </div>
                        <h4>Расклады Таро</h4>
                        <p>Диагностика ситуации, просмотр отношений, будущего, скрытых причин.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                    <div class="service-card animate-on-scroll">
                        <div class="service-icon-wrapper">
                            <i class="fas fa-star-of-life service-icon"></i>
                        </div>
                        <h4>Индивидуальный запрос</h4>
                        <p>Любой ритуал под ваш запрос. Обсуждается лично, цена индивидуально.</p>
                        <div class="price-ls">цена после диагностики</div>
                    </div>
                </div>
                <div class="warning-note animate-on-scroll">
                    <i class="fas fa-info-circle" style="margin-right: 10px;"></i> 
                    <strong>Важно:</strong> Все ритуалы проводятся только после бесплатной диагностики. Диагностика — 2 500 ₽ (фиксированная цена). Работа будет поставлена в день, когда всё будет обговорено. Цены на ритуалы индивидуальны.
                </div>
            </div>
        </div>

        <div class="features">
            <div class="container">
                <div class="section-header animate-on-scroll">
                    <h3>Преимущества</h3>
                    <p>Почему выбирают нашу практику</p>
                </div>
                <div class="feature-list">
                    <div class="feature-item animate-on-scroll">
                        <i class="fas fa-cat"></i>
                        <h4>Работа с бесами</h4>
                        <p>Мелкие бесы и князи</p>
                    </div>
                    <div class="feature-item animate-on-scroll">
                        <i class="fas fa-user-secret"></i>
                        <h4>Анонимность</h4>
                        <p>Полная конфиденциальность</p>
                    </div>
                    <div class="feature-item animate-on-scroll">
                        <i class="fas fa-chart-line"></i>
                        <h4>Без отката</h4>
                        <p>Защита на каждый обряд</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="reviews-channel">
            <div class="container">
                <div class="channel-card animate-on-scroll">
                    <div class="channel-icon">
                        <i class="fab fa-telegram"></i>
                    </div>
                    <h3>Канал с отзывами</h3>
                    <p>Реальные истории клиентов, результаты ритуалов, отзывы о работе с бесами и миром мёртвых</p>
                    <a href="https://t.me/okoyanny" target="_blank" class="channel-btn">
                        <i class="fab fa-telegram"></i> Перейти в канал
                    </a>
                    <div class="channel-footer">
                        @okoyanny
                    </div>
                </div>
            </div>
        </div>

        <div class="contact" id="contact">
            <div class="container contact-flex">
                <div class="contact-text animate-on-scroll">
                    <h3>Связаться</h3>
                    <p>Telegram — связь с владельцем и менеджерами. Бесплатная диагностика.</p>
                    
                    <div class="managers-list">
                        <h4><i class="fas fa-user-circle"></i> Контакты:</h4>
                        <div class="manager-tags">
                            <a href="https://t.me/Zara_zzaww" target="_blank" class="manager-tag owner-badge">
                                <i class="fab fa-telegram"></i> @Zara_zzaww — владелец
                            </a>
                            <a href="https://t.me/Yfcghuuuuuu" target="_blank" class="manager-tag">
                                <i class="fab fa-telegram"></i> @Yfcghuuuuuu — менеджер
                            </a>
                            <a href="https://t.me/kinght11111" target="_blank" class="manager-tag">
                                <i class="fab fa-telegram"></i> @kinght11111 — менеджер
                            </a>
                        </div>
                        <div class="divider"></div>
                        <p style="font-size: 0.75rem; margin-top: 16px; color: #9a8a76;">Ответ в течение часа. Все вопросы конфиденциальны. Диагностика — 2 500 ₽</p>
                    </div>
                </div>
                <a href="https://t.me/Zara_zzaww" target="_blank" class="contact-btn animate-on-scroll">Написать владельцу</a>
            </div>
        </div>

        <div class="container">
            <div class="legal-notice animate-on-scroll">
                <h4>📜 ОФИЦИАЛЬНОЕ УВЕДОМЛЕНИЕ О ПРАВОВОМ СТАТУСЕ</h4>
                <p>В соответствии с Федеральным законом от 25.07.2002 №114-ФЗ «О противодействии экстремистской деятельности» и ст. 282 УК РФ администрация заявляет:</p>
                <p>Все материалы носят информационно-аналитический, историко-культурный и просветительский характер. Контент предназначен для совершеннолетних (18+). Категорически отрицаем связь с запрещёнными организациями. Не осуществляем деятельность религиозных объединений. Администрация не несёт ответственности за самостоятельную интерпретацию материалов пользователями.</p>
            </div>
        </div>
    </main>

    <footer>
        <div class="container">
            <p>© 2026 Окоянное дитя — бесовские ритуалы. Все обряды 18+. Информационно-просветительский характер.</p>
        </div>
    </footer>

    <script>
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 60;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                const size = Math.random() * 5 + 2;
                particle.style.width = size + 'px';
                particle.style.height = size + 'px';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.animationDuration = Math.random() * 15 + 8 + 's';
                particle.style.animationDelay = Math.random() * 15 + 's';
                particle.style.background = `rgba(170, 90, 58, ${Math.random() * 0.4 + 0.1})`;
                particlesContainer.appendChild(particle);
            }
        }
        
        function createSmoke() {
            const smokeContainer = document.getElementById('smokeContainer');
            
            setInterval(() => {
                const smoke = document.createElement('div');
                smoke.classList.add('smoke');
                smoke.style.left = Math.random() * 100 + '%';
                smoke.style.animationDuration = Math.random() * 8 + 6 + 's';
                smoke.style.animationDelay = '0s';
                smokeContainer.appendChild(smoke);
                
                setTimeout(() => {
                    smoke.remove();
                }, 12000);
            }, 3000);
        }
        
        createParticles();
        createSmoke();
        
        const animateElements = document.querySelectorAll('.animate-on-scroll');
        
        const checkVisibility = () => {
            animateElements.forEach(el => {
                const rect = el.getBoundingClientRect();
                const windowHeight = window.innerHeight;
                if (rect.top < windowHeight - 100) {
                    el.classList.add('visible');
                }
            });
        };
        
        window.addEventListener('scroll', checkVisibility);
        window.addEventListener('load', checkVisibility);
        
        // МИНИ-ИГРА ДЛЯ ПОЛУЧЕНИЯ СКИДКИ
        document.addEventListener('DOMContentLoaded', function() {
            const imp = document.getElementById('impGuide');
            const tooltip = document.getElementById('impTooltip');
            let gameActive = false;
            let discountGiven = localStorage.getItem('tarotDiscountApplied') === 'true';
            
            if (!imp) return;
            
            // Бес появляется через 2 секунды
            setTimeout(() => {
                imp.style.display = 'block';
                imp.style.opacity = '0';
                imp.style.transform = 'scale(0) rotate(180deg)';
                imp.style.transition = 'all 0.5s cubic-bezier(0.68, -0.55, 0.265, 1.55)';
                setTimeout(() => {
                    imp.style.opacity = '1';
                    imp.style.transform = 'scale(1) rotate(0deg)';
                }, 50);
            }, 2000);
            
            function showDiscount() {
                if (discountGiven) return;
                discountGiven = true;
                localStorage.setItem('tarotDiscountApplied', 'true');
                
                const discountDiv = document.createElement('div');
                discountDiv.className = 'discount-badge';
                discountDiv.innerHTML = '🎉 СКИДКА 25% НА РАСКЛАД ТАРО! 🎉<br><span style="font-size: 1rem;">Пиши @Zara_zzaww с кодом BES25</span>';
                document.body.appendChild(discountDiv);
                
                setTimeout(() => {
                    discountDiv.style.transition = 'all 0.5s';
                    discountDiv.style.opacity = '0';
                    discountDiv.style.transform = 'translate(-50%, -50%) scale(0)';
                    setTimeout(() => discountDiv.remove(), 500);
                }, 4000);
                
                tooltip.textContent = '🎁 СКИДКА АКТИВИРОВАНА! ПИШИ! 🎁';
                tooltip.style.opacity = '1';
                setTimeout(() => {
                    if (!imp.matches(':hover')) tooltip.style.opacity = '0';
                }, 3000);
            }
            
            function startGame() {
                if (gameActive) return;
                if (discountGiven) {
                    tooltip.textContent = "😈 Скидка уже твоя! Пиши @Zara_zzaww с кодом BES25 😈";
                    tooltip.style.opacity = '1';
                    setTimeout(() => tooltip.style.opacity = '0', 2000);
                    return;
                }
                
                gameActive = true;
                
                const modal = document.createElement('div');
                modal.className = 'game-modal';
                modal.innerHTML = `
                    <div class="game-container">
                        <button class="close-game">✕</button>
                        <div class="game-area" id="gameArea">
                            <div class="game-stats">Ошибки: <span id="errorCount">0</span>/3</div>
                            <div class="game-message" id="gameMessage">Поймай НАСТОЯЩЕГО беса! У него красные глаза и золотой огонёк!</div>
                        </div>
                    </div>
                `;
                document.body.appendChild(modal);
                
                const gameArea = document.getElementById('gameArea');
                const errorSpan = document.getElementById('errorCount');
                const messageDiv = document.getElementById('gameMessage');
                let errors = 0;
                let moveIntervals = [];
                let realImp = null;
                
                function createImpElement(isReal, left, top) {
                    const div = document.createElement('div');
                    div.className = 'game-imp';
                    if (isReal) div.classList.add('real');
                    div.style.left = left + 'px';
                    div.style.top = top + 'px';
                    div.style.position = 'absolute';
                    div.innerHTML = `
                        <svg viewBox="0 0 80 80" width="80" height="80">
                            <circle cx="40" cy="45" r="28" fill="#3a1a1a" stroke="#aa5a3a" stroke-width="1.5"/>
                            <circle cx="28" cy="38" r="6" fill="${isReal ? '#ff3300' : '#aa5a3a'}"/>
                            <circle cx="52" cy="38" r="6" fill="${isReal ? '#ff3300' : '#aa5a3a'}"/>
                            <ellipse cx="28" cy="38" rx="2.5" ry="4" fill="black"/>
                            <ellipse cx="52" cy="38" rx="2.5" ry="4" fill="black"/>
                            <path d="M 30 55 L 40 62 L 50 55" stroke="#ff8866" stroke-width="2" fill="none"/>
                            ${isReal ? '<circle cx="40" cy="28" r="4" fill="gold"><animate attributeName="r" values="4;6;4" dur="0.8s" repeatCount="indefinite"/></circle>' : ''}
                        </svg>
                    `;
                    div.dataset.real = isReal ? 'true' : 'false';
                    return div;
                }
                
                function startMoving(imp) {
                    let dx = (Math.random() - 0.5) * 3;
                    let dy = (Math.random() - 0.5) * 3;
                    const interval = setInterval(() => {
                        if (!gameArea.contains(imp)) {
                            clearInterval(interval);
                            return;
                        }
                        let left = parseFloat(imp.style.left);
                        let top = parseFloat(imp.style.top);
                        left += dx;
                        top += dy;
                        const maxX = gameArea.clientWidth - 80;
                        const maxY = gameArea.clientHeight - 80;
                        if (left <= 0) { left = 0; dx = -dx; }
                        if (left >= maxX) { left = maxX; dx = -dx; }
                        if (top <= 0) { top = 0; dy = -dy; }
                        if (top >= maxY) { top = maxY; dy = -dy; }
                        imp.style.left = left + 'px';
                        imp.style.top = top + 'px';
                    }, 50);
                    moveIntervals.push(interval);
                    imp.moveInterval = interval;
                }
                
                function stopAllMoving() {
                    moveIntervals.forEach(interval => clearInterval(interval));
                    moveIntervals = [];
                }
                
                function startQuiz() {
                    stopAllMoving();
                    gameArea.innerHTML = '';
                    const quizDiv = document.createElement('div');
                    quizDiv.className = 'quiz-area';
                    const questions = [
                        { text: "Сколько лет практике «Окоянное дитя»?", options: ["3 года", "5 лет", "7 лет"], correct: 1 },
                        { text: "С какими сущностями работает практика?", options: ["Ангелы", "Семиотрядные бесы", "Домовые"], correct: 1 },
                        { text: "Что нужно сделать перед любым ритуалом?", options: ["Купить свечи", "Бесплатную диагностику", "Поститься"], correct: 1 }
                    ];
                    let currentQ = 0;
                    let quizErrors = 0;
                    
                    function showQuestion() {
                        quizDiv.innerHTML = `
                            <div style="text-align:center; width:100%;">
                                <div class="quiz-question">${questions[currentQ].text}</div>
                                <div class="quiz-options">
                                    ${questions[currentQ].options.map((opt, idx) => `<div class="quiz-option" data-opt="${idx}">${opt}</div>`).join('')}
                                </div>
                                <div class="quiz-feedback" id="quizFeedback"></div>
                            </div>
                        `;
                        quizDiv.querySelectorAll('.quiz-option').forEach(btn => {
                            btn.addEventListener('click', (e) => {
                                const selected = parseInt(btn.dataset.opt);
                                const feedback = quizDiv.querySelector('#quizFeedback');
                                if (selected === questions[currentQ].correct) {
                                    feedback.innerHTML = '✅ Верно!';
                                    currentQ++;
                                    if (currentQ < questions.length) {
                                        setTimeout(showQuestion, 800);
                                    } else {
                                        feedback.innerHTML = '🎉 Ты прошёл испытание! Скидка активирована! 🎉';
                                        setTimeout(() => {
                                            showDiscount();
                                            modal.remove();
                                            gameActive = false;
                                        }, 1500);
                                    }
                                } else {
                                    quizErrors++;
                                    feedback.innerHTML = `❌ Неправильно. Ошибок: ${quizErrors}/2`;
                                    if (quizErrors >= 2) {
                                        feedback.innerHTML = '💀 Слишком много ошибок. Игра проиграна! Начни заново...';
                                        setTimeout(() => {
                                            modal.remove();
                                            gameActive = false;
                                        }, 1500);
                                    }
                                }
                            });
                        });
                        gameArea.appendChild(quizDiv);
                    }
                    showQuestion();
                }
                
                // Создаём 6-8 бесов, один реальный
                const total = 6 + Math.floor(Math.random() * 3);
                const realIndex = Math.floor(Math.random() * total);
                
                for (let i = 0; i < total; i++) {
                    const isReal = (i === realIndex);
                    const left = 20 + Math.random() * (gameArea.clientWidth - 100);
                    const top = 20 + Math.random() * (gameArea.clientHeight - 100);
                    const impEl = createImpElement(isReal, left, top);
                    
                    impEl.addEventListener('click', (e) => {
                        e.stopPropagation();
                        if (impEl.dataset.real === 'true') {
                            stopAllMoving();
                            messageDiv.textContent = '✔️ Ты поймал настоящего беса! Теперь ответь на вопросы...';
                            document.querySelectorAll('.game-imp').forEach(el => el.remove());
                            startQuiz();
                        } else {
                            errors++;
                            errorSpan.textContent = errors;
                            messageDiv.textContent = `❌ Ложный бес! Штраф: ${errors}/3`;
                            if (errors >= 3) {
                                messageDiv.textContent = '💀 Слишком много ошибок! Игра проиграна. Начни заново...';
                                stopAllMoving();
                                setTimeout(() => {
                                    modal.remove();
                                    gameActive = false;
                                }, 1500);
                            } else {
                                impEl.remove();
                                const newLeft = 20 + Math.random() * (gameArea.clientWidth - 100);
                                const newTop = 20 + Math.random() * (gameArea.clientHeight - 100);
                                const newFake = createImpElement(false, newLeft, newTop);
                                newFake.addEventListener('click', arguments.callee);
                                gameArea.appendChild(newFake);
                                startMoving(newFake);
                            }
                        }
                    });
                    
                    gameArea.appendChild(impEl);
                    startMoving(impEl);
                    if (isReal) realImp = impEl;
                }
                
                modal.querySelector('.close-game').addEventListener('click', () => {
                    stopAllMoving();
                    modal.remove();
                    gameActive = false;
                });
            }
            
            imp.addEventListener('click', (e) => {
                e.stopPropagation();
                startGame();
            });
        });
    </script>
</body>
</html>
