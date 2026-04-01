<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover, user-scalable=yes">
    <title>Окоянное дитя | Бесовские ритуалы</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Все основные стили остаются из предыдущего файла */
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Inter', sans-serif; background: #03030a; color: #e8e6e3; line-height: 1.5; scroll-behavior: smooth; overflow-x: hidden; }
        @keyframes gradientShift { 0% { background-position: 0% 0%; } 50% { background-position: 100% 100%; } 100% { background-position: 0% 0%; } }
        body::before { content: ""; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: radial-gradient(circle at 20% 30%, rgba(80, 20, 20, 0.4), rgba(10, 5, 15, 0.9)), repeating-linear-gradient(45deg, rgba(100, 30, 30, 0.1) 0px, rgba(100, 30, 30, 0.1) 2px, transparent 2px, transparent 20px); background-size: 200% 200%, 30px 30px; animation: gradientShift 15s ease infinite; pointer-events: none; z-index: 0; }
        .smoke-container { position: fixed; bottom: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 2; overflow: hidden; }
        .smoke { position: absolute; bottom: 0; left: 50%; width: 200px; height: 200px; background: radial-gradient(circle, rgba(80, 40, 30, 0.4) 0%, rgba(30, 20, 15, 0.2) 50%, transparent 80%); border-radius: 50%; filter: blur(30px); animation: smokeDrift 12s ease-in-out infinite; opacity: 0; }
        @keyframes smokeDrift { 0% { transform: translateX(-50%) translateY(0) scale(0.8); opacity: 0; } 20% { opacity: 0.6; } 80% { opacity: 0.4; } 100% { transform: translateX(-50%) translateY(-300px) scale(2); opacity: 0; } }
        .particles { position: fixed; top: 0; left: 0; width: 100%; height: 100%; pointer-events: none; z-index: 1; overflow: hidden; }
        .particle { position: absolute; background: rgba(170, 90, 58, 0.3); border-radius: 50%; pointer-events: none; animation: floatParticle linear infinite; }
        @keyframes floatParticle { 0% { transform: translateY(100vh) rotate(0deg); opacity: 0; } 10% { opacity: 0.5; } 90% { opacity: 0.5; } 100% { transform: translateY(-20vh) rotate(360deg); opacity: 0; } }
        .container { width: 100%; max-width: 1400px; margin: 0 auto; padding: 0 32px; position: relative; z-index: 10; }
        .animate-on-scroll { opacity: 0; transform: translateY(40px); transition: all 0.8s cubic-bezier(0.2, 0.9, 0.4, 1.1); }
        .animate-on-scroll.visible { opacity: 1; transform: translateY(0); }
        .navbar { position: sticky; top: 0; background: rgba(3, 3, 10, 0.85); backdrop-filter: blur(20px); z-index: 1000; padding: 18px 0; border-bottom: 1px solid rgba(170, 90, 58, 0.3); }
        .nav-flex { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 20px; }
        .logo { display: flex; align-items: center; gap: 16px; }
        .logo-icon { width: 52px; height: 52px; border-radius: 50%; object-fit: cover; border: 1.5px solid #aa5a3a; background: #0f0f14; transition: all 0.3s; }
        .logo-icon:hover { box-shadow: 0 0 25px rgba(170, 90, 58, 0.6); transform: scale(1.02); }
        .logo-text h1 { font-size: 1.5rem; font-weight: 600; color: #e0cfb0; }
        .logo-text p { font-size: 0.65rem; color: #aa5a3a; letter-spacing: 1px; }
        .nav-links { display: flex; gap: 32px; align-items: center; flex-wrap: wrap; }
        .nav-links a { text-decoration: none; font-weight: 500; font-size: 0.9rem; color: #cdc6bc; transition: all 0.3s; position: relative; }
        .nav-links a::before { content: ''; position: absolute; bottom: -4px; left: 0; width: 0; height: 2px; background: linear-gradient(90deg, #aa5a3a, #cc8855); transition: width 0.3s; }
        .nav-links a:hover::before { width: 100%; }
        .nav-links a:hover { color: #bc6f4a; text-shadow: 0 0 10px rgba(170, 90, 58, 0.5); }
        .btn-outline { border: 1px solid #aa5a3a; padding: 8px 22px; border-radius: 40px; font-weight: 500; font-size: 0.8rem; background: transparent; transition: all 0.3s; position: relative; overflow: hidden; cursor: pointer; }
        .btn-outline::before { content: ''; position: absolute; top: 0; left: -100%; width: 100%; height: 100%; background: linear-gradient(90deg, transparent, rgba(170, 90, 58, 0.4), transparent); transition: left 0.5s; }
        .btn-outline:hover::before { left: 100%; }
        .btn-outline:hover { background: rgba(170, 90, 58, 0.2); box-shadow: 0 0 20px rgba(170, 90, 58, 0.4); transform: translateY(-2px); }
        .hero { padding: 100px 0 70px; }
        .hero-grid { display: flex; flex-direction: column; align-items: center; gap: 60px; }
        @media (min-width: 768px) { .hero-grid { flex-direction: row; text-align: left; } .hero-text { text-align: left; } .hero-stats { justify-content: flex-start; } }
        .hero-text { text-align: center; width: 100%; max-width: 900px; margin: 0 auto; }
        @media (min-width: 768px) { .hero-text { text-align: left; margin: 0; } }
        .hero-badge { display: inline-block; padding: 8px 20px; font-size: 0.75rem; font-weight: 500; color: #bc6f4a; margin-bottom: 24px; letter-spacing: 2px; background: rgba(170, 90, 58, 0.15); border-radius: 40px; animation: pulseGlow 2s infinite; }
        @keyframes pulseGlow { 0%, 100% { box-shadow: 0 0 5px rgba(170, 90, 58, 0.3); } 50% { box-shadow: 0 0 20px rgba(170, 90, 58, 0.6); } }
        .hero-text h2 { font-size: 3.2rem; font-weight: 700; line-height: 1.2; margin-bottom: 24px; background: linear-gradient(135deg, #e0cfb0, #bc6f4a); -webkit-background-clip: text; background-clip: text; color: transparent; }
        @media (min-width: 1200px) { .hero-text h2 { font-size: 3.8rem; } }
        .hero-text p { font-size: 1.05rem; color: #b8aa9a; margin-bottom: 36px; }
        .hero-stats { display: flex; justify-content: center; gap: 60px; flex-wrap: wrap; }
        .stat-item { font-weight: 700; font-size: 1.8rem; color: #bc6f4a; text-align: center; transition: all 0.3s; cursor: default; display: flex; flex-direction: column; align-items: center; gap: 6px; }
        .stat-item i { font-size: 1.6rem; color: #aa5a3a; }
        .stat-item:hover { transform: scale(1.1); text-shadow: 0 0 20px rgba(170, 90, 58, 0.6); }
        .stat-item span { font-size: 0.8rem; font-weight: 400; color: #8f7a66; }
        .hero-image { background: rgba(15, 15, 25, 0.3); backdrop-filter: blur(10px); border-radius: 40px; padding: 20px; text-align: center; border: 1px solid rgba(170, 90, 58, 0.3); width: 100%; max-width: 280px; margin: 0 auto; transition: all 0.4s; }
        .demon-eye-container { position: relative; width: 100%; max-width: 220px; margin: 0 auto; text-align: center; }
        .demon-eye { width: 100%; height: auto; filter: drop-shadow(0 0 20px rgba(170, 90, 58, 0.6)); transition: all 0.3s ease; cursor: pointer; }
        .demon-eye:hover { filter: drop-shadow(0 0 35px rgba(255, 80, 40, 0.9)); transform: scale(1.02); }
        .divider { width: 60px; height: 2px; background: linear-gradient(90deg, transparent, #aa5a3a, transparent); margin: 20px auto; }
        .about { padding: 90px 0; background: rgba(10, 10, 18, 0.6); backdrop-filter: blur(8px); border-top: 1px solid rgba(170, 90, 58, 0.2); border-bottom: 1px solid rgba(170, 90, 58, 0.2); }
        .about-text h3 { font-size: 2rem; font-weight: 700; color: #e0cfb0; margin-bottom: 28px; text-align: center; }
        .about-text p { color: #b8aa9a; margin-bottom: 24px; font-size: 1rem; text-align: center; max-width: 900px; margin-left: auto; margin-right: auto; }
        .about-stats { display: flex; flex-wrap: wrap; gap: 30px; margin-top: 40px; justify-content: center; }
        .about-stat { background: rgba(10, 10, 20, 0.6); backdrop-filter: blur(8px); padding: 24px 28px; border-radius: 20px; border: 1px solid rgba(170, 90, 58, 0.3); flex: 1; min-width: 160px; text-align: center; transition: all 0.3s; }
        .about-stat:hover { transform: translateY(-8px); border-color: #aa5a3a; box-shadow: 0 15px 35px rgba(0, 0, 0, 0.3), 0 0 20px rgba(170, 90, 58, 0.3); }
        .about-stat h4 { font-size: 2rem; font-weight: 700; color: #bc6f4a; }
        .about-stat p { font-size: 0.8rem; margin-bottom: 0; }
        .terms { padding: 60px 0; background: #03030a; }
        .terms-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 30px; margin-top: 40px; }
        .term-card { background: rgba(15, 15, 25, 0.6); backdrop-filter: blur(8px); border-radius: 24px; padding: 32px; text-align: center; border: 1px solid rgba(170, 90, 58, 0.2); transition: all 0.3s; }
        .term-card:hover { transform: translateY(-8px); border-color: #aa5a3a; box-shadow: 0 20px 35px rgba(0, 0, 0, 0.3), 0 0 20px rgba(170, 90, 58, 0.3); }
        .term-icon { font-size: 48px; color: #aa5a3a; margin-bottom: 20px; }
        .term-card h4 { font-size: 1.3rem; font-weight: 600; margin-bottom: 12px; color: #e0cfb0; }
        .term-card p { color: #b8aa9a; font-size: 0.9rem; }
        .price-highlight { font-size: 1.8rem; font-weight: 700; color: #bc6f4a; margin: 15px 0 5px; }
        .services { padding: 90px 0; background: rgba(10, 10, 18, 0.4); }
        .section-header { text-align: center; margin-bottom: 60px; }
        .section-header h3 { font-size: 2rem; font-weight: 700; margin-bottom: 15px; background: linear-gradient(135deg, #e0cfb0, #bc6f4a); -webkit-background-clip: text; background-clip: text; color: transparent; }
        .section-header p { color: #9a8a76; font-size: 0.95rem; }
        .services-grid { display: grid; grid-template-columns: 1fr; gap: 30px; }
        @media (min-width: 768px) { .services-grid { grid-template-columns: repeat(2, 1fr); } }
        @media (min-width: 1200px) { .services-grid { grid-template-columns: repeat(3, 1fr); } }
        .service-card { background: rgba(15, 15, 25, 0.6); backdrop-filter: blur(8px); border-radius: 24px; padding: 32px; transition: all 0.4s; border: 1px solid rgba(170, 90, 58, 0.2); position: relative; overflow: hidden; text-align: center; }
        .service-card::before { content: ''; position: absolute; top: 0; left: -100%; width: 100%; height: 100%; background: linear-gradient(90deg, transparent, rgba(170, 90, 58, 0.1), transparent); transition: left 0.6s; }
        .service-card:hover::before { left: 100%; }
        .service-card:hover { transform: translateY(-10px); border-color: #aa5a3a; box-shadow: 0 25px 45px rgba(0, 0, 0, 0.4), 0 0 25px rgba(170, 90, 58, 0.3); }
        .service-icon-wrapper { width: 80px; height: 80px; margin: 0 auto 24px auto; background: linear-gradient(135deg, rgba(170, 90, 58, 0.2), rgba(10, 10, 20, 0.6)); border-radius: 50%; display: flex; align-items: center; justify-content: center; border: 1px solid rgba(170, 90, 58, 0.4); transition: all 0.4s; }
        .service-icon { font-size: 38px; color: #bc6f4a; filter: drop-shadow(0 0 5px rgba(170, 90, 58, 0.5)); transition: all 0.3s; }
        .service-card:hover .service-icon-wrapper { transform: scale(1.05) rotate(3deg); border-color: #aa5a3a; box-shadow: 0 0 25px rgba(170, 90, 58, 0.5); }
        .service-card:hover .service-icon { transform: scale(1.1); color: #d47a4e; }
        .service-card h4 { font-size: 1.3rem; font-weight: 600; margin-bottom: 12px; color: #e0cfb0; }
        .service-card p { color: #b8aa9a; margin-bottom: 18px; font-size: 0.85rem; }
        .price-ls { font-weight: 500; font-size: 0.8rem; color: #bc6f4a; background: rgba(170, 90, 58, 0.15); display: inline-block; padding: 6px 16px; border-radius: 40px; transition: all 0.3s; }
        .service-card:hover .price-ls { background: rgba(170, 90, 58, 0.3); box-shadow: 0 0 12px rgba(170, 90, 58, 0.4); }
        .warning-note { background: rgba(15, 15, 25, 0.6); backdrop-filter: blur(8px); border-left: 3px solid #aa5a3a; padding: 22px 32px; border-radius: 20px; margin-top: 50px; font-size: 0.85rem; color: #b8aa9a; text-align: center; }
        .imp-story { padding: 80px 0; background: linear-gradient(135deg, rgba(10, 5, 15, 0.9), rgba(3, 3, 10, 0.95)); border-top: 1px solid rgba(170, 90, 58, 0.3); border-bottom: 1px solid rgba(170, 90, 58, 0.3); }
        .story-grid { display: grid; grid-template-columns: 1fr; gap: 50px; align-items: center; }
        @media (min-width: 900px) { .story-grid { grid-template-columns: 0.8fr 1.2fr; } }
        .story-avatar { display: flex; justify-content: center; align-items: center; }
        .avatar-container { position: relative; width: 280px; height: 280px; }
        .story-imp-svg { width: 100%; height: 100%; filter: drop-shadow(0 0 20px rgba(170, 90, 58, 0.6)); animation: impFloat 3s ease-in-out infinite; cursor: pointer; }
        @keyframes impFloat { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }
        .story-content { text-align: center; }
        @media (min-width: 900px) { .story-content { text-align: left; } }
        .story-badge { display: inline-block; background: rgba(170, 90, 58, 0.2); padding: 6px 16px; border-radius: 40px; font-size: 0.75rem; font-weight: 600; color: #ff8866; margin-bottom: 20px; border: 1px solid rgba(170, 90, 58, 0.4); }
        .story-content h3 { font-size: 1.8rem; font-weight: 700; margin: 20px 0 16px; background: linear-gradient(135deg, #e0cfb0, #bc6f4a); -webkit-background-clip: text; background-clip: text; color: transparent; }
        .story-content p { color: #b8aa9a; font-size: 0.95rem; line-height: 1.6; margin-bottom: 18px; }
        .story-divider { width: 60px; height: 2px; background: linear-gradient(90deg, #aa5a3a, transparent); margin: 25px 0; }
        .story-fact { background: rgba(170, 90, 58, 0.1); border-left: 3px solid #aa5a3a; padding: 18px 22px; border-radius: 16px; margin: 25px 0; display: flex; gap: 12px; align-items: flex-start; }
        .story-fact i { font-size: 24px; color: #aa5a3a; }
        .story-fact span { color: #d0c0aa; font-size: 0.85rem; }
        .features { padding: 90px 0; background: rgba(10, 10, 18, 0.6); backdrop-filter: blur(8px); border-top: 1px solid rgba(170, 90, 58, 0.2); border-bottom: 1px solid rgba(170, 90, 58, 0.2); }
        .feature-list { display: flex; flex-wrap: wrap; justify-content: center; gap: 50px; margin-top: 50px; }
        .feature-item { text-align: center; max-width: 200px; transition: all 0.3s; }
        .feature-item:hover { transform: translateY(-8px); }
        .feature-item i { font-size: 42px; background: rgba(170, 90, 58, 0.15); padding: 20px; border-radius: 50%; color: #aa5a3a; margin-bottom: 18px; display: inline-block; transition: all 0.3s; }
        .feature-item:hover i { background: rgba(170, 90, 58, 0.3); box-shadow: 0 0 25px rgba(170, 90, 58, 0.4); }
        .feature-item h4 { font-size: 1rem; font-weight: 600; margin-bottom: 8px; color: #e0cfb0; }
        .feature-item p { font-size: 0.75rem; color: #9a8a76; }
        .reviews-channel { padding: 70px 0; background: #03030a; }
        .channel-card { background: rgba(15, 15, 25, 0.7); backdrop-filter: blur(12px); border-radius: 32px; padding: 48px 32px; text-align: center; border: 1px solid rgba(170, 90, 58, 0.4); transition: all 0.4s; max-width: 700px; margin: 0 auto; }
        .channel-card:hover { transform: translateY(-8px); border-color: #aa5a3a; box-shadow: 0 0 30px rgba(170, 90, 58, 0.3); }
        .channel-icon { font-size: 58px; color: #aa5a3a; margin-bottom: 20px; }
        .channel-card h3 { font-size: 1.8rem; font-weight: 700; margin-bottom: 16px; background: linear-gradient(135deg, #e0cfb0, #bc6f4a); -webkit-background-clip: text; background-clip: text; color: transparent; }
        .channel-card p { color: #b8aa9a; font-size: 1rem; margin-bottom: 28px; }
        .channel-btn { display: inline-flex; align-items: center; gap: 12px; background: rgba(170, 90, 58, 0.2); padding: 14px 36px; border-radius: 60px; text-decoration: none; font-weight: 600; font-size: 1rem; color: #e0cfb0; transition: all 0.3s; border: 1px solid #aa5a3a; }
        .channel-btn:hover { transform: scale(1.03); box-shadow: 0 0 25px rgba(170, 90, 58, 0.5); background: rgba(170, 90, 58, 0.35); }
        .contact { background: #03030a; padding: 90px 0; }
        .contact-flex { display: flex; flex-direction: column; gap: 45px; }
        @media (min-width: 768px) { .contact-flex { flex-direction: row; justify-content: space-between; align-items: center; } .contact-text { text-align: left; flex: 1; } .contact-btn { margin: 0; } }
        .contact-text { text-align: center; }
        .contact-text h3 { font-size: 1.8rem; font-weight: 700; margin-bottom: 15px; color: #e0cfb0; }
        .contact-text p { color: #b8aa9a; font-size: 0.95rem; }
        .managers-list { margin-top: 35px; background: rgba(15, 15, 25, 0.6); backdrop-filter: blur(8px); padding: 32px 35px; border-radius: 24px; border: 1px solid rgba(170, 90, 58, 0.3); }
        .managers-list h4 { font-size: 0.9rem; font-weight: 600; margin-bottom: 20px; color: #bc6f4a; text-align: center; }
        @media (min-width: 768px) { .managers-list h4 { text-align: left; } .manager-tags { justify-content: flex-start; } }
        .manager-tags { display: flex; flex-wrap: wrap; justify-content: center; gap: 18px; }
        .manager-tag { background: rgba(10, 10, 20, 0.6); padding: 10px 22px; border-radius: 40px; font-size: 0.85rem; font-weight: 500; display: inline-flex; align-items: center; gap: 8px; text-decoration: none; color: #cdc6bc; border: 1px solid rgba(170, 90, 58, 0.3); transition: all 0.3s; }
        .manager-tag:hover { background: rgba(170, 90, 58, 0.2); color: #bc6f4a; border-color: #aa5a3a; transform: translateY(-3px); }
        .owner-badge { border-color: #aa5a3a; }
        .contact-btn { background: rgba(170, 90, 58, 0.15); padding: 14px 38px; border-radius: 50px; text-decoration: none; font-weight: 600; font-size: 0.95rem; color: #e0cfb0; display: inline-block; border: 1px solid #aa5a3a; text-align: center; width: fit-content; margin: 0 auto; transition: all 0.3s; position: relative; overflow: hidden; }
        .contact-btn:hover { background: rgba(170, 90, 58, 0.3); box-shadow: 0 0 30px rgba(170, 90, 58, 0.5); transform: translateY(-2px); }
        .legal-notice { background: rgba(15, 15, 25, 0.5); backdrop-filter: blur(8px); border: 1px solid rgba(170, 90, 58, 0.2); border-radius: 20px; padding: 30px 35px; margin: 50px 0 25px; font-size: 0.7rem; color: #9a8a76; }
        .legal-notice h4 { color: #bc6f4a; margin-bottom: 18px; font-size: 0.85rem; }
        footer { background: #03030a; color: #7a6a5a; text-align: center; padding: 35px; font-size: 0.75rem; border-top: 1px solid rgba(170, 90, 58, 0.2); }
        
        /* Стили для улучшенной игры */
        .game-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.95); backdrop-filter: blur(8px); z-index: 3000; display: none; justify-content: center; align-items: center; font-family: 'Inter', monospace; }
        .game-container { background: linear-gradient(135deg, #0a0a15, #03030a); border: 2px solid #aa5a3a; border-radius: 32px; padding: 30px; max-width: 650px; width: 90%; text-align: center; position: relative; box-shadow: 0 0 50px rgba(170, 90, 58, 0.5); animation: gameGlow 1s ease-in-out infinite; }
        @keyframes gameGlow { 0%, 100% { box-shadow: 0 0 20px rgba(170, 90, 58, 0.3); } 50% { box-shadow: 0 0 50px rgba(170, 90, 58, 0.7); } }
        .game-title { font-size: 1.8rem; font-weight: 700; background: linear-gradient(135deg, #ff8866, #aa5a3a); -webkit-background-clip: text; background-clip: text; color: transparent; margin-bottom: 15px; }
        .game-stats-bar { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 10px; margin: 10px 0; padding: 10px; background: rgba(0,0,0,0.5); border-radius: 20px; }
        .game-level, .game-score, .game-combo, .game-best { font-size: 0.9rem; color: #ff8866; }
        .game-level span, .game-score span, .game-combo span, .game-best span { color: #e0cfb0; font-size: 1.2rem; font-weight: bold; }
        .game-arena { background: rgba(0, 0, 0, 0.6); border: 2px solid #aa5a3a; border-radius: 20px; height: 400px; position: relative; margin: 20px 0; overflow: hidden; cursor: crosshair; }
        .game-imp, .fake-imp, .golden-imp, .trap { position: absolute; width: 60px; height: 60px; cursor: pointer; transition: all 0.05s linear; }
        .game-imp { filter: drop-shadow(0 0 10px #ff4422); z-index: 10; }
        .golden-imp { filter: drop-shadow(0 0 15px gold); z-index: 10; animation: goldenPulse 0.5s ease-in-out infinite; }
        @keyframes goldenPulse { 0%, 100% { filter: drop-shadow(0 0 10px gold); transform: scale(1); } 50% { filter: drop-shadow(0 0 25px #ffaa00); transform: scale(1.05); } }
        .fake-imp { filter: drop-shadow(0 0 5px #884422); opacity: 0.7; }
        .trap { filter: drop-shadow(0 0 8px #aa2222); animation: trapShake 0.3s ease-in-out infinite; cursor: pointer; }
        @keyframes trapShake { 0%, 100% { transform: translateX(0); } 25% { transform: translateX(-3px); } 75% { transform: translateX(3px); } }
        .game-timer { font-size: 1.2rem; font-weight: bold; color: #ff8866; background: rgba(0,0,0,0.6); padding: 5px 12px; border-radius: 20px; display: inline-block; margin: 5px; }
        .game-message { font-size: 0.85rem; color: #b8aa9a; margin: 10px 0; min-height: 50px; font-weight: bold; }
        .game-btn { background: rgba(170, 90, 58, 0.2); border: 1px solid #aa5a3a; padding: 10px 25px; border-radius: 40px; color: #ff8866; font-weight: 600; cursor: pointer; transition: all 0.3s; margin: 5px; }
        .game-btn:hover { background: rgba(170, 90, 58, 0.5); transform: scale(1.05); box-shadow: 0 0 15px rgba(170, 90, 58, 0.5); }
        .hit-animation { animation: impJump 0.2s ease-in-out; }
        @keyframes impJump { 0% { transform: scale(1); } 50% { transform: scale(1.3); filter: brightness(1.5); } 100% { transform: scale(1); } }
        .screen-shake { animation: shake 0.3s ease-in-out; }
        @keyframes shake { 0%, 100% { transform: translateX(0); } 25% { transform: translateX(-5px); } 75% { transform: translateX(5px); } }
        .discount-badge { position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); background: linear-gradient(135deg, #aa5a3a, #ff3300); color: white; padding: 20px 40px; border-radius: 20px; font-size: 2rem; font-weight: bold; z-index: 2000; animation: discountPulse 0.5s ease-out; box-shadow: 0 0 50px rgba(255, 51, 0, 0.8); text-align: center; white-space: nowrap; font-family: monospace; }
        @keyframes discountPulse { 0% { transform: translate(-50%, -50%) scale(0); opacity: 0; } 50% { transform: translate(-50%, -50%) scale(1.2); } 100% { transform: translate(-50%, -50%) scale(1); opacity: 1; } }
        
        /* Бес-гид */
        .imp-guide { position: fixed; bottom: 30px; right: 30px; width: 100px; height: 100px; cursor: pointer; z-index: 1000; display: none; filter: drop-shadow(0 0 10px rgba(170, 90, 58, 0.5)); animation: bounceGuide 2s ease-in-out infinite; transition: all 0.3s; }
        .imp-guide:hover { transform: scale(1.1); filter: drop-shadow(0 0 20px rgba(255, 80, 40, 0.8)); }
        @keyframes bounceGuide { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-8px); } }
        .imp-tooltip { position: absolute; bottom: 110px; right: 0; background: rgba(0, 0, 0, 0.95); backdrop-filter: blur(10px); padding: 8px 16px; border-radius: 25px; font-size: 0.7rem; font-weight: 500; color: #ff8866; white-space: nowrap; border: 1px solid #aa5a3a; opacity: 0; transition: opacity 0.3s; pointer-events: none; font-family: monospace; }
        .imp-guide:hover .imp-tooltip { opacity: 1; }
        .chaos-mode { animation: spinHead 0.2s linear infinite !important; }
        @keyframes spinHead { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    </style>
</head>
<body>
    <div class="smoke-container" id="smokeContainer"></div>
    <div class="particles" id="particles"></div>

    <!-- Бес-гид плавающий -->
    <div class="imp-guide" id="impGuide">
        <svg viewBox="0 0 100 100" style="width: 100%; height: 100%;">
            <defs>
                <radialGradient id="impBodyDark" cx="50%" cy="50%" r="50%"><stop offset="0%" stop-color="#5a2a2a"/><stop offset="100%" stop-color="#2a0a0a"/></radialGradient>
                <radialGradient id="impFace" cx="40%" cy="40%" r="60%"><stop offset="0%" stop-color="#3a1a1a"/><stop offset="100%" stop-color="#1a0505"/></radialGradient>
                <linearGradient id="hornGradient" x1="0%" y1="0%" x2="100%" y2="0%"><stop offset="0%" stop-color="#aa5a3a"/><stop offset="100%" stop-color="#6a2a1a"/></linearGradient>
            </defs>
            <ellipse cx="50" cy="85" rx="35" ry="12" fill="rgba(0,0,0,0.5)" opacity="0.5"/>
            <path d="M 35 55 L 35 75 Q 35 82 42 83 L 58 83 Q 65 82 65 75 L 65 55 Q 65 48 58 48 L 42 48 Q 35 48 35 55 Z" fill="url(#impBodyDark)" stroke="#aa5a3a" stroke-width="1.5"/>
            <path d="M 45 58 L 50 62 L 55 58" stroke="#ff6644" stroke-width="2" fill="none" opacity="0.7"/>
            <circle cx="50" cy="32" r="22" fill="url(#impFace)" stroke="#aa5a3a" stroke-width="2"/>
            <path d="M 35 25 L 42 28 M 65 25 L 58 28" stroke="#ff8866" stroke-width="3" stroke-linecap="round" fill="none"/>
            <path d="M 32 18 L 22 5 L 32 14" fill="url(#hornGradient)" stroke="#cc6633" stroke-width="1.5"/>
            <path d="M 68 18 L 78 5 L 68 14" fill="url(#hornGradient)" stroke="#cc6633" stroke-width="1.5"/>
            <circle cx="38" cy="31" r="5" fill="#ff3300" opacity="0.9"><animate attributeName="r" values="5;5.5;5" dur="1s" repeatCount="indefinite"/></circle>
            <circle cx="62" cy="31" r="5" fill="#ff3300" opacity="0.9"><animate attributeName="r" values="5;5.5;5" dur="1s" repeatCount="indefinite"/></circle>
            <ellipse cx="38" cy="31" rx="2.2" ry="3.5" fill="black"/>
            <ellipse cx="62" cy="31" rx="2.2" ry="3.5" fill="black"/>
            <path d="M 44 44 L 40 52 L 46 48" fill="#f0e0c0" stroke="#aa5a3a" stroke-width="1"/>
            <path d="M 56 44 L 60 52 L 54 48" fill="#f0e0c0" stroke="#aa5a3a" stroke-width="1"/>
            <path d="M 42 42 Q 50 48 58 42" stroke="#ff8866" stroke-width="2.5" fill="none" stroke-linecap="round"/>
            <circle cx="44" cy="38" r="2.5" fill="rgba(170,90,58,0.5)"><animate attributeName="r" values="2.5;4;2.5" dur="1.2s" repeatCount="indefinite"/></circle>
            <circle cx="56" cy="38" r="2.5" fill="rgba(170,90,58,0.5)"><animate attributeName="r" values="2.5;4;2.5" dur="1.2s" repeatCount="indefinite"/></circle>
        </svg>
        <div class="imp-tooltip" id="impTooltip">😈 ЖМИ НА МЕНЯ! 😈</div>
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
                <a href="#" class="btn-outline" id="gameLauncher">🎮 Игра на скидку</a>
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
                        <div class="stat-item"><i class="fas fa-eye-slash"></i> анонимность<span>полная конфиденциальность</span></div>
                    </div>
                </div>
                <div class="hero-image animate-on-scroll">
                    <div class="demon-eye-container">
                        <svg class="demon-eye" viewBox="0 0 200 200" id="movingEye">
                            <defs>
                                <radialGradient id="eyeBg" cx="50%" cy="50%" r="50%"><stop offset="0%" stop-color="#1a0508"/><stop offset="100%" stop-color="#030101"/></radialGradient>
                                <radialGradient id="irisGrad" cx="45%" cy="45%" r="50%"><stop offset="0%" stop-color="#ff4422"/><stop offset="70%" stop-color="#aa2200"/><stop offset="100%" stop-color="#4a0a00"/></radialGradient>
                                <radialGradient id="pupilGrad" cx="50%" cy="50%" r="50%"><stop offset="0%" stop-color="#000000"/><stop offset="100%" stop-color="#220000"/></radialGradient>
                            </defs>
                            <ellipse cx="100" cy="100" rx="85" ry="92" fill="url(#eyeBg)" stroke="#aa5a3a" stroke-width="2"/>
                            <path d="M 45 65 L 55 72 L 48 82" stroke="#aa3a2a" stroke-width="2" fill="none" opacity="0.6"><animate attributeName="opacity" values="0.4;0.8;0.4" dur="3s" repeatCount="indefinite"/></path>
                            <path d="M 155 65 L 145 72 L 152 82" stroke="#aa3a2a" stroke-width="2" fill="none" opacity="0.6"><animate attributeName="opacity" values="0.4;0.8;0.4" dur="3s" repeatCount="indefinite"/></path>
                            <ellipse cx="100" cy="100" rx="48" ry="55" fill="url(#irisGrad)" stroke="#ff6644" stroke-width="1.5"><animate attributeName="rx" values="48;50;48" dur="2s" repeatCount="indefinite"/><animate attributeName="ry" values="55;57;55" dur="2s" repeatCount="indefinite"/></ellipse>
                            <ellipse id="movingPupil" cx="100" cy="100" rx="20" ry="32" fill="url(#pupilGrad)" stroke="#ff3300" stroke-width="1"><animate attributeName="rx" values="20;18;22;20" dur="2.5s" repeatCount="indefinite"/><animate attributeName="ry" values="32;35;30;32" dur="2.5s" repeatCount="indefinite"/></ellipse>
                            <circle cx="100" cy="100" r="38" fill="none" stroke="#ff4422" stroke-width="1" opacity="0.5"><animate attributeName="r" values="38;43;38" dur="1.5s" repeatCount="indefinite"/></circle>
                            <ellipse cx="100" cy="100" rx="95" ry="102" fill="none" stroke="#aa5a3a" stroke-width="1" stroke-dasharray="6 6"><animate attributeName="rx" values="95;98;95" dur="3s" repeatCount="indefinite"/></ellipse>
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
                    <p>Каждый ритуал сопровождается обязательной платной диагностикой и индивидуальным подходом. Работаем только через Telegram, гарантируем полную анонимность и соблюдение сроков.</p>
                    <div class="about-stats"><div class="about-stat"><h4>5 лет</h4><p>практики с бесами</p></div><div class="about-stat"><h4>1000+</h4><p>успешных обрядов</p></div><div class="about-stat"><h4>Бесовые князи</h4><p>высший уровень</p></div></div>
                </div>
            </div>
        </div>

        <div class="terms" id="terms">
            <div class="container"><div class="section-header animate-on-scroll"><h3>Условия работы</h3><p>Порядок проведения ритуалов и стоимость</p></div>
                <div class="terms-grid">
                    <div class="term-card"><div class="term-icon"><i class="fas fa-stethoscope"></i></div><h4>Диагностика</h4><p>Обязательная платная диагностика перед любым ритуалом.</p><div class="price-highlight">2 500 ₽</div></div>
                    <div class="term-card"><div class="term-icon"><i class="fas fa-calendar-check"></i></div><h4>Сроки выполнения</h4><p>Работа будет поставлена в день, когда всё будет обговорено.</p></div>
                    <div class="term-card"><div class="term-icon"><i class="fas fa-gem"></i></div><h4>Цены на ритуалы</h4><p>После платной диагностики. Цены индивидуальны.</p><div class="price-highlight">индивидуально</div></div>
                </div>
            </div>
        </div>

        <!-- Блок Бес-гид -->
        <div class="imp-story">
            <div class="container">
                <div class="story-grid">
                    <div class="story-avatar animate-on-scroll">
                        <div class="avatar-container">
                            <svg viewBox="0 0 200 200" class="story-imp-svg">
                                <defs>
                                    <radialGradient id="storyImpBody" cx="50%" cy="50%" r="50%"><stop offset="0%" stop-color="#6a2a2a"/><stop offset="100%" stop-color="#2a0a0a"/></radialGradient>
                                    <radialGradient id="storyImpFace" cx="40%" cy="40%" r="60%"><stop offset="0%" stop-color="#4a2a2a"/><stop offset="100%" stop-color="#1a0505"/></radialGradient>
                                </defs>
                                <circle cx="100" cy="100" r="95" fill="none" stroke="#aa5a3a" stroke-width="1" stroke-dasharray="5 5" opacity="0.5"><animate attributeName="r" values="95;98;95" dur="3s" repeatCount="indefinite"/></circle>
                                <path d="M 70 110 L 70 150 Q 70 165 85 166 L 115 166 Q 130 165 130 150 L 130 110 Q 130 95 115 95 L 85 95 Q 70 95 70 110 Z" fill="url(#storyImpBody)" stroke="#aa5a3a" stroke-width="2"/>
                                <circle cx="100" cy="65" r="35" fill="url(#storyImpFace)" stroke="#aa5a3a" stroke-width="2.5"/>
                                <path d="M 65 40 L 45 10 L 65 30" fill="#aa5a3a" stroke="#cc6633" stroke-width="2"/>
                                <path d="M 135 40 L 155 10 L 135 30" fill="#aa5a3a" stroke="#cc6633" stroke-width="2"/>
                                <circle cx="75" cy="60" r="8" fill="#ff4422"><animate attributeName="r" values="8;9;8" dur="1s" repeatCount="indefinite"/></circle>
                                <circle cx="125" cy="60" r="8" fill="#ff4422"><animate attributeName="r" values="8;9;8" dur="1s" repeatCount="indefinite"/></circle>
                                <ellipse cx="75" cy="60" rx="3" ry="5" fill="black"/>
                                <ellipse cx="125" cy="60" rx="3" ry="5" fill="black"/>
                                <path d="M 85 88 L 78 100 L 88 94" fill="#f0e0c0" stroke="#aa5a3a" stroke-width="1.5"/>
                                <path d="M 115 88 L 122 100 L 112 94" fill="#f0e0c0" stroke="#aa5a3a" stroke-width="1.5"/>
                                <path d="M 85 85 Q 100 95 115 85" stroke="#ff8866" stroke-width="3" fill="none"/>
                                <circle cx="100" cy="92" r="6" fill="rgba(170,90,58,0.5)"><animate attributeName="r" values="6;10;6" dur="1.5s" repeatCount="indefinite"/></circle>
                            </svg>
                            <div class="avatar-glow"></div>
                        </div>
                    </div>
                    <div class="story-content animate-on-scroll">
                        <div class="story-badge">🔥 БЕС-ГИД 🔥</div>
                        <h3>Кто такой этот бесёнок?</h3>
                        <p>— А вот и я, собственной персоной! <strong>Маленький, злой, но справедливый бес-гид</strong>. Меня приставили к этому сайту, чтобы всякие сомневающиеся не убегали, а сразу задавали вопросы.</p>
                        <p>Я тут главный по <strong>навигации, подсказкам и внезапным скидкам</strong>. Жми на меня или на кнопку «Игра на скидку» — испытай удачу!</p>
                        <div class="story-divider"></div>
                        <h3>📜 История «Окоянного дитя»</h3>
                        <p>Началось всё <strong>пять лет назад</strong> в глухой деревне, где старуха-знахарка передала свои знания <strong>тому</strong>, кто оказался способен видеть <strong>мир мёртвых и бесов</strong>. Со временем практика выросла в мощный канал работы с <strong>семиотрядными бесами, бесовыми князьями и духами умерших</strong>.</p>
                        <div class="story-fact"><i class="fas fa-fire"></i><span><strong>Факт:</strong> Самый нетерпеливый клиент тыкал меня 47 раз. На 48-й я скинул скидку 30% просто чтобы отстал!</span></div>
                    </div>
                </div>
            </div>
        </div>

        <div class="services" id="services">
            <div class="container"><div class="section-header animate-on-scroll"><h3>Перечень услуг</h3><p>Все ритуалы проводятся только после платной диагностики.</p></div>
                <div class="services-grid">
                    <div class="service-card"><div class="service-icon-wrapper"><i class="fas fa-heart-broken service-icon"></i></div><h4>Присушка</h4><p>Любовная привязка на тоску и влечение.</p><div class="price-ls">цена после диагностики</div></div>
                    <div class="service-card"><div class="service-icon-wrapper"><i class="fas fa-link service-icon"></i></div><h4>Бесовская привязка</h4><p>Крепкая привязка человека к вам.</p><div class="price-ls">цена после диагностики</div></div>
                    <div class="service-card"><div class="service-icon-wrapper"><i class="fas fa-eye service-icon"></i></div><h4>Диагностика магических способностей</h4><p>Проверка вашего канала, видят ли бесы, сила рода.</p><div class="price-ls">2 500 ₽</div></div>
                    <div class="service-card"><div class="service-icon-wrapper"><i class="fas fa-skull service-icon"></i></div><h4>Порча через семиотрядных бесов</h4><p>Мощный ритуал на поражение врага.</p><div class="price-ls">цена после диагностики</div></div>
                    <div class="service-card"><div class="service-icon-wrapper"><i class="fas fa-ghost service-icon"></i></div><h4>Работа с миром мёртвых</h4><p>Вызов духов умерших, родовые вопросы.</p><div class="price-ls">цена после диагностики</div></div>
                    <div class="service-card"><div class="service-icon-wrapper"><i class="fas fa-chalkboard-user service-icon"></i></div><h4>Расклады Таро</h4><p>Диагностика ситуации, просмотр отношений.</p><div class="price-ls">цена после диагностики</div></div>
                </div>
                <div class="warning-note"><i class="fas fa-info-circle"></i> <strong>Важно:</strong> Все ритуалы только после платной диагностики (2500 ₽). Диагностика магических способностей — 2500 ₽.</div>
            </div>
        </div>

        <div class="features"><div class="container"><div class="section-header"><h3>Преимущества</h3><p>Почему выбирают нас</p></div><div class="feature-list"><div class="feature-item"><i class="fas fa-cat"></i><h4>Работа с бесами</h4><p>Мелкие бесы и князи</p></div><div class="feature-item"><i class="fas fa-user-secret"></i><h4>Анонимность</h4><p>Полная конфиденциальность</p></div><div class="feature-item"><i class="fas fa-chart-line"></i><h4>Без отката</h4><p>Защита на каждый обряд</p></div></div></div></div>

        <div class="reviews-channel"><div class="container"><div class="channel-card"><div class="channel-icon"><i class="fab fa-telegram"></i></div><h3>Канал с отзывами</h3><p>Реальные истории клиентов, результаты ритуалов</p><a href="https://t.me/okoyanny" target="_blank" class="channel-btn"><i class="fab fa-telegram"></i> Перейти в канал</a><div class="channel-footer">@okoyanny</div></div></div></div>

        <div class="contact" id="contact"><div class="container contact-flex"><div class="contact-text"><h3>Связаться</h3><p>Telegram — связь с владельцем и менеджерами. Диагностика — 2 500 ₽.</p><div class="managers-list"><h4><i class="fas fa-user-circle"></i> Контакты:</h4><div class="manager-tags"><a href="https://t.me/Zara_zzaww" target="_blank" class="manager-tag owner-badge"><i class="fab fa-telegram"></i> @Zara_zzaww — владелец</a><a href="https://t.me/Yfcghuuuuuu" target="_blank" class="manager-tag"><i class="fab fa-telegram"></i> @Yfcghuuuuuu — менеджер</a><a href="https://t.me/kinght11111" target="_blank" class="manager-tag"><i class="fab fa-telegram"></i> @kinght11111 — менеджер</a></div><div class="divider"></div><p style="font-size: 0.75rem; margin-top: 16px;">Ответ в течение часа. Диагностика — 2 500 ₽</p></div></div><a href="https://t.me/Zara_zzaww" target="_blank" class="contact-btn">Написать владельцу</a></div></div>

        <div class="container"><div class="legal-notice"><h4>📜 ОФИЦИАЛЬНОЕ УВЕДОМЛЕНИЕ</h4><p>Все материалы носят информационно-просветительский характер. 18+</p></div></div>
    </main>

    <footer><div class="container"><p>© 2026 Окоянное дитя — бесовские ритуалы. Все обряды 18+.</p></div></footer>

    <!-- Улучшенная игра -->
    <div class="game-overlay" id="gameOverlay">
        <div class="game-container">
            <div class="game-title">🎯 ПОЙМАЙ БЕСА! 🎯</div>
            <div class="game-stats-bar">
                <div class="game-level">Уровень: <span id="gameLevel">1</span> / 5</div>
                <div class="game-score">Счёт: <span id="gameScore">0</span> / <span id="gameTarget">5</span></div>
                <div class="game-combo">Комбо: <span id="gameCombo">0</span>x</div>
                <div class="game-best">Рекорд: <span id="gameBest">0</span></div>
            </div>
            <div class="game-arena" id="gameArena"></div>
            <div class="game-timer" id="gameTimer">⏱️ 3.0с</div>
            <div class="game-message" id="gameMessage">🔥 Лови беса! Золотой даёт x2 очка! 🔥</div>
            <div><button class="game-btn" id="gameStartBtn">НАЧАТЬ ИГРУ</button><button class="game-btn" id="gameCloseBtn">ЗАКРЫТЬ</button></div>
        </div>
    </div>

    <script>
        // Эффекты
        function createParticles() { const container = document.getElementById('particles'); for (let i = 0; i < 50; i++) { const p = document.createElement('div'); p.classList.add('particle'); p.style.width = (Math.random() * 5 + 2) + 'px'; p.style.height = p.style.width; p.style.left = Math.random() * 100 + '%'; p.style.animationDuration = Math.random() * 15 + 8 + 's'; p.style.animationDelay = Math.random() * 15 + 's'; p.style.background = `rgba(170, 90, 58, ${Math.random() * 0.4 + 0.1})`; container.appendChild(p); } }
        function createSmoke() { setInterval(() => { const smoke = document.createElement('div'); smoke.classList.add('smoke'); smoke.style.left = Math.random() * 100 + '%'; smoke.style.animationDuration = Math.random() * 8 + 6 + 's'; document.getElementById('smokeContainer').appendChild(smoke); setTimeout(() => smoke.remove(), 12000); }, 3000); }
        createParticles(); createSmoke();
        
        const animateElements = document.querySelectorAll('.animate-on-scroll');
        const checkVisibility = () => { animateElements.forEach(el => { if (el.getBoundingClientRect().top < window.innerHeight - 100) el.classList.add('visible'); }); };
        window.addEventListener('scroll', checkVisibility);
        window.addEventListener('load', checkVisibility);
        
        // Движущийся глаз
        const eyeSvg = document.getElementById('movingEye');
        const pupil = document.getElementById('movingPupil');
        if (eyeSvg && pupil) {
            eyeSvg.addEventListener('mousemove', (e) => { const rect = eyeSvg.getBoundingClientRect(); const x = (e.clientX - rect.left) / rect.width * 200; const y = (e.clientY - rect.top) / rect.height * 200; pupil.setAttribute('cx', Math.min(Math.max(x, 80), 120)); pupil.setAttribute('cy', Math.min(Math.max(y, 80), 120)); });
            eyeSvg.addEventListener('mouseleave', () => { pupil.setAttribute('cx', 100); pupil.setAttribute('cy', 100); });
        }
        
        // Бес-гид
        setTimeout(() => { const imp = document.getElementById('impGuide'); if (imp) { imp.style.display = 'block'; imp.style.opacity = '0'; imp.style.transform = 'scale(0) rotate(180deg)'; imp.style.transition = 'all 0.5s cubic-bezier(0.68, -0.55, 0.265, 1.55)'; setTimeout(() => { imp.style.opacity = '1'; imp.style.transform = 'scale(1) rotate(0deg)'; }, 50); } }, 2000);
        
        const impGuide = document.getElementById('impGuide');
        const impTooltip = document.getElementById('impTooltip');
        const gameLauncher = document.getElementById('gameLauncher');
        const gameOverlay = document.getElementById('gameOverlay');
        const messages = ["😈 А ну, давай в игру!", "🔥 Жми на кнопку \"Игра на скидку\"!", "🎮 Поймай меня 5 раз — получи скидку!", "⚡ Быстрее, пока я не передумал!", "👹 Золотой бес даёт x2 очка!", "💀 Ловушки отнимают время!", "🎯 Кликай на меня в игре!", "😈 АГА! СЛАБО ПОЙМАТЬ?", "🔥 ДАВАЙ, ЖМИ НА КНОПКУ!"];
        let clickCount = 0;
        function showMessage() { const randomMsg = messages[Math.floor(Math.random() * messages.length)]; impTooltip.textContent = randomMsg; impTooltip.style.opacity = '1'; impTooltip.style.transform = 'scale(1.1)'; setTimeout(() => { impTooltip.style.transform = 'scale(1)'; setTimeout(() => { if (!impGuide.matches(':hover')) impTooltip.style.opacity = '0'; }, 1500); }, 200); }
        function launchGame() { gameOverlay.style.display = 'flex'; resetGame(); impTooltip.textContent = "🎮 УДАЧИ! ЛОВИ БЕСА! 🎮"; impTooltip.style.opacity = '1'; setTimeout(() => { if (!impGuide.matches(':hover')) impTooltip.style.opacity = '0'; }, 2000); }
        impGuide.addEventListener('click', (e) => { e.stopPropagation(); clickCount++; impGuide.style.transform = 'scale(0.95)'; setTimeout(() => { impGuide.style.transform = 'scale(1)'; }, 150); showMessage(); if (clickCount >= 2) { launchGame(); clickCount = 0; } });
        gameLauncher.addEventListener('click', (e) => { e.preventDefault(); launchGame(); });
        
        // ИГРА
        const gameArena = document.getElementById('gameArena');
        const gameScoreEl = document.getElementById('gameScore');
        const gameLevelEl = document.getElementById('gameLevel');
        const gameTimerEl = document.getElementById('gameTimer');
        const gameMessage = document.getElementById('gameMessage');
        const gameTarget = document.getElementById('gameTarget');
        const gameComboEl = document.getElementById('gameCombo');
        const gameBestEl = document.getElementById('gameBest');
        
        let gameActive = false;
        let currentLevel = 1;
        let currentScore = 0;
        let currentCombo = 0;
        let bestScore = localStorage.getItem('gameBestScore') || 0;
        let currentImp = null;
        let currentFakes = [];
        let currentTraps = [];
        let goldenImp = null;
        let moveInterval = null;
        let timerInterval = null;
        let timeLeft = 3;
        let discountGiven = false;
        gameBestEl.textContent = bestScore;
        
        const impSvg = `<svg viewBox="0 0 60 60"><circle cx="30" cy="35" r="18" fill="#5a2a2a" stroke="#aa5a3a"/><circle cx="30" cy="22" r="12" fill="#3a1a1a"/><path d="M 20 15 L 12 5 L 20 12" fill="#aa5a3a"/><path d="M 40 15 L 48 5 L 40 12" fill="#aa5a3a"/><circle cx="22" cy="20" r="3" fill="#ff3300"/><circle cx="38" cy="20" r="3" fill="#ff3300"/><ellipse cx="22" cy="20" rx="1.5" ry="2.5" fill="black"/><ellipse cx="38" cy="20" rx="1.5" ry="2.5" fill="black"/><path d="M 24 30 Q 30 35 36 30" stroke="#ff8866" stroke-width="2" fill="none"/><path d="M 27 35 L 24 41 L 30 37" fill="#f0e0c0"/><path d="M 33 35 L 36 41 L 30 37" fill="#f0e0c0"/></svg>`;
        const goldenSvg = `<svg viewBox="0 0 60 60"><circle cx="30" cy="35" r="18" fill="#aa8833" stroke="#ffaa44"/><circle cx="30" cy="22" r="12" fill="#886622"/><path d="M 20 15 L 12 5 L 20 12" fill="#ffaa44"/><path d="M 40 15 L 48 5 L 40 12" fill="#ffaa44"/><circle cx="22" cy="20" r="3" fill="#ffcc66"/><circle cx="38" cy="20" r="3" fill="#ffcc66"/><ellipse cx="22" cy="20" rx="1.5" ry="2.5" fill="black"/><ellipse cx="38" cy="20" rx="1.5" ry="2.5" fill="black"/><path d="M 24 30 Q 30 35 36 30" stroke="#ffcc66" stroke-width="2"/><path d="M 27 35 L 24 41 L 30 37" fill="#ffcc88"/><path d="M 33 35 L 36 41 L 30 37" fill="#ffcc88"/></svg>`;
        const fakeSvg = `<svg viewBox="0 0 60 60"><circle cx="30" cy="35" r="16" fill="#3a2a2a" stroke="#886644"/><circle cx="30" cy="22" r="10" fill="#2a1a1a"/><path d="M 22 16 L 16 8 L 22 14" fill="#886644"/><path d="M 38 16 L 44 8 L 38 14" fill="#886644"/><circle cx="24" cy="20" r="2" fill="#aa6644"/><circle cx="36" cy="20" r="2" fill="#aa6644"/><path d="M 26 28 Q 30 32 34 28" stroke="#aa8866"/></svg>`;
        const trapSvg = `<svg viewBox="0 0 60 60"><circle cx="30" cy="35" r="18" fill="#442222" stroke="#aa3333"/><text x="30" y="42" font-size="28" text-anchor="middle" fill="#aa3333" font-weight="bold">💀</text></svg>`;
        
        function getRandomPos() { const rect = gameArena.getBoundingClientRect(); return { x: Math.random() * (rect.width - 70), y: Math.random() * (rect.height - 70) }; }
        function clearAll() { if (currentImp) currentImp.remove(); if (goldenImp) goldenImp.remove(); currentFakes.forEach(f => f.remove()); currentTraps.forEach(t => t.remove()); currentFakes = []; currentTraps = []; goldenImp = null; currentImp = null; }
        
        function spawnTraps() {
            currentTraps.forEach(t => t.remove());
            currentTraps = [];
            let trapCount = currentLevel >= 3 ? 2 : 1;
            for (let i = 0; i < trapCount; i++) {
                const pos = getRandomPos();
                const trap = document.createElement('div');
                trap.className = 'trap';
                trap.innerHTML = trapSvg;
                trap.style.left = pos.x + 'px';
                trap.style.top = pos.y + 'px';
                trap.style.position = 'absolute';
                trap.addEventListener('click', (e) => { e.stopPropagation(); if (!gameActive) return; timeLeft = Math.max(0.5, timeLeft - 0.8); gameTimerEl.textContent = `⏱️ ${timeLeft.toFixed(1)}с`; gameMessage.innerHTML = '💀 ЛОВУШКА! -0.8 сек 💀'; trap.remove(); gameArena.classList.add('screen-shake'); setTimeout(() => gameArena.classList.remove('screen-shake'), 300); });
                gameArena.appendChild(trap);
                currentTraps.push(trap);
            }
        }
        
        function spawnFakes() {
            currentFakes.forEach(f => f.remove());
            currentFakes = [];
            let fakeCount = currentLevel === 1 ? 1 : currentLevel === 2 ? 2 : currentLevel === 3 ? 3 : currentLevel === 4 ? 4 : 5;
            for (let i = 0; i < fakeCount; i++) {
                const pos = getRandomPos();
                const fake = document.createElement('div');
                fake.className = 'fake-imp';
                fake.innerHTML = fakeSvg;
                fake.style.left = pos.x + 'px';
                fake.style.top = pos.y + 'px';
                fake.style.position = 'absolute';
                fake.addEventListener('click', (e) => { e.stopPropagation(); if (!gameActive) return; currentCombo = 0; gameComboEl.textContent = '0'; gameMessage.innerHTML = '😵 ФАЛЬШИВКА! Комбо сброшено! 😵'; fake.remove(); gameArena.classList.add('screen-shake'); setTimeout(() => gameArena.classList.remove('screen-shake'), 200); });
                gameArena.appendChild(fake);
                currentFakes.push(fake);
            }
        }
        
        function spawnGoldenImp() {
            if (goldenImp) goldenImp.remove();
            if (Math.random() < 0.3) {
                const pos = getRandomPos();
                const golden = document.createElement('div');
                golden.className = 'golden-imp';
                golden.innerHTML = goldenSvg;
                golden.style.left = pos.x + 'px';
                golden.style.top = pos.y + 'px';
                golden.style.position = 'absolute';
                golden.addEventListener('click', (e) => { e.stopPropagation(); if (!gameActive) return; catchGolden(); });
                gameArena.appendChild(golden);
                goldenImp = golden;
                setTimeout(() => { if (goldenImp && goldenImp.parentNode) goldenImp.remove(); goldenImp = null; }, 2000);
            }
        }
        
        function catchGolden() {
            currentScore += 2;
            gameScoreEl.textContent = currentScore;
            currentCombo++;
            gameComboEl.textContent = currentCombo;
            if (goldenImp) goldenImp.remove();
            goldenImp = null;
            gameMessage.innerHTML = '🌟 ЗОЛОТОЙ БЕС! +2 ОЧКА! 🌟';
            gameArena.classList.add('screen-shake');
            setTimeout(() => gameArena.classList.remove('screen-shake'), 200);
            if (currentScore >= 5) levelUp();
            else { spawnImp(); resetTimer(); spawnFakes(); spawnTraps(); }
        }
        
        function spawnImp() {
            if (currentImp) currentImp.remove();
            const pos = getRandomPos();
            const imp = document.createElement('div');
            imp.className = 'game-imp';
            imp.innerHTML = impSvg;
            imp.style.left = pos.x + 'px';
            imp.style.top = pos.y + 'px';
            imp.style.position = 'absolute';
            imp.addEventListener('click', (e) => { e.stopPropagation(); if (!gameActive) return; catchImp(); });
            gameArena.appendChild(imp);
            currentImp = imp;
        }
        
        function catchImp() {
            currentScore++;
            gameScoreEl.textContent = currentScore;
            currentCombo++;
            gameComboEl.textContent = currentCombo;
            currentImp.classList.add('hit-animation');
            setTimeout(() => currentImp.classList.remove('hit-animation'), 200);
            gameMessage.innerHTML = `🎯 ПОПАЛ! +1 (Комбо x${currentCombo}) 🎯`;
            gameArena.classList.add('screen-shake');
            setTimeout(() => gameArena.classList.remove('screen-shake'), 150);
            if (currentScore >= 5) levelUp();
            else { spawnImp(); resetTimer(); spawnFakes(); spawnTraps(); spawnGoldenImp(); }
        }
        
        function levelUp() {
            if (currentLevel >= 5) { winGame(); return; }
            currentLevel++;
            currentScore = 0;
            gameScoreEl.textContent = '0';
            gameLevelEl.textContent = currentLevel;
            gameTarget.textContent = '5';
            gameMessage.innerHTML = `✨ УРОВЕНЬ ${currentLevel}! Быстрее! ✨`;
            if (moveInterval) clearInterval(moveInterval);
            let speed = currentLevel === 1 ? 900 : currentLevel === 2 ? 700 : currentLevel === 3 ? 550 : currentLevel === 4 ? 450 : 350;
            startMoving(speed);
            timeLeft = Math.max(2.5 - (currentLevel - 1) * 0.3, 1.2);
            resetTimer();
            clearAll();
            spawnImp();
            spawnFakes();
            spawnTraps();
            spawnGoldenImp();
        }
        
        function moveImp() { if (!gameActive || !currentImp) return; const pos = getRandomPos(); currentImp.style.left = pos.x + 'px'; currentImp.style.top = pos.y + 'px'; }
        function startMoving(delay) { if (moveInterval) clearInterval(moveInterval); moveInterval = setInterval(() => moveImp(), delay); }
        
        function resetTimer() {
            if (timerInterval) clearInterval(timerInterval);
            timeLeft = Math.max(3 - (currentLevel - 1) * 0.3, 1.2);
            gameTimerEl.textContent = `⏱️ ${timeLeft.toFixed(1)}с`;
            timerInterval = setInterval(() => {
                if (!gameActive) return;
                timeLeft -= 0.1;
                gameTimerEl.textContent = `⏱️ ${timeLeft.toFixed(1)}с`;
                if (timeLeft <= 0) { clearInterval(timerInterval); gameMessage.innerHTML = '💨 ВРЕМЯ ВЫШЛО! Игра заново 💨'; endGame(false); }
            }, 100);
        }
        
        function showDiscount() {
            if (discountGiven) return;
            discountGiven = true;
            const div = document.createElement('div');
            div.className = 'discount-badge';
            div.innerHTML = '🎉 СКИДКА 25% НА РАСКЛАД ТАРО! 🎉<br><span style="font-size:1rem">Пиши @Zara_zzaww с кодом GAME25</span>';
            document.body.appendChild(div);
            setTimeout(() => { div.style.transition = 'all 0.5s'; div.style.opacity = '0'; div.style.transform = 'translate(-50%, -50%) scale(0)'; setTimeout(() => div.remove(), 500); }, 5000);
        }
        
        function winGame() {
            gameActive = false;
            if (moveInterval) clearInterval(moveInterval);
            if (timerInterval) clearInterval(timerInterval);
            if (currentScore > bestScore) { bestScore = currentScore; localStorage.setItem('gameBestScore', bestScore); gameBestEl.textContent = bestScore; }
            gameMessage.innerHTML = '🏆 ПОБЕДА! Ты прошёл все уровни! 🏆';
            showDiscount();
            setTimeout(() => { gameOverlay.style.display = 'none'; resetGame(); }, 3000);
        }
        
        function endGame(isWin) {
            gameActive = false;
            if (moveInterval) clearInterval(moveInterval);
            if (timerInterval) clearInterval(timerInterval);
            clearAll();
            if (!isWin) { setTimeout(() => { resetGame(); gameOverlay.style.display = 'none'; }, 2000); }
        }
        
        function resetGame() { currentLevel = 1; currentScore = 0; currentCombo = 0; discountGiven = false; gameActive = false; if (moveInterval) clearInterval(moveInterval); if (timerInterval) clearInterval(timerInterval); clearAll(); }
        
        function startGame() {
            resetGame();
            gameActive = true;
            currentLevel = 1;
            currentScore = 0;
            currentCombo = 0;
            gameLevelEl.textContent = '1';
            gameScoreEl.textContent = '0';
            gameTarget.textContent = '5';
            gameComboEl.textContent = '0';
            gameMessage.innerHTML = '🔥 ЛОВИ БЕСА! Золотой даёт x2! 🔥';
            gameArena.innerHTML = '';
            startMoving(900);
            timeLeft = 3;
            resetTimer();
            spawnImp();
            spawnFakes();
            spawnTraps();
        }
        
        document.getElementById('gameStartBtn').addEventListener('click', () => { startGame(); });
        document.getElementById('gameCloseBtn').addEventListener('click', () => { gameOverlay.style.display = 'none'; resetGame(); });
    </script>
</body>
</html>
