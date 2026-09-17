<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="View or download Piyush Tak's professional resume. Aspiring AI & ML Engineer with expertise in Python, C, Data Science, and Problem-Solving.">
    <meta name="keywords" content="Piyush Tak, resume, CV, AI engineer, ML engineer, Python developer">
    <meta name="author" content="Piyush Tak">
    <title>Piyush Tak - Resume</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        :root {
            --primary: #007AFF;
            --primary-dark: #0051D5;
            --secondary: #5AC8FA;
            --bg: #ffffff;
            --bg-light: #f8f9fa;
            --text: #1a1a1a;
            --text-light: #666666;
            --border: #e0e0e0;
        }
        @media (prefers-color-scheme: dark) {
            :root {
                --bg: #0a0a0a;
                --bg-light: #1a1a1a;
                --text: #ffffff;
                --text-light: #b0b0b0;
                --border: #333333;
            }
        }
        html {
            scroll-behavior: smooth;
        }
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Helvetica Neue', sans-serif;
            background: linear-gradient(135deg, var(--bg) 0%, var(--bg-light) 100%);
            color: var(--text);
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }
        .container {
            max-width: 700px;
            width: 100%;
            text-align: center;
        }
        /* Header Animation */
        .header {
            animation: slideDown 0.6s ease-out;
            margin-bottom: 40px;
        }
        @keyframes slideDown {
            from {
                opacity: 0;
                transform: translateY(-30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .profile-icon {
            width: 120px;
            height: 120px;
            margin: 0 auto 30px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 60px;
            box-shadow: 0 10px 30px rgba(0, 122, 255, 0.3);
            animation: bounce 2s infinite;
        }
        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
        .name {
            font-size: 48px;
            font-weight: 700;
            color: var(--text);
            margin-bottom: 12px;
            letter-spacing: -0.5px;
        }
        .title {
            font-size: 24px;
            color: var(--primary);
            font-weight: 500;
            margin-bottom: 8px;
        }
        .tagline {
            font-size: 16px;
            color: var(--text-light);
            margin-bottom: 40px;
            line-height: 1.8;
        }
        /* Stats Section */
        .stats {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 50px;
            animation: fadeInUp 0.8s ease-out 0.2s both;
        }
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .stat-card {
            background: var(--bg-light);
            padding: 20px;
            border-radius: 12px;
            border: 1px solid var(--border);
            transition: all 0.3s;
        }
        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 122, 255, 0.15);
            border-color: var(--primary);
        }
        .stat-number {
            font-size: 28px;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 8px;
        }
        .stat-label {
            font-size: 12px;
            color: var(--text-light);
            text-transform: uppercase;
            font-weight: 600;
            letter-spacing: 0.5px;
        }
        /* CTA Button */
        .cta-section {
            animation: fadeInUp 0.8s ease-out 0.4s both;
            margin-bottom: 50px;
        }
        .cta-text {
            font-size: 18px;
            color: var(--text-light);
            margin-bottom: 25px;
            font-weight: 500;
        }
        .button-wrapper {
            display: flex;
            gap: 15px;
            flex-direction: column;
        }
        .btn {
            padding: 16px 40px;
            border-radius: 12px;
            font-size: 16px;
            font-weight: 600;
            text-decoration: none;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            display: inline-block;
            position: relative;
            overflow: hidden;
        }
        .btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: rgba(255, 255, 255, 0.2);
            transition: left 0.3s;
        }
        .btn:hover::before {
            left: 100%;
        }
         btn-primary {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            color: #ffffff;
            box-shadow: 0 8px 20px rgba(0, 122, 255, 0.3);
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 12px 30px rgba(0, 122, 255, 0.4);
        }
        .btn-secondary {
            background: transparent;
            color: var(--primary);
            border: 2px solid var(--primary);
        }
        .btn-secondary:hover {
            background: var(--primary);
            color: #ffffff;
        }
        .btn-icon {
            margin-left: 8px;
            transition: transform 0.3s;
        }
        .btn:hover .btn-icon {
            transform: translateX(3px);
        }
        /* Skills Preview */
        .skills-preview {
            background: var(--bg-light);
            padding: 30px;
            border-radius: 12px;
            border: 1px solid var(--border);
            text-align: left;
            animation: fadeInUp 0.8s ease-out 0.6s both;
            margin-bottom: 40px;
        }
        .skills-title {
            font-size: 16px;
            font-weight: 600;
            color: var(--text);
            margin-bottom: 16px;
            text-align: center;
        }
        .skills-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 12px;
        }
        .skill-tag {
            background: linear-gradient(135deg, rgba(0, 122, 255, 0.1), rgba(90, 200, 250, 0.1));
            color: var(--primary);
            padding: 8px 12px;
            border-radius: 6px;
            font-size: 13px;
            font-weight: 500;
            text-align: center;
            border: 1px solid var(--primary);
            border-opacity: 0.3;
        }
        /* Social Links */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 40px;
            animation: fadeIn 1s ease-out 0.8s both;
        }
        .social-btn {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 20px;
            text-decoration: none;
            background: var(--bg-light);
            color: var(--primary);
            border: 2px solid var(--border);
            transition: all 0.3s;
        }
        .social-btn:hover {
            background: var(--primary);
            color: #ffffff;
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 122, 255, 0.3);
        }
        /* Footer */
        footer {
            font-size: 12px;
            color: var(--text-light);
            text-align: center;
            animation: fadeIn 1s ease-out 1s both;
            padding-top: 20px;
            border-top: 1px solid var(--border);
        }
        /* Responsive */
        @media (max-width: 600px) {
            .name {
                font-size: 36px;
            }
            .title {
                font-size: 18px;
            }
            .tagline {
                font-size: 14px;
            }
            .stats {
                grid-template-columns: 1fr;
            }
            .skills-grid {
                grid-template-columns: 1fr;
            }
            .button-wrapper {
                gap: 12px;
            }
            .btn {
                padding: 14px 30px;
                font-size: 15px;
            }
            .profile-icon {
                width: 100px;
                height: 100px;
                font-size: 48px;
            }
        }
        /* Loading Animation */
        .loading {
            display: inline-block;
            width: 8px;
            height: 8px;
            background: currentColor;
            border-radius: 50%;
            animation: pulse 1.5s infinite;
            margin-left: 8px;
        }
        @keyframes pulse {
            0%, 100% {
                opacity: 1;
            }
            50% {
                opacity: 0.5;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <div class="profile-icon">📄</div>
            <h1 class="name">Piyush Tak</h1>
            <p class="title">Aspiring AI & ML Engineer</p>
            <p class="tagline">2nd-Year CS Student | Python & C Programmer | Data Science Enthusiast</p>
        </div>
        <!-- Stats -->
        <div class="stats">
            <div class="stat-card">
                <div class="stat-number">30%</div>
                <div class="stat-label">Efficiency Gain</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">Top 5%</div>
                <div class="stat-label">Coding Contest</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">20%</div>
                <div class="stat-label">Model Accuracy</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">40%</div>
                <div class="stat-label">Delivery Speed</div>
            </div>
        </div>
        <!-- Skills Preview -->
        <div class="skills-preview">
            <div class="skills-title">Core Skills</div>
            <div class="skills-grid">
                <div class="skill-tag">Python</div>
                <div class="skill-tag">C</div>
                <div class="skill-tag">Data Science</div>
                <div class="skill-tag">Machine Learning</div>
                <div class="skill-tag">Git/GitHub</div>
                <div class="skill-tag">DSA</div>
                <div class="skill-tag">SQL</div>
                <div class="skill-tag">JavaScript</div>
            </div>
        </div>
        <!-- CTA Section -->
        <div class="cta-section">
            <p class="cta-text">Want to know more about me?</p>
            <div class="button-wrapper">
                <a href="https://hilarious-belekoy-b2c70a.netlify.app/" target="_blank" class="btn btn-primary">
                    📥 View My Resume <span class="btn-icon">→</span>
                </a>
                <a href="https://hilarious-belekoy-b2c70a.netlify.app/" download class="btn btn-secondary">
                    ⬇️ Download PDF
                </a>
            </div>
        </div>
        <!-- Social Links -->
        <div class="social-links">
            <a href="mailto:takpiyush10@gmail.com" class="social-btn" title="Email">✉️</a>
            <a href="https://linkedin.com/in/piyush-tak-220b433b7" target="_blank" class="social-btn" title="LinkedIn">🔗</a>
            <a href="https://github.com/takpiyush1" target="_blank" class="social-btn" title="GitHub">💻</a>
            <a href="tel:+918619872787" class="social-btn" title="Phone">📱</a>
        </div>
        <!-- Footer -->
        <footer>
            <p>© 2026 Piyush Tak | Aspiring AI & ML Engineer | Jodhpur, Rajasthan</p>
            <p style="margin-top: 8px;">Built with ❤️ | Free Portfolio</p>
        </footer>
    </div>
    <script>
        // Add smooth scroll to top on load
        window.addEventListener('load', () => {
            window.scrollTo(0, 0);
        });
        // Add click feedback
        document.querySelectorAll('.btn').forEach(btn => {
            btn.addEventListener('click', function() {
                // Visual feedback
                this.style.transform = 'scale(0.98)';
                setTimeout(() => {
                    this.style.transform = '';
                }, 200);
            });
        });
        // Analytics (optional)
        document.querySelectorAll('a[target="_blank"]').forEach(link => {
            link.addEventListener('click', () => {
                console.log('External link clicked:', link.href);
            });
        });
    </script>
</body>
</html>
