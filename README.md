<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sofi The Mastermind | Official Hub</title>
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&family=Hind+Siliguri:wght@400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-red: #FF0000;
            --accent-glow: rgba(255, 0, 0, 0.4);
            --glass-bg: rgba(20, 20, 20, 0.7);
            --glass-border: rgba(255, 255, 255, 0.1);
            --ios-blur: blur(20px);
            --text-main: #ffffff;
            --text-dim: #cfcfcf;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', 'Hind Siliguri', sans-serif;
        }

        body {
            background-color: #050505;
            background-image: 
                radial-gradient(circle at 20% 30%, rgba(255, 0, 0, 0.08) 0%, transparent 40%),
                radial-gradient(circle at 80% 70%, rgba(255, 0, 0, 0.08) 0%, transparent 40%);
            color: var(--text-main);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 40px 15px;
            overflow-x: hidden;
        }

        /* Trading Chart Background Pattern */
        body::after {
            content: "";
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background-image: linear-gradient(rgba(255,255,255,0.03) 1px, transparent 1px),
                              linear-gradient(90deg, rgba(255,255,255,0.03) 1px, transparent 1px);
            background-size: 40px 40px;
            z-index: -2;
        }

        .container {
            width: 100%;
            max-width: 440px;
            text-align: center;
        }

        /* Profile/Logo Section */
        .profile {
            margin-bottom: 35px;
        }

        .logo-wrapper {
            position: relative;
            display: inline-block;
            margin-bottom: 15px;
        }

        .profile-img {
            width: 110px;
            height: 110px;
            border-radius: 50%;
            border: 2px solid var(--primary-red);
            object-fit: cover;
            padding: 4px;
            box-shadow: 0 0 25px var(--accent-glow);
        }

        .trading-badge {
            position: absolute;
            bottom: 5px;
            right: 5px;
            background: var(--primary-red);
            font-size: 0.7rem;
            padding: 4px 8px;
            border-radius: 20px;
            font-weight: 800;
            text-transform: uppercase;
        }

        .profile h1 {
            font-size: 1.6rem;
            font-weight: 800;
            letter-spacing: -0.5px;
            text-transform: uppercase;
            margin-bottom: 5px;
        }

        .profile h1 span { color: var(--primary-red); }
        .profile p { color: var(--text-dim); font-size: 0.9rem; opacity: 0.8; }

        /* Links Section */
        .links-group {
            display: flex;
            flex-direction: column;
            gap: 14px;
        }

        .link-card {
            background: var(--glass-bg);
            backdrop-filter: var(--ios-blur);
            -webkit-backdrop-filter: var(--ios-blur);
            border: 1px solid var(--glass-border);
            border-radius: 16px;
            padding: 16px 20px;
            text-decoration: none;
            color: var(--text-main);
            display: flex;
            align-items: center;
            transition: all 0.3s ease;
            position: relative;
        }

        .link-card:hover {
            transform: translateY(-3px);
            border-color: var(--primary-red);
            background: rgba(255, 255, 255, 0.08);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.5);
        }

        .link-card i {
            font-size: 1.4rem;
            width: 35px;
            color: var(--primary-red);
        }

        .link-content {
            flex-grow: 1;
            text-align: left;
            margin-left: 10px;
        }

        .link-content h3 { font-size: 0.95rem; font-weight: 600; margin-bottom: 2px; }
        .link-content p { font-size: 0.75rem; color: var(--text-dim); }

        /* Pocket Option Special Style */
        .featured {
            background: linear-gradient(135deg, rgba(255,0,0,0.1) 0%, rgba(20,20,20,0.8) 100%);
            border-color: rgba(255, 0, 0, 0.3);
        }

        /* Footer & Notification */
        .notice-box {
            margin-top: 35px;
            padding: 15px;
            background: rgba(255, 255, 255, 0.03);
            border-radius: 12px;
            border-left: 3px solid var(--primary-red);
        }

        .notice-box p {
            font-size: 0.85rem;
            color: var(--text-dim);
            line-height: 1.4;
        }

        footer {
            margin-top: 30px;
            font-size: 0.75rem;
            color: #666;
            text-transform: uppercase;
            letter-spacing: 1.5px;
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .container { animation: fadeIn 0.8s ease-out; }

    </style>
</head>
<body>

<div class="container">
    <div class="profile">
        <div class="logo-wrapper">
            <img src="227708.jpg" alt="Sofi The Mastermind" class="profile-img">
            <div class="trading-badge"><i class="fas fa-bolt"></i> PRO</div>
        </div>
        <h1>SOFI THE <span>MASTERMIND</span></h1>
        <p><i class="fas fa-chart-area"></i> Binary Options Specialist & Content Creator</p>
    </div>

    <div class="links-group">
        <!-- Pocket Option -->
        <a href="http://pocketoption.mastermindsofi.com" target="_blank" class="link-card featured">
            <i class="fas fa-money-bill-trend-up"></i>
            <div class="link-content">
                <h3>Open Pocket Option Account</h3>
                <p>Join our exclusive trading team</p>
            </div>
            <i class="fas fa-chevron-right" style="font-size: 0.7rem; opacity: 0.4;"></i>
        </a>

        <!-- Free Signal -->
        <a href="https://t.me/sofi_the_mastermind_signal" target="_blank" class="link-card">
            <i class="fas fa-signal"></i>
            <div class="link-content">
                <h3>Free Signal Channel</h3>
                <p>90%+ Accuracy Trading Signals</p>
            </div>
            <i class="fas fa-chevron-right" style="font-size: 0.7rem; opacity: 0.4;"></i>
        </a>

        <!-- YouTube -->
        <a href="https://youtube.com/@sofi_the_mastermind" target="_blank" class="link-card">
            <i class="fab fa-youtube"></i>
            <div class="link-content">
                <h3>Mastermind YouTube</h3>
                <p>Learn Strategies & Market Analysis</p>
            </div>
            <i class="fas fa-chevron-right" style="font-size: 0.7rem; opacity: 0.4;"></i>
        </a>

        <!-- Public Telegram -->
        <a href="https://t.me/sofi_the_mastermind" target="_blank" class="link-card">
            <i class="fab fa-telegram-plane"></i>
            <div class="link-content">
                <h3>Public Telegram</h3>
                <p>Daily updates & community news</p>
            </div>
            <i class="fas fa-chevron-right" style="font-size: 0.7rem; opacity: 0.4;"></i>
        </a>

        <!-- Personal Contact -->
        <a href="https://t.me/sofi_the_master" target="_blank" class="link-card">
            <i class="fas fa-headset"></i>
            <div class="link-content">
                <h3>Contact Me</h3>
                <p>Direct support for account & signals</p>
            </div>
            <i class="fas fa-chevron-right" style="font-size: 0.7rem; opacity: 0.4;"></i>
        </a>
    </div>

    <!-- Requested Notice Message -->
    <div class="notice-box">
        <p>যদি টেলিগ্রাম ওপেন না হয় তাহলে টেলিগ্রামে সার্চ করেন <strong>@sofi_the_master</strong></p>
    </div>

    <footer>
        <p>&copy; 2026 SOFI THE MASTERMIND | ALL SYSTEMS OPERATIONAL</p>
    </footer>
</div>

</body>
</html>
