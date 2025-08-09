<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eslam Abdelbasset - Senior Backend Engineer</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://unpkg.com/typed.js@2.0.16/dist/typed.umd.js"></script>
    <style>
        :root {
            --primary: #1a1b27;
            --secondary: #2d2e3f;
            --accent: #4f46e5;
            --text: #e2e8f0;
            --text-secondary: #a0aec0;
            --success: #10b981;
            --warning: #f59e0b;
            --danger: #ef4444;
            --info: #3b82f6;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: var(--primary);
            color: var(--text);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .rainbow {
            height: 8px;
            background: linear-gradient(90deg, #ff9aa2, #ffb7b2, #ffdac1, #e2f0cb, #b5ead7, #c7ceea);
            width: 100%;
            margin: 0 auto;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .hero {
            text-align: center;
            padding: 40px 0;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            min-height: 80px;
        }
        
        .profile-widget {
            max-width: 600px;
            margin: 30px auto;
            background: var(--secondary);
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .section-title {
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            margin: 40px 0 30px;
        }
        
        .section-title img {
            height: 40px;
            margin-right: 15px;
        }
        
        .about-card {
            background: var(--secondary);
            border-radius: 15px;
            padding: 30px;
            margin: 20px 0;
            position: relative;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .about-card::before {
            content: '';
            position: absolute;
            top: 0;
            right: 0;
            height: 100%;
            width: 50px;
            background: linear-gradient(180deg, #4f46e5, #7c3aed);
            z-index: 0;
        }
        
        .about-content {
            position: relative;
            z-index: 1;
        }
        
        .about-content h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }
        
        .about-content h3 i {
            margin-right: 10px;
            color: var(--info);
        }
        
        .about-content ul {
            list-style: none;
            padding-left: 20px;
        }
        
        .about-content li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
        }
        
        .about-content li::before {
            content: '•';
            position: absolute;
            left: 0;
            color: var(--accent);
            font-size: 1.5rem;
        }
        
        .portfolio-btn {
            display: inline-block;
            background: linear-gradient(45deg, var(--accent), #7c3aed);
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 20px;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(79, 70, 229, 0.4);
        }
        
        .portfolio-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(79, 70, 229, 0.6);
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        
        .skill-category {
            background: var(--secondary);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .skill-category h3 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }
        
        .skill-category h3 i {
            margin-right: 10px;
        }
        
        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .badge {
            background: rgba(79, 70, 229, 0.15);
            color: var(--text);
            padding: 8px 15px;
            border-radius: 50px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            border: 1px solid rgba(79, 70, 229, 0.3);
        }
        
        .badge i {
            margin-right: 5px;
        }
        
        .stats-section {
            margin: 50px 0;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }
        
        .stat-card {
            background: var(--secondary);
            border-radius: 15px;
            padding: 25px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .stat-card img {
            width: 100%;
            border-radius: 10px;
        }
        
        .views-counter {
            background: var(--secondary);
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            margin: 30px auto;
            max-width: 600px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 40px 0;
            flex-wrap: wrap;
        }
        
        .social-link {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: var(--secondary);
            color: white;
            font-size: 1.5rem;
            text-decoration: none;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .social-link:hover {
            transform: translateY(-5px);
        }
        
        .linkedin { background: linear-gradient(45deg, #0077B5, #00a0dc); }
        .email { background: linear-gradient(45deg, #D44638, #EA4335); }
        .facebook { background: linear-gradient(45deg, #1877F2, #3b5998); }
        .whatsapp { background: linear-gradient(45deg, #25D366, #128C7E); }
        
        .divider {
            height: 2px;
            background: linear-gradient(90deg, transparent, var(--accent), transparent);
            margin: 30px auto;
            max-width: 800px;
        }
        
        .waving-footer {
            height: 80px;
            background: linear-gradient(180deg, var(--accent), #7c3aed);
            border-radius: 0 0 15px 15px;
            margin-top: 50px;
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .skills-grid {
                grid-template-columns: 1fr;
            }
            
            .stats-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Rainbow Header -->
    <div class="rainbow"></div>
    
    <div class="container">
        <!-- Hero Section -->
        <section class="hero">
            <h1 id="typed-text"></h1>
            <div class="profile-widget">
                <img src="https://github-widgetbox.vercel.app/api/profile?username=eslamabdelbasset1&data=followers,repositories,stars,commits&theme=viridescent" alt="GitHub Stats">
            </div>
        </section>
        
        <!-- My Information Section -->
        <div class="section-title">
            <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="40">
            <h2>MY INFORMATION</h2>
        </div>
        
        <div class="about-card">
            <div class="about-content">
                <h3><i class="fas fa-laptop-code"></i> About Me</h3>
                <ul>
                    <li><strong>🚀 Expertise:</strong> Building scalable backend systems with PHP, Laravel, MySQL, Docker, and RESTful APIs</li>
                    <li><strong>🔍 Focus:</strong> Optimizing backend infrastructure and API performance</li>
                    <li><strong>🌱 Continuous Growth:</strong> Expanding full-stack knowledge while staying updated with emerging tech</li>
                    <li><strong>❤ Passion:</strong> Back-end Developer | PHP & Laravel | Building immersive web applications</li>
                    <li><strong>🎓 Education:</strong> Bachelor's in Computer Science from Modern Academy for Science and Technology</li>
                    <li><strong>💡 Problem Solver:</strong> Thrive on complex challenges and mentoring junior developers</li>
                </ul>
                <a href="https://eslamabdelbasset.netlify.app" class="portfolio-btn" target="_blank">View My Portfolio</a>
            </div>
        </div>
        
        <!-- Skills Section -->
        <div class="section-title">
            <h2>SKILLS & TECHNOLOGIES</h2>
        </div>
        
        <div class="skills-grid">
            <!-- Languages -->
            <div class="skill-category">
                <h3><i class="fas fa-globe"></i> Languages</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fab fa-php"></i> PHP</span>
                    <span class="badge"><i class="fab fa-js"></i> JavaScript</span>
                    <span class="badge"><i class="fab fa-js"></i> TypeScript</span>
                    <span class="badge"><i class="fas fa-code"></i> C#</span>
                    <span class="badge"><i class="fas fa-code"></i> C++</span>
                    <span class="badge"><i class="fab fa-html5"></i> HTML</span>
                    <span class="badge"><i class="fab fa-css3"></i> CSS</span>
                </div>
            </div>
            
            <!-- Frameworks -->
            <div class="skill-category">
                <h3><i class="fas fa-layer-group"></i> Frameworks</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fab fa-bootstrap"></i> Bootstrap</span>
                    <span class="badge"><i class="fab fa-js"></i> jQuery</span>
                    <span class="badge"><i class="fab fa-sass"></i> Sass</span>
                    <span class="badge"><i class="fab fa-angular"></i> Angular</span>
                    <span class="badge"><i class="fab fa-laravel"></i> Laravel</span>
                    <span class="badge"><i class="fas fa-server"></i> NestJS</span>
                    <span class="badge"><i class="fab fa-node-js"></i> Express.js</span>
                    <span class="badge"><i class="fas fa-palette"></i> Material UI</span>
                </div>
            </div>
            
            <!-- Databases -->
            <div class="skill-category">
                <h3><i class="fas fa-database"></i> Databases</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fas fa-database"></i> MySQL</span>
                    <span class="badge"><i class="fas fa-database"></i> SQLite</span>
                </div>
            </div>
            
            <!-- Tools -->
            <div class="skill-category">
                <h3><i class="fas fa-tools"></i> Tools</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fab fa-git"></i> Git</span>
                    <span class="badge"><i class="fab fa-github"></i> GitHub</span>
                    <span class="badge"><i class="fab fa-markdown"></i> Markdown</span>
                    <span class="badge"><i class="fas fa-cpanel"></i> cPanel</span>
                    <span class="badge"><i class="fas fa-code"></i> VS Code</span>
                    <span class="badge"><i class="fas fa-jet-fighter"></i> PhpStorm</span>
                    <span class="badge"><i class="fas fa-paper-plane"></i> Postman</span>
                    <span class="badge"><i class="fas fa-server"></i> Xampp</span>
                    <span class="badge"><i class="fas fa-server"></i> Nginx</span>
                    <span class="badge"><i class="fab fa-docker"></i> Docker</span>
                </div>
            </div>
            
            <!-- CI/CD -->
            <div class="skill-category">
                <h3><i class="fas fa-sync-alt"></i> CI/CD</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fab fa-github"></i> GitHub Actions</span>
                </div>
            </div>
            
            <!-- Hosting -->
            <div class="skill-category">
                <h3><i class="fas fa-cloud"></i> Hosting</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fab fa-heroku"></i> Heroku</span>
                    <span class="badge"><i class="fas fa-server"></i> Vercel</span>
                </div>
            </div>
            
            <!-- Design -->
            <div class="skill-category">
                <h3><i class="fas fa-paint-brush"></i> Design</h3>
                <div class="badge-container">
                    <span class="badge"><i class="fab fa-adobe"></i> Adobe XD</span>
                </div>
            </div>
        </div>
        
        <div class="rainbow"></div>
        
        <!-- GitHub Stats Section -->
        <div class="section-title">
            <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExYzFhYzJkMmQ2MWQ3ZGY3MDhjZTE3MDI2Mzk3NzE1OWQyZTRlMmYwMCZjdD1z/iY8CRBdQXODJSCERIr/giphy.gif" width="40">
            <h2>GITHUB STATISTICS</h2>
        </div>
        
        <div class="views-counter">
            <p><i class="fas fa-eye"></i> Profile Views: <strong>5,280</strong></p>
            <p><i class="fas fa-sync-alt"></i> Last Updated: <strong>Today</strong></p>
        </div>
        
        <div class="stats-grid">
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api?username=eslamabdelbasset1&theme=dark&hide_border=false&include_all_commits=false&count_private=false" alt="GitHub Stats">
            </div>
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=eslamabdelbasset1&theme=dark&border_radius=10&hide_title=true&layout=compact&langs_count=20" alt="Top Languages">
            </div>
            <div class="stat-card">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=eslamabdelbasset1&theme=dark&hide_border=false" alt="GitHub Streak">
            </div>
            <div class="stat-card">
                <img src="http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=eslamabdelbasset1&theme=dark" alt="Profile Details">
            </div>
        </div>
        
        <div class="rainbow"></div>
        
        <!-- Connect Section -->
        <div class="section-title">
            <h2>CONNECT WITH ME</h2>
        </div>
        
        <div class="social-links">
            <a href="https://www.linkedin.com/in/eslamabdelbasset" class="social-link linkedin" target="_blank">
                <i class="fab fa-linkedin-in"></i>
            </a>
            <a href="mailto:eslamabdelbasset1@gmail.com" class="social-link email">
                <i class="fas fa-envelope"></i>
            </a>
            <a href="https://www.facebook.com/eslam3bdelbasset" class="social-link facebook" target="_blank">
                <i class="fab fa-facebook-f"></i>
            </a>
            <a href="https://api.whatsapp.com/send/?phone=201060838210" class="social-link whatsapp" target="_blank">
                <i class="fab fa-whatsapp"></i>
            </a>
        </div>
        
        <div class="divider"></div>
    </div>
    
    <!-- Waving Footer -->
    <div class="waving-footer"></div>
    
    <script>
        // Typed.js initialization
        document.addEventListener('DOMContentLoaded', function() {
            const typed = new Typed('#typed-text', {
                strings: ["Hi There! 👋", "I'm Eslam Abdelbasset"],
                typeSpeed: 70,
                backSpeed: 40,
                loop: true,
                showCursor: true,
                cursorChar: '|',
                autoInsertCss: true
            });
        });
        
        // Simple counter animation
        const counters = document.querySelectorAll('.views-counter strong');
        counters.forEach(counter => {
            const target = counter.textContent === '5,280' ? 5280 : 0;
            let count = 0;
            
            const updateCounter = () => {
                const increment = target / 50;
                count += increment;
                
                if (count < target) {
                    counter.textContent = Math.ceil(count).toLocaleString();
                    setTimeout(updateCounter, 20);
                } else {
                    counter.textContent = target.toLocaleString();
                }
            };
            
            updateCounter();
        });
    </script>
</body>
</html>
