<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://github.com/banebounce-MAIN/BaneBounce/blob/main/Logo.jpg">
        <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #6ecbf5 0%, #ff9de9 100%);
            color: #333;
            line-height: 1.6;
            text-align: center;
        }
        
        header {
            background: linear-gradient(to right, #ff5e8e, #ff9a3d);
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
            position: relative;
            overflow: hidden;
        }
        
        .logo-container {
            display: flex;
            align-items: center;
        }
        
        .logo {
            width: 60px;
            height: 60px;
            background: linear-gradient(45deg, #ff9a3d, #ff5e8e);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin-right: 15px;
            border: 3px solid white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
        }
        
        .logo i {
            font-size: 28px;
            color: white;
        }
        
        .logo-text {
            text-align: left;
        }
        
        .logo-text h1 {
            font-size: 1.8rem;
            margin: 0;
            text-shadow: 2px 2px 0px #ff5e8e;
        }
        
        .logo-text p {
            font-size: 0.9rem;
            margin: 0;
            opacity: 0.9;
        }
        
        nav a {
            margin: 0 10px;
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            border-radius: 20px;
            transition: all 0.3s;
        }
        
        nav a:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-2px);
        }
        
        .hero {
            background: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('https://images.unsplash.com/photo-1571019613454-1cb2f99b2d8b') no-repeat center/cover;
            color: white;
            padding: 100px 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
            position: relative;
        }
        
        .hero h2 {
            font-size: 2.8rem;
            margin: 0 0 20px 0;
            color: #fff;
            text-shadow: 3px 3px 0px #ff5e8e;
        }
        
        .hero p {
            font-size: 1.4rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            margin-top: 20px;
            padding: 15px 30px;
            background: #ff5e8e;
            color: white;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.2rem;
            box-shadow: 0 4px 0 #d1386c;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 0 #d1386c;
            background: #ff4780;
        }
        
        .btn:active {
            transform: translateY(1px);
            box-shadow: 0 2px 0 #d1386c;
        }
        
        .section {
            padding: 70px 20px;
        }
        
        .section-title {
            font-size: 2.5rem;
            margin-bottom: 40px;
            color: #ff5e8e;
            text-shadow: 2px 2px 0px #ffd166;
        }
        
        .container {
            max-width: 1100px;
            margin: 0 auto;
        }
        
        .card {
            background: white;
            border-radius: 20px;
            padding: 30px;
            max-width: 500px;
            margin: 0 auto;
            box-shadow: 0 10px 30px rgba(0,0,0,0.15);
            border: 5px solid #ffd166;
            transition: transform 0.3s;
        }
        
        .card:hover {
            transform: translateY(-10px);
        }
        
        .card h3 {
            font-size: 1.8rem;
            color: #ff5e8e;
            margin-bottom: 15px;
        }
        
        .card p {
            margin-bottom: 20px;
            font-size: 1.1rem;
        }
        
        .price {
            font-size: 2.2rem;
            color: #06d6a0;
            font-weight: bold;
            margin: 15px 0;
            text-shadow: 2px 2px 0px #e6e6e6;
        }
        
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 25px;
            margin: 40px 0;
        }
        
        .feature {
            flex: 1;
            min-width: 250px;
            background: white;
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .feature i {
            font-size: 3rem;
            color: #6ecbf5;
            margin-bottom: 15px;
        }
        
        .castle-showcase {
            margin: 50px 0;
            padding: 30px;
            background: linear-gradient(to right, #06d6a0, #6ecbf5);
            border-radius: 20px;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        
        .castle-showcase img {
            max-width: 100%;
            border-radius: 15px;
            border: 5px solid white;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }
        
        .contact-info {
            line-height: 1.8;
            font-size: 1.2rem;
            margin: 20px 0;
        }
        
        .contact-info i {
            width: 30px;
            color: #ff5e8e;
        }
        
        footer {
            background: #333;
            color: white;
            padding: 30px 20px;
            margin-top: 40px;
        }
        
        .bounce {
            animation: bounce 2s infinite;
        }
        
        @keyframes bounce {
            0%, 20%, 50%, 80%, 100% {transform: translateY(0);}
            40% {transform: translateY(-20px);}
            60% {transform: translateY(-10px);}
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0% {transform: translateY(0px);}
            50% {transform: translateY(-15px);}
            100% {transform: translateY(0px);}
        }
        
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                padding: 15px;
            }
            
            .logo-container {
                margin-bottom: 15px;
            }
            
            nav {
                width: 100%;
                display: flex;
                justify-content: space-around;
            }
            
            .hero h2 {
                font-size: 2rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo-container">
            <div class="logo">
                <i class="fas fa-cloud"></i>
            </div>
            <div class="logo-text">
                <h1>Bane Bounce</h1>
                <p>Jumping Castle Fun!</p>
            </div>
        </div>
        <nav>
            <a href="#services">Services</a>
            <a href="#pricing">Pricing</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero">
        <h2>Make Every Party Unforgettable! 🎉</h2>
        <p>Fun and safe jumping castle for kids' birthdays, school events, and more!</p>
        <a href="#contact" class="btn bounce"><i class="fas fa-ticket-alt"></i> Book Now!</a>
    </section>

    <section id="services" class="section">
        <h2 class="section-title">Our Service</h2>
        <div class="container">
            <p>We provide a reliable, high-quality jumping castle for events in Pretoria & Gauteng. Perfect for birthdays, community events, or any special celebration!</p>
            
            <div class="features">
                <div class="feature floating">
                    <i class="fas fa-shield-alt"></i>
                    <h3>Safe & Clean</h3>
                    <p>Thoroughly cleaned and safety checked before every event</p>
                </div>
                <div class="feature floating" style="animation-delay: 0.5s;">
                    <i class="fas fa-truck"></i>
                    <h3>Delivery & Setup</h3>
                    <p>We deliver, set up, and collect - hassle free!</p>
                </div>
                <div class="feature floating" style="animation-delay: 1s;">
                    <i class="fas fa-star"></i>
                    <h3>Premium Quality</h3>
                    <p>Well-maintained castle that kids absolutely love</p>
                </div>
            </div>
        </div>
    </section>

    <section class="castle-showcase">
        <div class="container">
            <h2 class="section-title">Our Amazing Castle!</h2>
            <img src="section id="pricing" class="section">
        <h2 class="section-title">Pricing</h2>
        <div class="card">
            <h3>3x3m Jumping Castle</h3>
            <p>Perfect size for most parties and gatherings. Includes delivery, setup, and collection within Pretoria.</p>
            <div class="price">R670 per day PRETORIA</div>" 
            <a href="#contact" class="btn">Book This Castle</a>
        </div>
    </section>
            <p style="margin-top: 20px; font-size: 1.2rem; color: white; text-shadow: 1px 1px 2px rgba(0,0,0,0.5);">Our vibrant 3x3m castle guarantees hours of bouncing fun!</p>
        </div>
<section id="pricing" class="section">
        <h2 class="section-title">Pricing</h2>
           <div class="card">
            <h3>3x3m Jumping Castle</h3>
            <p>Perfect size for most parties and gatherings. Includes delivery, setup, and collection within Joburg.</p>
         <div class="price">R750 per day</div>
            <a href="#contact" class="btn">Book This Castle</a>
        </div>
    </section>

    <section id="contact" class="section">
        <h2 class="section-title">Contact Us</h2>
        <div class="card">
            <div class="contact-info">
                <p><i class="fas fa-phone"></i> Call: 067 688 9364</p>
                <p><i class="fas fa-envelope"></i> Email: banebounce@gmail.co.za</p>
                <p><i class="fas fa-map-marker-alt"></i> Based in Pretoria, Gauteng</p>
            </div>
            <a href="https://wa.me/+27761 973 1266" class="btn" style="background: #25D366;"><i class="fab fa-whatsapp"></i> Message on WhatsApp</a>
        </div>
    </section>

    <footer>
        <p>© 2025 Bane Bounce. All Rights Reserved.</p>
        <p>Making parties fun and memorable!</p>
    </footer>

    <script>
        // Simple animation for the booking buttons
        document.querySelectorAll('.btn').forEach(btn => {
            btn.addEventListener('mouseover', () => {
                btn.style.transform = 'translateY(-3px)';
            });
            
            btn.addEventListener('mouseout', () => {
                btn.style.transform = 'translateY(0)';
            });
        });
    </script>
</body>
</html>
