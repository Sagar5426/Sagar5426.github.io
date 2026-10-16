
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My College Mate — Sagar Jangra</title>
    <meta name="description" content="Download My College Mate by Sagar Jangra on the Apple App Store and Google Play Store.">
    <!-- Browser Tab Icon (Favicon) -->
    <link rel="icon" type="image/png" href="CollegeHat.png">
    <link rel="apple-touch-icon" href="CollegeHat.png">
    <style>
        :root {
            --bg-primary: #07090e;
            --bg-card: rgba(255, 255, 255, 0.035);
            --border-glass: rgba(255, 255, 255, 0.09);
            --border-hover: rgba(255, 255, 255, 0.22);
            --text-primary: #f8fafc;
            --text-secondary: #94a3b8;
            --accent-blue: #3b82f6;
            --accent-indigo: #6366f1;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display", "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-primary);
            color: var(--text-primary);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 24px;
            position: relative;
            overflow-x: hidden;
            -webkit-font-smoothing: antialiased;
        }

        /* Ambient Background Glows */
        .glow {
            position: fixed;
            width: 420px;
            height: 420px;
            border-radius: 50%;
            filter: blur(110px);
            opacity: 0.22;
            z-index: 0;
            pointer-events: none;
        }

        .glow-top {
            top: -120px;
            left: -100px;
            background: var(--accent-blue);
        }

        .glow-bottom {
            bottom: -120px;
            right: -100px;
            background: var(--accent-indigo);
        }

        /* Main Glassmorphic Container */
        .card {
            position: relative;
            z-index: 1;
            max-width: 480px;
            width: 100%;
            background: var(--bg-card);
            backdrop-filter: blur(24px);
            -webkit-backdrop-filter: blur(24px);
            border: 1px solid var(--border-glass);
            border-radius: 28px;
            padding: 48px 36px;
            text-align: center;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.65);
        }

        /* App Icon Emblem */
        .app-icon {
            width: 88px;
            height: 88px;
            margin: 0 auto 20px;
            border-radius: 22px;
            background: rgba(255, 255, 255, 0.04);
            border: 1px solid rgba(255, 255, 255, 0.12);
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.45);
        }

        .app-icon img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }

        h1 {
            font-size: 32px;
            font-weight: 800;
            letter-spacing: -0.6px;
            margin-bottom: 12px;
            background: linear-gradient(180deg, #ffffff 0%, #cbd5e1 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .subtitle {
            font-size: 15.5px;
            line-height: 1.6;
            color: var(--text-secondary);
            margin-bottom: 32px;
        }

        /* Store Buttons Layout */
        .button-group {
            display: flex;
            flex-direction: column;
            gap: 14px;
        }

        .store-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 14px;
            width: 100%;
            padding: 15px 24px;
            border-radius: 16px;
            text-decoration: none;
            color: var(--text-primary);
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--border-glass);
            transition: all 0.25s cubic-bezier(0.16, 1, 0.3, 1);
            position: relative;
        }

        .store-btn:hover {
            transform: translateY(-2px);
            background: rgba(255, 255, 255, 0.09);
            border-color: var(--border-hover);
            box-shadow: 0 12px 24px -6px rgba(0, 0, 0, 0.5);
        }

        .store-btn:active {
            transform: translateY(0);
        }

        /* Primary highlight for detected OS */
        .store-btn.recommended {
            background: linear-gradient(135deg, rgba(59, 130, 246, 0.18), rgba(99, 102, 241, 0.18));
            border-color: rgba(96, 165, 250, 0.5);
            box-shadow: 0 8px 25px -4px rgba(59, 130, 246, 0.25);
        }

        .store-btn.recommended:hover {
            background: linear-gradient(135deg, rgba(59, 130, 246, 0.26), rgba(99, 102, 241, 0.26));
            border-color: rgba(96, 165, 250, 0.75);
        }

        .store-icon {
            width: 28px;
            height: 28px;
            flex-shrink: 0;
        }

        .btn-text {
            text-align: left;
            display: flex;
            flex-direction: column;
        }

        .btn-label {
            font-size: 11px;
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 0.6px;
            color: var(--text-secondary);
            line-height: 1.1;
        }

        .btn-title {
            font-size: 18px;
            font-weight: 700;
            letter-spacing: -0.2px;
            color: var(--text-primary);
            line-height: 1.25;
            margin-top: 2px;
        }

        .device-hint {
            margin-top: 24px;
            font-size: 12.5px;
            color: #64748b;
        }

        @media (min-width: 440px) {
            .button-group {
                flex-direction: row;
            }
            .store-btn {
                flex: 1;
                padding: 15px 18px;
            }
        }
    </style>
