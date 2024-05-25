# Tech_Haven


##A tech company website made using HTML & CSS

HTML FILE:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Haven</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link rel="stylesheet" href="Tech_Haven.css">
</head>
<body>
    <header>
        <div class="navbar">
            <h1><span class="navbar-logo">Tech Haven</span></h1>
            <a href="#home">Home</a>
            <a href="#about">About Us</a>
            <a href="#models">Products Available</a>
            <a href="#contact">Contact us</a>
            <a class="nav-cart border">Cart
                <i class="fa-solid fa-cart-shopping"></i>  
                </a>
            
            <div class="nav-search">
            <select class="search-select">
                <option>All</option>
            </select>
            <input placeholder="Search Tech Haven" class="search-input">
            <div class="search-icon">
                <i class="fa-solid fa-magnifying-glass"></i>
            </div>
        </div>
    </div>
    </header>
    <section id="about">
        <div class="container">
            <h2>About Us</h2>
            <p>Tech Haven is a pioneering tech company committed to transforming the digital landscape through innovation and expertise. With a focus on creating seamless technological solutions, Tech Haven endeavors to simplify complexities and empower individuals and businesses alike. From cutting-edge software development to revolutionary hardware solutions, Tech Haven's dedication to excellence ensures that it remains at the forefront of technological advancement. With a team of highly skilled professionals and a passion for pushing boundaries, Tech Haven is poised to shape the future of technology, making the world a more connected, efficient, and secure place for all..</p>
        </div>
    </section>

    <section id="services">

        <div class="container">
            <h2>Our Services</h2>
            
            <div class="services-container">
                <div class="service">
                    <h3>Web Development</h3>
                    <div class="box-img" style="background-image:url('webdev.jpg');"></div>
                    <p>We create stunning websites tailored to your needs, ensuring a seamless user experience.</p>
                </div>
                <div class="service">
                    
                    <h3>Mobile App Development</h3>
                    <div class="box-img" style="background-image:url('appdev.jpg');"></div>
                    <p>From iOS to Android, we develop cutting-edge mobile applications that elevate your brand.</p>
                </div>
                <div class="service">
                    
                    <h3>Consulting</h3>
                    <div class="box-img" style="background-image:url('consulting.jpg');"></div>
                    <p>Our experts provide strategic guidance and technology consulting to drive your business forward.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Ready to start your next project with us? Reach out to our team today!</p>
            <form id="contact-form">
                <input type="text" id="name" placeholder="Name" required>
                <input type="email" id="email" placeholder="Email" required>
                <textarea id="message" placeholder="Message" required></textarea>
                <button type="submit">Send</button>
            </form>
        </div>
    </section>

    <footer>

        <footer>
            <div class="foot-panel1">
                Back to Top
            </div>
            <div class="foot-panel2">
                <ul>
                    <p>Get to Know Us</p>
                    <a>What's new</a>
                 <a>Surface Pro 9</a>
                 <a>Surface Laptop 5</a>
                 <a>Surface Laptop Go 2</a>
                 <a>Microsoft Copilot</a>
                <a>Microsoft 365</a>  
            </ul>
                <ul>
                   <p>Company</p> 
                    <a>Careers</a>
                    <a>About Microsoft</a>
                    <a>Company news</a>
                    <a>Privacy at Tevh Haven</a>
                    </ul>
                    <ul>
                        <p>Business</p>
                         <a>About Us</a>
                         <a>Careers</a>
                         <a>Press Releases</a>
                         <a>Sciences</a>
                        </ul>
                        <ul>
                            <p>Developer Center</p>
                             <a>About Us</a>
                             <a>Careers</a>
                             <a>Press Releases</a>
                             <a>Sciences</a>
                            </ul>
            </div>
            <div class="foot-panel4">
                <div class="pages">
        <a>Conditions of Use</a>
        <a>Privacy Notice</a>
        <a>Your Ads Privacy Choices</a>
        
                </div>
                <div class="copyright">
                    &copy; 2024 Tech Haven. All rights reserved.
                </div>
            </div>
        </footer>
</body>
</html>





