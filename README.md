# my-website.
ПОПА
<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Тема: Кріштіану Роналду</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Roboto:wght@300;400;500&display=swap" rel="stylesheet">
    <style>
        :root {
            --cr7-red: #c40303;
            --cr7-dark: #1a1a1a;
            --cr7-gold: #daa520;
            --cr7-light: #f5f5f5;
            --cr7-white: #ffffff;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--cr7-dark);
            color: var(--cr7-light);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header */
        header {
            background: linear-gradient(rgba(26, 26, 26, 0.9), rgba(26, 26, 26, 0.9)), 
                        url('https://images.unsplash.com/photo-1598880940080-ff9a29891b85?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80');
            background-size: cover;
            background-position: center;
            padding: 60px 0 40px;
            text-align: center;
            border-bottom: 5px solid var(--cr7-red);
            position: relative;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        .logo {
            font-size: 3.5rem;
            color: var(--cr7-red);
            margin-bottom: 10px;
        }
        
        h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 3.2rem;
            font-weight: 700;
            margin-bottom: 10px;
            background: linear-gradient(to right, var(--cr7-red), var(--cr7-gold));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        
        .subtitle {
            font-size: 1.4rem;
            color: var(--cr7-gold);
            margin-bottom: 30px;
            font-weight: 300;
        }
        
        /* Stats Section */
        .stats {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
            margin: 40px 0;
        }
        
        .stat-item {
            background-color: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            padding: 25px;
            text-align: center;
            min-width: 200px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid rgba(196, 3, 3, 0.2);
        }
        
        .stat-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(196, 3, 3, 0.2);
        }
        
        .stat-number {
            font-size: 3rem;
            font-weight: 700;
            color: var(--cr7-red);
            margin-bottom: 5px;
        }
        
        .stat-label {
            font-size: 1.1rem;
            color: var(--cr7-gold);
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        /* Profile Section */
        .profile-section {
            display: flex;
            flex-wrap: wrap;
            gap: 40px;
            margin: 60px 0;
            align-items: center;
        }
        
        .profile-image {
            flex: 1;
            min-width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.5);
            border: 3px solid var(--cr7-red);
        }
        
        .profile-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.5s ease;
        }
        
        .profile-image img:hover {
            transform: scale(1.05);
        }
        
        .profile-info {
            flex: 2;
            min-width: 300px;
        }
        
        .profile-info h2 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            color: var(--cr7-red);
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .profile-info h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 80px;
            height: 4px;
            background-color: var(--cr7-gold);
        }
        
        .profile-info p {
            margin-bottom: 20px;
            font-size: 1.1rem;
            color: #ccc;
        }
        
        /* Clubs Section */
        .clubs-section {
            margin: 80px 0;
        }
        
        .section-title {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.5rem;
            color: var(--cr7-gold);
            text-align: center;
            margin-bottom: 50px;
            position: relative;
        }
        
        .section-title:after {
            content: '';
            position: absolute;
            bottom: -15px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background-color: var(--cr7-red);
        }
        
        .clubs {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
        }
        
        .club-card {
            background-color: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            overflow: hidden;
            width: 280px;
            transition: transform 0.3s ease;
            border: 1px solid rgba(196, 3, 3, 0.2);
        }
        
        .club-card:hover {
            transform: translateY(-10px);
        }
        
        .club-logo {
            height: 180px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.03);
        }
        
        .club-logo i {
            font-size: 5rem;
            color: var(--cr7-red);
        }
        
        .club-info {
            padding: 20px;
            text-align: center;
        }
        
        .club-name {
            font-size: 1.5rem;
            color: var(--cr7-white);
            margin-bottom: 10px;
            font-weight: 600;
        }
        
        .club-years {
            color: var(--cr7-gold);
            font-size: 1.1rem;
            margin-bottom: 15px;
        }
        
        /* Achievements */
        .achievements {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin: 60px 0;
        }
        
        .achievement-item {
            background-color: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            padding: 25px;
            border-left: 5px solid var(--cr7-red);
        }
        
        .achievement-icon {
            font-size: 2.5rem;
            color: var(--cr7-gold);
            margin-bottom: 15px;
        }
        
        .achievement-title {
            font-size: 1.5rem;
            color: var(--cr7-white);
            margin-bottom: 10px;
        }
        
        /* Footer */
        footer {
            background-color: rgba(0, 0, 0, 0.7);
            padding: 40px 0;
            text-align: center;
            border-top: 3px solid var(--cr7-red);
            margin-top: 60px;
        }
        
        .footer-logo {
            font-size: 2.5rem;
            color: var(--cr7-red);
            margin-bottom: 20px;
        }
        
        .footer-text {
            color: #aaa;
            margin-bottom: 20px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-icon {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: var(--cr7-white);
            font-size: 1.5rem;
            transition: all 0.3s ease;
        }
        
        .social-icon:hover {
            background-color: var(--cr7-red);
            transform: translateY(-5px);
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .stat-item {
                min-width: 150px;
                padding: 20px;
            }
            
            .stat-number {
                font-size: 2.5rem;
            }
            
            .profile-section {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-futbol"></i>
                </div>
                <h1>Кріштіану Роналду</h1>
                <p class="subtitle">Легенда футболу • Найкращий бомбардир в історії • П'ятиразовий володар Золотого м'яча</p>
                
                <div class="stats">
                    <div class="stat-item">
                        <div class="stat-number">850+</div>
                        <div class="stat-label">Голів за кар'єру</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">5</div>
                        <div class="stat-label">Золотих м'ячів</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">34</div>
                        <div class="stat-label">Трофеї</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">200</div>
                        <div class="stat-label">Матчі за збірну</div>
                    </div>
                </div>
            </div>
        </div>
    </header>
    
    <main class="container">
        <section class="profile-section">
            <div class="profile-image">
                <img src="https://images.unsplash.com/photo-1629757509637-7c99379d6d26?ixlib=rb-4.0.3&auto=format&fit=crop&w=1000&q=80" alt="Кріштіану Роналду">
            </div>
            <div class="profile-info">
                <h2>Про легенду</h2>
                <p>Кріштіану Роналду душ Сантуш Авейру (нар. 5 лютого 1985) — португальський футболіст, нападник саудівського клубу «Ан-Наср» та збірної Португалії. Вважається одним з найкращих футболістів усіх часів.</p>
                <p>Роналду — єдиний футболіст, який виграв чемпіонат Англії, Іспанії та Італії. Він також є рекордсменом за кількістю голів у Лізі чемпіонів УЄФА та найкращим бомбардиром в історії збірних.</p>
                <p>За свою кар'єру він виграв 5 Золотих м'ячів, 4 Золоті бутси та багато інших індивідуальних і командних нагород.</p>
            </div>
        </section>
        
        <section class="clubs-section">
            <h2 class="section-title">Клубна кар'єра</h2>
            <div class="clubs">
                <div class="club-card">
                    <div class="club-logo">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <div class="club-info">
                        <h3 class="club-name">Спортінг</h3>
                        <p class="club-years">2002-2003</p>
                        <p>31 матч, 5 голів</p>
                    </div>
                </div>
                
                <div class="club-card">
                    <div class="club-logo">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <div class="club-info">
                        <h3 class="club-name">Манчестер Юнайтед</h3>
                        <p class="club-years">2003-2009, 2021-2022</p>
                        <p>346 матчів, 145 голів</p>
                    </div>
                </div>
                
                <div class="club-card">
                    <div class="club-logo">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <div class="club-info">
                        <h3 class="club-name">Реал Мадрид</h3>
                        <p class="club-years">2009-2018</p>
                        <p>438 матчів, 450 голів</p>
                    </div>
                </div>
                
                <div class="club-card">
                    <div class="club-logo">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <div class="club-info">
                        <h3 class="club-name">Ювентус</h3>
                        <p class="club-years">2018-2021</p>
                        <p>134 матчі, 101 гол</p>
                    </div>
                </div>
            </div>
        </section>
        
        <section class="achievements-section">
            <h2 class="section-title">Досягнення</h2>
            <div class="achievements">
                <div class="achievement-item">
                    <div class="achievement-icon">
                        <i class="fas fa-trophy"></i>
                    </div>
                    <h3 class="achievement-title">Ліга чемпіонів УЄФА</h3>
                    <p>5 разів: 2008 (Манчестер Юнайтед), 2014, 2016, 2017, 2018 (Реал Мадрид)</p>
                </div>
                
                <div class="achievement-item">
                    <div class="achievement-icon">
                        <i class="fas fa-medal"></i>
                    </div>
                    <h3 class="achievement-title">Чемпіонат Європи</h3>
                    <p>Перемога на Євро-2016 зі збірною Португалії</p>
                </div>
                
                <div class="achievement-item">
                    <div class="achievement-icon">
                        <i class="fas fa-award"></i>
                    </div>
                    <h3 class="achievement-title">Золотий м'яч</h3>
                    <p>5 разів: 2008, 2013, 2014, 2016, 2017</p>
                </div>
                
                <div class="achievement-item">
                    <div class="achievement-icon">
                        <i class="fas fa-futbol"></i>
                    </div>
                    <h3 class="achievement-title">Золота бутса</h3>
                    <p>4 рази: 2008, 2011, 2014, 2015</p>
                </div>
            </div>
        </section>
    </main>
    
    <footer>
        <div class="container">
            <div class="footer-logo">
                <i class="fas fa-futbol"></i>
            </div>
            <p class="footer-text">Ця тема GitHub присвячена одній з найвизначніших футбольних легенд усіх часів - Кріштіану Роналду. Створено з натхненням від його кар'єри та досягнень.</p>
            
            <div class="social-links">
                <a href="#" class="social-icon">
                    <i class="fab fa-github"></i>
                </a>
                <a href="#" class="social-icon">
                    <i class="fab fa-twitter"></i>
                </a>
                <a href="#" class="social-icon">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="#" class="social-icon">
                    <i class="fab fa-youtube"></i>
                </a>
            </div>
            
            <p style="margin-top: 30px; color: #777; font-size: 0.9rem;">© 2023 CR7 GitHub Theme. Усі права захищені.</p>
        </div>
    </footer>

    <script>
        // Анимация для счетчиков статистики
        document.addEventListener('DOMContentLoaded', function() {
            const statItems = document.querySelectorAll('.stat-item');
            
            statItems.forEach(item => {
                item.addEventListener('mouseenter', function() {
                    const numberElement = this.querySelector('.stat-number');
                    const originalText = numberElement.textContent;
                    const number = parseInt(originalText);
                    
                    if (!isNaN(number)) {
                        let current = 0;
                        const increment = Math.ceil(number / 20);
                        const timer = setInterval(() => {
                            current += increment;
                            if (current >= number) {
                                current = number;
                                clearInterval(timer);
                            }
                            numberElement.textContent = current + (originalText.includes('+') ? '+' : '');
                        }, 30);
                    }
                });
            });
            
            // Анимация появления элементов при прокрутке
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };
            
            const observer = new IntersectionObserver(function(entries) {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0)';
                    }
                });
            }, observerOptions);
            
            // Применяем анимацию к элементам
            const animatedElements = document.querySelectorAll('.stat-item, .club-card, .achievement-item');
            animatedElements.forEach(el => {
                el.style.opacity = '0';
                el.style.transform = 'translateY(20px)';
                el.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(el);
            });
        });
    </script>
</body>
</html>