</head>
<body>

    <div class="glow glow-top"></div>
    <div class="glow glow-bottom"></div>

    <main class="card">
        <div class="app-icon">
            <img src="CollegeHat.png" alt="My College Mate Icon">
        </div>

        <h1>My College Mate</h1>
        <p class="subtitle">Track your attendance, manage your schedule, and stay on top of your classes effortlessly.</p>

        <div class="button-group">
            <!-- Apple App Store Button -->
            <a id="ios-btn"
               href="https://apps.apple.com/in/app/mycollegemate-attendance/id6754844571"
               class="store-btn"
               target="_blank"
               rel="noopener noreferrer">
                <svg class="store-icon" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M18.71 19.5c-.83 1.24-1.71 2.45-3.05 2.47-1.34.03-1.77-.79-3.29-.79-1.53 0-2 .77-3.27.82-1.31.05-2.3-1.32-3.14-2.53C4.25 17 2.94 12.45 4.7 9.39c.87-1.52 2.43-2.48 4.12-2.51 1.28-.02 2.5.87 3.29.87.78 0 2.26-1.07 3.81-.91.65.03 2.47.26 3.64 1.98-.09.06-2.17 1.28-2.15 3.81.03 3.02 2.65 4.03 2.68 4.04-.03.07-.42 1.44-1.38 2.83M15.97 6.33c.64-.78 1.08-1.86.96-2.94-.93.04-2.06.62-2.72 1.4-.58.68-1.1 1.79-.96 2.84 1.04.08 2.08-.52 2.72-1.3z"/>
                </svg>
                <div class="btn-text">
                    <span class="btn-label">Download on the</span>
                    <span class="btn-title">App Store</span>
                </div>
            </a>

            <!-- Google Play Store Button -->
            <a id="android-btn"
               href="https://play.google.com/store/apps/details?id=com.sagar.mycollegemate&pcampaignid=web_share"
               class="store-btn"
               target="_blank"
               rel="noopener noreferrer">
                <svg class="store-icon" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M3.609 1.814L13.792 12 3.61 22.186a1.996 1.996 0 0 1-.497-1.324V3.138c0-.505.19-.968.496-1.324zm11.62 11.62l2.79 2.79-9.927 5.732 7.137-8.522zm3.895-2.618l2.222 1.283c.87.502.87 1.32 0 1.822l-2.222 1.283-2.952-2.194 2.952-2.194zM8.092 2.276l9.927 5.732-2.79 2.79-7.137-8.522z"/>
                </svg>
                <div class="btn-text">
                    <span class="btn-label">Get it on</span>
                    <span class="btn-title">Google Play</span>
                </div>
            </a>
        </div>

        <p id="device-status" class="device-hint">Available for iOS and Android devices</p>
    </main>

    <script>
        (function highlightDeviceButton() {
            const ua = navigator.userAgent || navigator.vendor || window.opera;
            const iosBtn = document.getElementById('ios-btn');
            const androidBtn = document.getElementById('android-btn');
            const statusText = document.getElementById('device-status');

            if (/iPad|iPhone|iPod/.test(ua) && !window.MSStream) {
                iosBtn.classList.add('recommended');
                statusText.textContent = 'Optimized for your iPhone / iPad';
            } else if (/android/i.test(ua)) {
                androidBtn.classList.add('recommended');
                statusText.textContent = 'Optimized for your Android device';
            }
        })();
    </script>

</body>
</html>
