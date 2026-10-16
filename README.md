
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>My College Mate — Sagar Jangra</title>
    <meta name="description" content="Download MyCollegeMate by Sagar Jangra on the Apple App Store and Google Play Store.">

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
            font-family: -apple-system, BlinkMacSystemFont, "SF Pro Display",
                "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
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

        /* Main Container */
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
            padding: 40px 32px 30px;
            text-align: center;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.65);
        }

        /* App Icon */
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
            margin-bottom: 28px;
        }

        /* Store Buttons */
        .button-group {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .store-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 12px;
            width: 100%;
            padding: 14px 18px;
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

        .store-btn.recommended {
            background: linear-gradient(
                135deg,
                rgba(59, 130, 246, 0.18),
                rgba(99, 102, 241, 0.18)
            );
            border-color: rgba(96, 165, 250, 0.5);
            box-shadow: 0 8px 25px -4px rgba(59, 130, 246, 0.25);
        }

        .store-btn.recommended:hover {
            background: linear-gradient(
                135deg,
                rgba(59, 130, 246, 0.26),
                rgba(99, 102, 241, 0.26)
            );
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
            font-size: 10px;
            font-weight: 500;
            text-transform: uppercase;
            letter-spacing: 0.6px;
            color: var(--text-secondary);
            line-height: 1.3;
        }

        .btn-title {
            font-size: 17px;
            font-weight: 700;
            letter-spacing: -0.2px;
            color: var(--text-primary);
            line-height: 1.25;
            margin-top: 2px;
        }

        .device-hint {
            margin-top: 18px;
            font-size: 12px;
            color: #64748b;
        }

        /* Why Choose Us */
        .why-section {
            margin-top: 30px;
            padding-top: 25px;
            border-top: 1px solid var(--border-glass);
            text-align: left;
        }

        .why-eyebrow {
            color: #60a5fa;
            font-size: 10px;
            font-weight: 700;
            letter-spacing: 1.8px;
            text-transform: uppercase;
            margin-bottom: 8px;
            text-align: center;
        }

        .why-title {
            font-size: 21px;
            font-weight: 750;
            letter-spacing: -0.5px;
            margin-bottom: 8px;
            text-align: center;
            color: var(--text-primary);
        }

        .why-subtitle {
            text-align: center;
            color: var(--text-secondary);
            font-size: 13px;
            line-height: 1.5;
            margin-bottom: 22px;
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 10px;
        }

        .feature {
            display: flex;
            align-items: flex-start;
            gap: 10px;
            padding: 14px 12px;
            background: rgba(255, 255, 255, 0.025);
            border: 1px solid rgba(255, 255, 255, 0.065);
            border-radius: 14px;
            transition: background 0.2s ease, border-color 0.2s ease;
        }

        .feature:hover {
            background: rgba(255, 255, 255, 0.05);
            border-color: var(--border-hover);
        }

        .feature-icon {
            width: 30px;
            height: 30px;
            flex-shrink: 0;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 9px;
            color: #93c5fd;
            background: rgba(59, 130, 246, 0.12);
            font-size: 17px;
            font-weight: 600;
        }

        .feature h3 {
            font-size: 12.5px;
            font-weight: 700;
            line-height: 1.35;
            margin: 1px 0 5px;
            color: #f1f5f9;
        }

        .feature p {
            font-size: 11.5px;
            line-height: 1.5;
            color: var(--text-secondary);
        }

        .feature:last-child {
            grid-column: 1 / -1;
        }

        /* Closing Call to Action */
        .closing-cta {
            margin-top: 24px;
            font-size: 13px;
            line-height: 1.6;
            color: #cbd5e1;
            text-align: center;
        }

        .closing-cta strong {
            color: #ffffff;
        }

        @media (min-width: 440px) {
            .button-group {
                flex-direction: row;
            }

            .store-btn {
                flex: 1;
                padding: 14px 12px;
            }
        }

        @media (max-width: 380px) {
            body {
                padding: 14px;
            }

            .card {
                padding: 32px 20px 24px;
                border-radius: 24px;
            }

            h1 {
                font-size: 28px;
            }

            .feature-grid {
                gap: 8px;
            }

            .feature {
                padding: 12px 9px;
                gap: 8px;
            }

            .feature-icon {
                width: 26px;
                height: 26px;
                font-size: 15px;
            }

            .feature h3 {
                font-size: 12px;
            }

            .feature p {
                font-size: 11px;
            }
        }

        @media (prefers-reduced-motion: reduce) {
            *,
            *::before,
            *::after {
                scroll-behavior: auto !important;
                transition: none !important;
            }
        }
    </style>
</head>

<body>

    <div class="glow glow-top"></div>
    <div class="glow glow-bottom"></div>

    <main class="card">

        <div class="app-icon">
            <img src="CollegeHat.png" alt="My College Mate app icon">
        </div>

        <h1>My College Mate</h1>

        <p class="subtitle">
            Track attendance, manage your timetable, and stay on top of college life.
            All in one place.
        </p>

        <!-- Download Section -->
        <div class="button-group">

            <!-- Apple App Store -->
            <a
                id="ios-btn"
                href="https://apps.apple.com/in/app/mycollegemate-attendance/id6754844571"
                class="store-btn"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="Download My College Mate from the Apple App Store"
            >
                <svg class="store-icon" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true">
                    <path d="M18.71 19.5c-.83 1.24-1.71 2.45-3.05 2.47-1.34.03-1.77-.79-3.29-.79-1.53 0-2 .77-3.27.82-1.31.05-2.3-1.32-3.14-2.53C4.25 17 2.94 12.45 4.7 9.39c.87-1.52 2.43-2.48 4.12-2.51 1.28-.02 2.5.87 3.29.87.78 0 2.26-1.07 3.81-.91.65.03 2.47.26 3.64 1.98-.09.06-2.17 1.28-2.15 3.81.03 3.02 2.65 4.03 2.68 4.04-.03.07-.42 1.44-1.38 2.83M15.97 6.33c.64-.78 1.08-1.86.96-2.94-.93.04-2.06.62-2.72 1.4-.58.68-1.1 1.79-.96 2.84 1.04.08 2.08-.52 2.72-1.3z"/>
                </svg>

                <div class="btn-text">
                    <span class="btn-label">Download on the</span>
                    <span class="btn-title">App Store</span>
                </div>
            </a>

            <!-- Google Play Store -->
            <a
                id="android-btn"
                href="https://play.google.com/store/apps/details?id=com.sagar.mycollegemate&amp;pcampaignid=web_share"
                class="store-btn"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="Download My College Mate from Google Play"
            >
                <svg class="store-icon" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true">
                    <path d="M3.609 1.814L13.792 12 3.61 22.186a1.996 1.996 0 0 1-.497-1.324V3.138c0-.505.19-.968.496-1.324zm11.62 11.62l2.79 2.79-9.927 5.732 7.137-8.522zm3.895-2.618l2.222 1.283c.87.502.87 1.32 0 1.822l-2.222 1.283-2.952-2.194 2.952-2.194zM8.092 2.276l9.927 5.732-2.79 2.79-7.137-8.522z"/>
                </svg>

                <div class="btn-text">
                    <span class="btn-label">Get it on</span>
                    <span class="btn-title">Google Play</span>
                </div>
            </a>

        </div>

        <p id="device-status" class="device-hint">
            Available for iOS and Android
        </p>

        <!-- Why Choose Us Section -->
        <section class="why-section" id="why-choose-us" aria-labelledby="why-title">

            <p class="why-eyebrow">Made for student life</p>

            <h2 class="why-title" id="why-title">Why choose us?</h2>

            <p class="why-subtitle">
                Less college admin. More time for what matters.
            </p>

            <div class="feature-grid">

                <article class="feature">
                    <span class="feature-icon" aria-hidden="true">✦</span>
                    <div>
                        <h3>AI Timetable</h3>
                        <p>Turn a timetable photo into a schedule. Skip manual entry.</p>
                    </div>
                </article>

                <article class="feature">
                    <span class="feature-icon" aria-hidden="true">↯</span>
                    <div>
                        <h3>Quick Attendance</h3>
                        <p>Mark attendance from your lock screen or notifications.</p>
                    </div>
                </article>

                <article class="feature">
                    <span class="feature-icon" aria-hidden="true">▤</span>
                    <div>
                        <h3>Everything Together</h3>
                        <p>Keep notes, PDFs, and assignment reminders organized.</p>
                    </div>
                </article>

                <article class="feature">
                    <span class="feature-icon" aria-hidden="true">✓</span>
                    <div>
                        <h3>Student-Friendly</h3>
                        <p>A clean interface, minimal ads, and most features free.</p>
                    </div>
                </article>

                <article class="feature">
                    <span class="feature-icon" aria-hidden="true">☁</span>
                    <div>
                        <h3>iCloud Sync for Apple Devices</h3>
                        <p>Keep your data in sync across your Apple devices.</p>
                    </div>
                </article>

            </div>

            <p class="closing-cta">
                <strong>Your college life, simplified.</strong><br>
                Download MyCollegeMate and make every class count.
            </p>

        </section>

    </main>

    <script>
        (function highlightDeviceButton() {
            const ua = navigator.userAgent || navigator.vendor || window.opera;

            const iosBtn = document.getElementById("ios-btn");
            const androidBtn = document.getElementById("android-btn");
            const statusText = document.getElementById("device-status");

            if (/iPad|iPhone|iPod/.test(ua) && !window.MSStream) {
                iosBtn.classList.add("recommended");
                statusText.textContent = "Optimized for your iPhone or iPad";
            } else if (/android/i.test(ua)) {
                androidBtn.classList.add("recommended");
                statusText.textContent = "Optimized for your Android device";
            }
        })();
    </script>

</body>
</html>
