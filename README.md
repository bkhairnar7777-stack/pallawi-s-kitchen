[index.html](https://github.com/user-attachments/files/25316263/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pallawi'S Kitchen | Delicious Fast Food</title>
    <style>
        :root {
            --primary-red: #b30000; /* Deep Red */
            --accent-gold: #d4a373; /* Golden accent */
            --dark: #1a1a1a;
            --light-bg: #fdfdfd;
        }

        body { font-family: 'Segoe UI', Arial, sans-serif; margin: 0; line-height: 1.6; color: #333; background-color: var(--light-bg); scroll-behavior: smooth; }
        
        /* Navigation */
        nav { background-color: var(--dark); padding: 1rem; position: sticky; top: 0; z-index: 1000; display: flex; justify-content: space-around; align-items: center; border-bottom: 3px solid var(--primary-red); }
        nav a { color: white; text-decoration: none; font-weight: bold; text-transform: uppercase; font-size: 0.85rem; letter-spacing: 1px; }
        nav a:hover { color: var(--accent-gold); }

        /* Hero Section */
        .hero { 
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('https://images.unsplash.com/photo-1513104890138-7c749659a591?auto=format&fit=crop&w=1200&q=80'); 
            background-size: cover; background-position: center; height: 70vh; 
            display: flex; align-items: center; justify-content: center; color: white; text-align: center; 
        }
        .hero h1 { font-size: 3.5rem; margin-bottom: 0; color: var(--accent-gold); text-shadow: 2px 2px 4px #000; }
        .hero p { font-size: 1.2rem; font-style: italic; margin-top: 10px; }

        /* Menu Section */
        section { padding: 4rem 1rem; max-width: 1100px; margin: 0 auto; }
        .section-title { text-align: center; margin-bottom: 3rem; position: relative; }
        .section-title::after { content: ''; width: 60px; height: 3px; background: var(--primary-red); position: absolute; bottom: -10px; left: 50%; transform: translateX(-50%); }

        .menu-container { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; }
        
        .menu-item { 
            background: #fff; border-radius: 12px; overflow: hidden; 
            box-shadow: 0 4px 15px rgba(0,0,0,0.05); border: 1px solid #eee; transition: 0.3s;
        }
        .menu-item:hover { transform: translateY(-5px); box-shadow: 0 8px 25px rgba(179, 0, 0, 0.2); }
        .menu-item img { width: 100%; height: 220px; object-fit: cover; border-bottom: 4px solid var(--primary-red); }
        .menu-info { padding: 1.5rem; }
        .menu-info h3 { margin: 0; color: var(--dark); }
        .price-tag { color: var(--primary-red); font-weight: bold; font-size: 1.25rem; display: block; margin-top: 10px; }

        /* Contact Section */
        #contact { background-color: #fff4f4; border-radius: 20px; margin-bottom: 4rem; padding: 3rem; }
        .contact-flex { display: flex; flex-wrap: wrap; gap: 40px; }
        .contact-info { flex: 1; min-width: 280px; }
        .btn { background: var(--primary-red); color: white; padding: 12px 25px; text-decoration: none; border-radius: 5px; display: inline-block; margin-top: 20px; }

        footer { background-color: var(--dark); color: white; text-align: center; padding: 2rem; border-top: 5px solid var(--primary-red); }
        
        @media (max-width: 600px) {
            .hero h1 { font-size: 2.2rem; }
        }
    </style>
</head>
<body>

    <nav>
        <a href="#home">Home</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Contact</a>
        <a href="https://www.instagram.com/pallawiskitchen_0109" target="_blank">Instagram</a>
    </nav>
    
    <section id="home" class="hero" style="max-width: 100%; padding: 0;">
        <div class="hero-content">
            <h1>Pallawi'S Kitchen</h1>
            <p>Delicious Fast Food Ever | Pizza starting at ₹99</p>
            <a href="#menu" class="btn">View Menu</a>
        </div>
    </section>
    
    <section id="menu">
        <h2 class="section-title">Our Specials</h2>
        <div class="menu-container">
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1565299624946-b28f40a0ae38?auto=format&fit=crop&w=500&q=80" alt="Cheesy Pizza">
                <div class="menu-info">
                    <h3>Cheesy Pasta Pizza</h3>
                    <p>Our signature fusion pizza loaded with cheese and pasta.</p>
                    <span class="price-tag">Starting at ₹99</span>
                </div>
            </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1571091718767-18b5b1457add?auto=format&fit=crop&w=500&q=80" alt="Veg Burger">
                <div class="menu-info">
                    <h3>Veggie Crunch Burger</h3>
                    <p>Classic crispy patty with fresh veggies and special sauce.</p>
                    <span class="price-tag">Best Price</span>
                </div>
            </div>
            <div class="menu-item">
                <img src="https://images.unsplash.com/photo-1612927601601-6638404737ce?auto=format&fit=crop&w=500&q=80" alt="Magic Maggi">
                <div class="menu-info">
                    <h3>Magic Maggi Pizza</h3>
                    <p>A unique combination for noodle and pizza lovers.</p>
                    <span class="price-tag">Hot & Fresh</span>
                </div>
            </div>
        </div>
    </section>
    
    <section id="contact">
        <div class="contact-flex">
            <div class="contact-info">
                <h2 style="color: var(--primary-red);">Visit Us</h2>
                <p><strong>Address:</strong> Pandesara, Surat, Gujarat</p>
                <p><strong>Phone:</strong> +91 9274786484</p>
                <p><strong>Instagram:</strong> @pallawiskitchen_0109</p>
                <a href="tel:9274786484" class="btn">Order Now</a>
            </div>
            <div style="flex: 1.5; min-width: 300px; border-radius: 15px; overflow: hidden; height: 300px; background: #ddd;">
                <div style="width:100%; height:100%; display:flex; align-items:center; justify-content:center; background:#eee; border:1px solid #ccc;">
                    Map Location: Pandesara, Surat
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <p>© 2026 Pallawi'S Kitchen. All rights reserved.</p>
        <p><small>Follow us on Instagram: pallawiskitchen_0109</small></p>
    </footer>

</body>
</html>
<section id="full-menu" style="background-color: #fff;">
        <h2 class="section-title">Our Full Menu</h2>
        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 40px;">
            
            <div>
                <h3 style="color: var(--primary-red); border-bottom: 2px solid var(--accent-gold); padding-bottom: 5px;">Pizzas</h3>
                <ul style="list-style: none; padding: 0;">
                    <li style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <span>Cheesy Pasta Pizza</span> <strong>₹99</strong>
                    </li>
                    <li style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <span>Magic Maggi Pizza</span> <strong>₹120</strong>
                    </li>
                    <li style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <span>Classic Margherita</span> <strong>₹99</strong>
                    </li>
                </ul>
            </div>

            <div>
                <h3 style="color: var(--primary-red); border-bottom: 2px solid var(--accent-gold); padding-bottom: 5px;">Sides & Snacks</h3>
                <ul style="list-style: none; padding: 0;">
                    <li style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <span>Veg Burger</span> <strong>₹60</strong>
                    </li>
                    <li style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <span>Locho (Oil)</span> <strong>₹40</strong>
                    </li>
                    <li style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                        <span>Manchow Soup</span> <strong>₹50</strong>
                    </li>
                </ul>
            </div>

        </div>
        <p style="text-align: center; margin-top: 30px; font-style: italic;">*Prices are subject to change. Visit us for daily specials!</p>
    </section>
/* Floating WhatsApp Button */
.whatsapp-float {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #25d366;
    color: white;
    width: 60px;
    height: 60px;
    border-radius: 50px;
    text-align: center;
    font-size: 30px;
    box-shadow: 2px 2px 10px rgba(0,0,0,0.2);
    z-index: 1000;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    transition: transform 0.3s;
}

.whatsapp-float:hover {
    transform: scale(1.1);
    background-color: #128c7e;
}

.whatsapp-text {
    font-size: 12px;
    font-weight: bold;
}
<a href="https://wa.me/919274786484?text=Hello%20Pallawi'S%20Kitchen,%20I%20want%20to%20place%20an%20order!" 
   class="whatsapp-float" 
   target="_blank">
   <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp" style="width: 35px; height: 35px;">
</a>