CSS CODE:



    /* Reset default margin and padding */
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    /* Navbar styles */
    .navbar {
        background-color: #333;
        overflow: hidden;
    }

    .navbar-logo {
        font-weight: bold;
        color: white;
        padding: 10px 20px;
        float: left;
    }

    .navbar a {
        float: left;
        font-size: 1rem;
        color: #f2f2f2;
        text-align: center;
        padding: 14px 16px;
        text-decoration: none;
        margin-right: 30px;
    }

    .navbar a:hover {
        background-color: #ddd;
        color: black;
    }

    .box-img {
        height: 300px;
        background-size: cover;
        margin-top: 1rem;
        margin-bottom: 1rem;
    }

    /* Active link style */
    .navbar a.active {
        background-color: #ddd;
        color: black;
        border-radius: 5px;
    }

    /** box 3**/
.nav-search {
    display: flex;
    justify-content: space-evenly;
    background-color: pink;
    width: 620px;
    height: 40px;
    border-radius: 4px;
    justify-content: space-evenly;
}

.search-select {
    background-color: #f3f3f3;
    width: 50px;
    text-align: center;
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;
    border: none;
}

.search-input {
    width: 100%;
    font-size: 1rem;
    border: none;
}

.search-icon {
    width: 45px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 1.2rem;
    background-color:orange;
    border-top-left-radius: 4px;
    border-bottom-left-radius: 4px;
    color: #0f1111;
}

.nav-search:hover {
    border: 2px solid orange;
}




/* Reset CSS */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Global Styles */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background-color: #f8f8f8;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

header {
    background: #333;
    color: #fff;
    padding: 20px 0;
    position: fixed;
    width: 100%;
    z-index: 1000;
}

header h1 {
    margin: 0;
}

nav ul {
    list-style: none;
}

nav ul li {
    display: inline;
    margin-right: 20px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    transition: color 0.3s ease;
}

nav ul li a:hover {
    color: #ffd700;
}

section {
    padding: 80px 0;
}

h2 {
    margin-bottom: 40px;
    color: #333;
}

.services-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

.service {
    flex: 0 0 calc(33.333% - 20px);
    background-color: #fff;
    border-radius: 8px;
    padding: 20px;
    margin-bottom: 40px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.service:hover {
    transform: translateY(-5px);
}

.service h3 {
    margin-bottom: 10px;
    color: #333;
}

.service p {
    color: #666;
}

#contact-form {
    max-width: 500px;
    margin: 0 auto;
}

#contact-form input,
#contact-form textarea,
#contact-form button {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #fff;
}

#contact-form button {
    background-color: #333;
    color: #fff;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

#contact-form button:hover {
    background-color: #ffd700;
}

.footer {
    margin-top: 15px;
}

.foot-panel1 {
    background-color: #37475a;
    color: white;
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 0.85rem;
}

.foot-panel2 {
    background-color:#333;
    color: white;
    height: 300px;
    display: flex;
    justify-content: space-evenly;
}

ul {
    margin-top: 20px;
}

ul a {
    display: block;
    font-size: 0.85rem;
    margin-top: 10px;
    color: #dddddd;
}

.foot-panel4 {
    background-color: #0f1111;
    color: white;
    height: 100px;
    font-size: 0.7rem;
    text-align: center;
}

.pages {
    font-size: 0.7rem;
    text-align: center;
    padding-top: 25px;
}

.copyright {
    padding-top: 5px;
}

/* Slide in animation for navbar */
@keyframes slideInNav {
    from {
        opacity: 0;
        transform: translateY(-100%);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* Fade in animation for nav-second */
@keyframes fadeInNavSecond {
    from {
        opacity: 0;
    }
    to {
        opacity: 1;
    }
}

/* Blink animation for nav-cart */
@keyframes blink {
    0% {
        opacity: 1;
    }
    50% {
        opacity: 0;
    }
    100% {
        opacity: 1;
    }
}

/* Rotate animation for footer logo */
@keyframes rotate {
    0% {
        transform: rotate(0deg);
    }
    100% {
        transform: rotate(360deg);
    }
}

/* Add animations to respective elements */
.navbar {
    animation: slideInNav 0.5s ease-in-out forwards;
}

.nav-second {
    animation: fadeInNavSecond 0.5s ease-in-out forwards;
}

.nav-cart {
    animation: blink 1.5s infinite;
}

.footer .foot-panel3 .logo {
    animation: rotate 4s linear infinite;
}
