<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CryptoVision Pro - Advanced Trading Platform</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #6c5ce7;
            --primary-dark: #5649d1;
            --secondary-color: #a29bfe;
            --dark-color: #1a1a2e;
            --light-color: #f5f6fa;
            --success-color: #00b894;
            --danger-color: #d63031;
            --warning-color: #fdcb6e;
            --info-color: #0984e3;
            --border-radius: 10px;
            --box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
            --transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--dark-color);
            color: var(--light-color);
            line-height: 1.6;
            margin: 0;
            padding: 0;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }

        h1, h2, h3, h4 {
            font-weight: 600;
            margin-top: 0;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Styles */
        .header {
            background-color: rgba(26, 26, 46, 0.9);
            box-shadow: var(--box-shadow);
            position: sticky;
            top: 0;
            z-index: 100;
            backdrop-filter: blur(10px);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            display: flex;
            align-items: center;
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--light-color);
            text-decoration: none;
        }

        .logo-highlight {
            color: var(--primary-color);
        }

        .logo i {
            margin-right: 10px;
            font-size: 1.8rem;
            color: var(--primary-color);
        }

        .nav-links {
            display: flex;
            list-style: none;
            margin: 0;
            padding: 0;
        }

        .nav-links li {
            margin-left: 30px;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--light-color);
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }

        .nav-links a:hover {
            color: var(--primary-color);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: var(--primary-color);
            transition: var(--transition);
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .auth-buttons {
            display: flex;
            align-items: center;
        }

        .btn {
            padding: 12px 24px;
            border: none;
            border-radius: var(--border-radius);
            cursor: pointer;
            font-weight: 500;
            transition: var(--transition);
            font-size: 0.95rem;
        }

        .btn-primary {
            background-color: var(--primary-color);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(108, 92, 231, 0.3);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid var(--primary-color);
            color: var(--primary-color);
        }

        .btn-outline:hover {
            background-color: rgba(108, 92, 231, 0.1);
        }

        .btn-login {
            background-color: transparent;
            color: var(--light-color);
            margin-right: 15px;
        }

        .btn-login:hover {
            color: var(--primary-color);
        }

        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--light-color);
        }

        /* Hero Section */
        .hero {
            padding: 100px 0 80px;
            background: linear-gradient(135deg, #1a1a2e 0%, #16213e 100%);
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(108, 92, 231, 0.1) 0%, transparent 70%);
            z-index: 0;
        }

        .hero-content {
            max-width: 600px;
            position: relative;
            z-index: 1;
        }

        .hero h1 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .text-gradient {
            background: linear-gradient(90deg, var(--primary-color), var(--secondary-color));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
        }

        .hero p {
            font-size: 1.15rem;
            margin-bottom: 30px;
            color: #b8c2d8;
        }

        .hero-cta {
            display: flex;
            gap: 15px;
            margin-bottom: 40px;
        }

        .btn-lg {
            padding: 14px 32px;
            font-size: 1.05rem;
        }

        .hero-stats {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        .stat-card {
            background-color: rgba(255, 255, 255, 0.05);
            padding: 15px 20px;
            border-radius: var(--border-radius);
            box-shadow: var(--box-shadow);
            min-width: 120px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: var(--transition);
        }

        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
        }

        .stat-value {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
        }

        .stat-label {
            font-size: 0.85rem;
            color: #b8c2d8;
        }

        .hero-image {
            flex: 1;
            position: relative;
            z-index: 1;
        }

        .chart-container {
            background-color: rgba(26, 26, 46, 0.7);
            border-radius: var(--border-radius);
            padding: 20px;
            box-shadow: var(--box-shadow);
            height: 350px;
            width: 100%;
            position: relative;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .chart-placeholder {
            background: linear-gradient(135deg, rgba(26, 26, 46, 0.5) 0%, rgba(44, 44, 84, 0.7) 100%);
            height: 100%;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--light-color);
            font-weight: 500;
            border: 1px dashed rgba(255, 255, 255, 0.2);
        }

        /* Market Data Section */
        .market-section {
            padding: 80px 0;
            background-color: var(--dark-color);
        }

        .section-header {
            text-align: center;
            margin-bottom: 40px;
        }

        .section-title {
            font-size: 2.2rem;
            margin-bottom: 10px;
            color: var(--light-color);
        }

        .section-subtitle {
            color: #b8c2d8;
            font-size: 1.1rem;
            max-width: 700px;
            margin: 0 auto;
        }

        .crypto-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 20px;
        }

        .crypto-card {
            background-color: rgba(26, 26, 46, 0.7);
            border-radius: var(--border-radius);
            padding: 20px;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .crypto-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            border-color: rgba(108, 92, 231, 0.3);
        }

        .crypto-header {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }

        .crypto-icon {
            width: 40px;
            height: 40px;
            margin-right: 10px;
            border-radius: 50%;
        }

        .crypto-name {
            font-weight: 600;
            color: var(--light-color);
        }

        .crypto-symbol {
            color: #b8c2d8;
            font-size: 0.9rem;
            margin-left: 5px;
        }

        .crypto-price {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 5px;
            color: var(--light-color);
        }

        .price-change {
            display: flex;
            align-items: center;
            font-size: 0.9rem;
        }

        .positive {
            color: var(--success-color);
        }

        .negative {
            color: var(--danger-color);
        }

        .sparkline-container {
            height: 40px;
            margin-top: 15px;
            background-color: rgba(26, 26, 46, 0.5);
            border-radius: 4px;
            position: relative;
            overflow: hidden;
        }

        .sparkline {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            stroke: var(--primary-color);
            fill: none;
            stroke-width: 2;
        }

        .sparkline-fill {
            fill: rgba(108, 92, 231, 0.1);
        }

        /* Market Sentiment Section */
        .sentiment-section {
            padding: 80px 0;
            background-color: rgba(21, 21, 39, 0.8);
        }

        .sentiment-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .sentiment-card {
            background-color: rgba(26, 26, 46, 0.7);
            border-radius: var(--border-radius);
            padding: 25px;
            box-shadow: var(--box-shadow);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: var(--transition);
        }

        .sentiment-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        .sentiment-card h3 {
            color: var(--light-color);
            margin-bottom: 10px;
        }

        .sentiment-value {
            font-size: 1.8rem;
            font-weight: 700;
            margin: 10px 0;
            color: var(--light-color);
        }

        .sentiment-bar-container {
            height: 8px;
            background-color: rgba(26, 26, 46, 0.5);
            border-radius: 4px;
            margin: 15px 0;
            overflow: hidden;
            position: relative;
        }

        .sentiment-bar {
            height: 100%;
            background: linear-gradient(to right,
                #d63031 0%,
                #ff7f50 25%,
                #ffeaa7 50%,
                #55efc4 75%,
                #00b894 100%
            );
            width: 0%;
            transition: width 1s ease-out;
        }
        
        .sentiment-bar-thumb {
            position: absolute;
            top: -5px;
            width: 2px;
            height: 18px;
            background-color: white;
            border-radius: 2px;
            box-shadow: 0 0 5px rgba(0,0,0,0.3);
            transform: translateX(-50%);
            transition: left 1s ease-out;
        }

        .sentiment-description {
            font-size: 0.9rem;
            color: #b8c2d8;
        }

        /* Strategies Section */
        .strategies-section {
            padding: 80px 0;
            background-color: var(--dark-color);
        }

        .strategy-tabs {
            display: flex;
            justify-content: center;
            margin-bottom: 30px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
            flex-wrap: wrap;
        }

        .strategy-tab {
            padding: 12px 25px;
            background: none;
            border: none;
            border-bottom: 3px solid transparent;
            font-size: 1rem;
            font-weight: 600;
            color: #b8c2d8;
            cursor: pointer;
            transition: var(--transition);
            margin: 0 5px;
        }

        .strategy-tab.active {
            color: var(--primary-color);
            border-bottom-color: var(--primary-color);
        }

        .strategy-tab:hover:not(.active) {
            color: var(--light-color);
        }

        .strategy-content {
            display: none;
        }

        .strategy-content.active {
            display: block;
        }

        .strategy-header {
            text-align: center;
            margin-bottom: 40px;
        }

        .market-indicator {
            display: inline-flex;
            align-items: center;
            padding: 8px 20px;
            border-radius: 30px;
            font-weight: 600;
            margin-bottom: 15px;
            backdrop-filter: blur(5px);
        }

        .market-indicator i {
            margin-right: 8px;
        }

        .market-indicator.bullish {
            background-color: rgba(0, 184, 148, 0.1);
            color: var(--success-color);
            border: 1px solid rgba(0, 184, 148, 0.3);
        }

        .market-indicator.bearish {
            background-color: rgba(214, 48, 49, 0.1);
            color: var(--danger-color);
            border: 1px solid rgba(214, 48, 49, 0.3);
        }

        .market-indicator.volatile {
            background-color: rgba(253, 203, 110, 0.1);
            color: #e17055;
            border: 1px solid rgba(253, 203, 110, 0.3);
        }
        .market-indicator.ranging {
            background-color: rgba(129, 236, 236, 0.1);
            color: #00cec9;
            border: 1px solid rgba(129, 236, 236, 0.3);
        }

        .strategies-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .strategy-card {
            background-color: rgba(26, 26, 46, 0.7);
            border-radius: var(--border-radius);
            padding: 25px;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            border-top: 4px solid var(--primary-color);
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.5s ease-out, transform 0.5s ease-out, box-shadow 0.3s ease;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .strategy-card.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .strategy-card:hover {
            transform: translateY(-5px) !important;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            border-color: rgba(108, 92, 231, 0.5);
        }

        .strategy-card h4 {
            font-size: 1.3rem;
            margin-bottom: 15px;
            color: var(--light-color);
            display: flex;
            align-items: center;
        }

        .strategy-card h4 i {
            margin-right: 10px;
            color: var(--primary-color);
        }

        .strategy-card p {
            color: #b8c2d8;
            margin-bottom: 15px;
        }

        .strategy-meta {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
            padding-top: 15px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
        }

        .difficulty {
            display: flex;
            align-items: center;
            color: #b8c2d8;
        }

        .difficulty i {
            color: var(--warning-color);
            margin-right: 5px;
        }

        .risk-level {
            margin-left: 15px;
            color: #b8c2d8;
        }

        .reward-ratio {
            background-color: rgba(108, 92, 231, 0.2);
            color: var(--primary-color);
            padding: 5px 12px;
            border-radius: 20px;
            font-weight: 600;
            font-size: 0.8rem;
        }

        .strategy-indicators {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 15px;
        }

        .indicator-tag {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 500;
            color: #b8c2d8;
        }

        /* Indicators Section */
        .indicator-section {
            padding: 80px 0;
            background-color: rgba(21, 21, 39, 0.8);
        }

        .indicators-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .indicator-card {
            background-color: rgba(26, 26, 46, 0.7);
            border-radius: var(--border-radius);
            padding: 25px;
            box-shadow: var(--box-shadow);
            transition: var(--transition);
            text-align: center;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .indicator-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
        }

        .indicator-icon {
            width: 60px;
            height: 60px;
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 1.5rem;
            box-shadow: 0 5px 15px rgba(108, 92, 231, 0.3);
        }

        .indicator-card h3 {
            margin-bottom: 15px;
            color: var(--light-color);
        }

        .indicator-card p {
            color: #b8c2d8;
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .indicator-meta {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .indicator-tag.bullish {
            background-color: rgba(0, 184, 148, 0.1);
            color: var(--success-color);
            border: 1px solid rgba(0, 184, 148, 0.3);
        }

        .indicator-tag.bearish {
            background-color: rgba(214, 48, 49, 0.1);
            color: var(--danger-color);
            border: 1px solid rgba(214, 48, 49, 0.3);
        }

        .indicator-tag.volatile {
            background-color: rgba(253, 203, 110, 0.1);
            color: #e17055;
            border: 1px solid rgba(253, 203, 110, 0.3);
        }

        .indicator-tag.ranging {
            background-color: rgba(129, 236, 236, 0.1);
            color: #00cec9;
            border: 1px solid rgba(129, 236, 236, 0.3);
        }

        .indicator-tag.breakout {
            background-color: rgba(108, 92, 231, 0.1);
            color: var(--primary-color);
            border: 1px solid rgba(108, 92, 231, 0.3);
        }

        .indicator-tag.confirmation {
            background-color: rgba(9, 132, 227, 0.1);
            color: var(--info-color);
            border: 1px solid rgba(9, 132, 227, 0.3);
        }

        /* Footer */
        .footer {
            background-color: #0f0f1f;
            color: white;
            padding: 60px 0 0;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-section h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: white;
        }

        .footer-section p {
            margin-bottom: 20px;
            color: #b8c2d8;
        }

        .footer-section ul {
            list-style: none;
            padding: 0;
        }

        .footer-section ul li {
            margin-bottom: 10px;
        }

        .footer-section ul li a {
            color: #b8c2d8;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-section ul li a:hover {
            color: var(--primary-color);
            padding-left: 5px;
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-icons a {
            color: #b8c2d8;
            font-size: 1.2rem;
            transition: var(--transition);
        }

        .social-icons a:hover {
            color: var(--primary-color);
            transform: translateY(-3px);
        }

        .subscribe-form {
            display: flex;
            margin-top: 20px;
        }

        .subscribe-form input {
            flex: 1;
            padding: 12px;
            border: none;
            border-radius: var(--border-radius) 0 0 var(--border-radius);
            background-color: rgba(255, 255, 255, 0.1);
            color: white;
            outline: none;
        }

        .subscribe-form input::placeholder {
            color: #b8c2d8;
        }

        .subscribe-form button {
            border-radius: 0 var(--border-radius) var(--border-radius) 0;
            padding: 0 20px;
        }

        .footer-bottom {
            padding: 20px 0;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: #b8c2d8;
            font-size: 0.9rem;
        }

        .footer-links {
            display: flex;
            gap: 20px;
        }

        .footer-links a {
            color: #b8c2d8;
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover {
            color: var(--primary-color);
        }

        /* Loading Skeleton */
        .skeleton {
            background-color: rgba(255, 255, 255, 0.05);
            border-radius: 4px;
            position: relative;
            overflow: hidden;
        }

        .skeleton::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(90deg, 
                transparent, 
                rgba(255, 255, 255, 0.05), 
                transparent);
            animation: shimmer 1.5s infinite;
        }

        @keyframes shimmer {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }

        /* Responsive Styles */
        @media (min-width: 992px) {
            .hero .container {
                display: flex;
                align-items: center;
                gap: 50px;
            }
        }

        @media (max-width: 992px) {
            .hero {
                text-align: center;
            }
            
            .hero-content {
                max-width: 100%;
                margin-bottom: 40px;
            }
            
            .hero-cta {
                justify-content: center;
            }
            
            .hero-stats {
                justify-content: center;
            }
            
            .chart-container {
                height: 300px;
            }
        }

        @media (max-width: 768px) {
            .nav-links {
                display: none;
                flex-direction: column;
                position: absolute;
                top: 80px;
                left: 0;
                width: 100%;
                background-color: rgba(26, 26, 46, 0.95);
                box-shadow: var(--box-shadow);
                padding: 20px 0;
                border-top: 1px solid rgba(255, 255, 255, 0.1);
                z-index: 99;
                backdrop-filter: blur(10px);
            }

            .nav-links.active {
                display: flex;
            }

            .nav-links li {
                margin: 10px 0;
                text-align: center;
            }

            .auth-buttons {
                display: none;
                position: absolute;
                top: 250px;
                left: 0;
                width: 100%;
                flex-direction: column;
                align-items: center;
                gap: 15px;
                padding: 20px 0;
                background-color: rgba(26, 26, 46, 0.95);
                box-shadow: var(--box-shadow);
                border-top: 1px solid rgba(255, 255, 255, 0.1);
                z-index: 99;
                backdrop-filter: blur(10px);
            }

            .auth-buttons.active {
                display: flex;
            }
            
            .mobile-menu {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .strategy-tab {
                padding: 10px 15px;
                font-size: 0.9rem;
            }
        }

        @media (max-width: 576px) {
            .hero-cta {
                flex-direction: column;
            }
            
            .hero-stats {
                flex-direction: column;
                align-items: center;
            }
            
            .stat-card {
                width: 100%;
                text-align: center;
            }

            .footer-content {
                grid-template-columns: 1fr;
            }

            .footer-bottom {
                flex-direction: column;
                gap: 15px;
                text-align: center;
            }

            .footer-links {
                justify-content: center;
            }
        }

        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .animate-fade-in {
            animation: fadeIn 0.5s ease-out forwards;
        }

        /* Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: var(--dark-color);
        }

        ::-webkit-scrollbar-thumb {
            background: var(--primary-color);
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: var(--primary-dark);
        }
    </style>
</head>
<body>
    <header class="header">
        <div class="container">
            <nav class="navbar">
                <a href="#" class="logo">
                    <i class="fab fa-bitcoin"></i>
                    <span>CryptoVision<span class="logo-highlight">Pro</span></span>
                </a>
                <ul class="nav-links" id="navLinks">
                    <li><a href="#market">Market</a></li>
                    <li><a href="#sentiment">Sentiment</a></li>
                    <li><a href="#strategies">Strategies</a></li>
                    <li><a href="#indicators">Indicators</a></li>
                </ul>
                <div class="auth-buttons">
                    <button class="btn btn-login">Login</button>
                    <button class="btn btn-primary">Sign Up</button>
                </div>
                <div class="mobile-menu" id="mobileMenuToggle">
                    <i class="fas fa-bars"></i>
                </div>
            </nav>
        </div>
    </header>

    <main class="main-content">
        <section class="hero">
            <div class="container">
                <div class="hero-content">
                    <h1>Advanced Crypto Trading <span class="text-gradient">Strategies</span></h1>
                    <p>Professional-grade tools and analytics for bullish and bearish market conditions</p>
                    <div class="hero-cta">
                        <button class="btn btn-primary btn-lg">Explore Strategies</button>
                        <button class="btn btn-outline">Market Analysis <i class="fas fa-arrow-right"></i></button>
                    </div>
                    <div class="hero-stats">
                        <div class="stat-card">
                            <div class="stat-value">15+</div>
                            <div class="stat-label">Trading Strategies</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-value">24/7</div>
                            <div class="stat-label">Market Monitoring</div>
                        </div>
                        <div class="stat-card">
                            <div class="stat-value">100+</div>
                            <div class="stat-label">Technical Indicators</div>
                        </div>
                    </div>
                </div>
                <div class="hero-image">
                    <div class="chart-container">
                        <div class="chart-placeholder">Live Market Chart (Dummy)</div>
                    </div>
                </div>
            </div>
        </section>

        <section id="market" class="market-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">Live Market Data</h2>
                    <p class="section-subtitle">Real-time cryptocurrency prices and trends</p>
                </div>
                <div class="crypto-grid" id="crypto-data">
                    <!-- Loading skeleton -->
                    <div class="crypto-card skeleton" style="height: 150px;"></div>
                    <div class="crypto-card skeleton" style="height: 150px;"></div>
                    <div class="crypto-card skeleton" style="height: 150px;"></div>
                    <div class="crypto-card skeleton" style="height: 150px;"></div>
                </div>
            </div>
        </section>

        <section id="sentiment" class="sentiment-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">Market Sentiment Analysis</h2>
                    <p class="section-subtitle">Understand current market psychology and trends</p>
                </div>
                <div class="sentiment-cards">
                    <div class="sentiment-card">
                        <h3>Fear & Greed Index</h3>
                        <p id="fear-greed-index" class="sentiment-value">Loading...</p>
                        <div class="sentiment-bar-container">
                            <div id="sentiment-bar" class="sentiment-bar"></div>
                            <div id="sentiment-bar-thumb" class="sentiment-bar-thumb" style="left:0%;"></div>
                        </div>
                        <p class="sentiment-description" id="sentiment-desc">Loading market sentiment data...</p>
                    </div>
                    <div class="sentiment-card">
                        <h3>Bitcoin Dominance</h3>
                        <p id="btc-dominance" class="sentiment-value">Loading...</p>
                        <p class="sentiment-description">Percentage of total crypto market cap</p>
                    </div>
                    <div class="sentiment-card">
                        <h3>Total Market Cap</h3>
                        <p id="total-market-cap" class="sentiment-value">Loading...</p>
                        <p class="sentiment-description">Value of all cryptocurrencies combined</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="strategies" class="strategies-section">
            <div class="container">
                <div class="section-header">
                    <h2 class="section-title">Market-Adaptive Trading Strategies</h2>
                    <p class="section-subtitle">Professional strategies tailored for different market conditions</p>
                </div>
                
                <div class="strategy-tabs" id="strategyTabs">
                    <!-- Tabs will be generated by JavaScript -->
                </div>
                
                <div id="strategies-content">
                    <!-- Content will be generated by JavaScript -->
                </div>
            </div>
        </section>

        <section id="indicators" class="ind
