<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Foodie</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css" integrity="sha512-Kc323vGBEqzTmouAECnVceyQqyqdsSiqLQISBL29aUW4U/M7pSPA/gEUZQqv1cwx4OnYxTxve5UMg5GT6L4JJg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css" />
    <script src="https://code.jquery.com/jquery-3.7.1.min.js"></script>
</head>
<body>
    <div class="main">
        <nav>
            <div class="logo">Foodie</div>
            <ul class="nav-links">
                <li><a href="#">Home</a></li>
                <li><a href="#">Order</a></li>
                <li><a href="#">Testimonials</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
            <ul class="social-links">
                <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-github"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
            </ul>
        </nav>
        <div class="hero animate__animated animate__zoomIn animate__delay-1">
            <img src="./dishong.png" width="400px" height="430px" alt="food image" data-tilt>
        </div>
        <div class="text animate__animated animate__zoomIn animate__delay-1s">
            <h1>Stay fit</h1>
            <h1>Eat healthy</h1>
            <button class="btn">Order Now!</button>
        </div>
   
    <div class="first animate__animated animate__slideInDown"></div>
    <div class="second animate__animated animate__zoomIn"></div>
    <div class="third animate__animated animate__slideInUp"></div>
</div>



* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: sans-serif;
}

body {
    width: 100%;
    height: 100%;
}

.main{
    display: flex;
}
nav {
    width: 100%;
    height: 70px;
    display: flex;
    position: absolute;
    top: 0;
    left: 0;
    justify-content: space-evenly;
    align-items: center;
}

nav .logo {
    font-size: 40px;
    font-weight: 500;
    color: #ccc;
}

nav .logo::first-letter {
    font-size: 50px;
    color: rgba(226, 242, 6, 0.856);
}

ul {
    list-style: none;
}

ul li a {
    text-decoration: none;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 20px;
    margin-right: 150px;
}

.social-links {
    display: flex;
    align-items: center;
    gap: 6px;
}

.social-links li a {
    font-size: 18px;
    background-color: black;
    padding: 10px 13px;
    border-radius: 50%;
    color: rgba(193, 193, 8, 0.849);
    transition: all 0.5s ease-in-out;
}

.social-links li a:hover {
    background-color: rgba(0, 0, 0, 0.5);
    color: rgb(173, 207, 23);
}

.nav-links li a {
    color: aliceblue;
}

.hero {
    position: absolute;
    right: 100px;
    top: 0px;
}

.text {
    position: absolute;
    top: 20%;
    left: 10%;
    color: white;
    font-size: 50px;
}

.text h1::first-letter {
    color: rgba(255, 255, 0, 0.87);
}

.btn {
    padding: 10px 20px;
    color: black;
    background-color: rgba(255, 255, 0, 0.737);
    border: none;
    transition: all 0.5s ease-in-out;
    border-radius: 5px;
}

.btn:hover {
    color: yellow;
    background-color: rgba(0, 0, 0, 0.5);
}

.first {
    z-index: -1;
    width: 30%;
    height: 100vh;
    background-color: rgba(38, 38, 36, 0.906);
}

.second {
    z-index: -1;
    width: 40%;
    height: 100vh;
    background-color: black;
}

.third {
    z-index: -1;
    width: 30%;
    height: 100vh;
    background-color: rgba(222, 237, 0, 0.756);
}
@media (max-width:1000px){
    .text{
        margin-left: 100px;
    }
}

/* Responsive Styling for Tablets */
@media (max-width: 768px) {
    .main {
        flex-direction: column;
        align-items: center;
    }

    .hero {
        margin-top: 120px;
        
    }

    .hero img {
        width: 300px;
        height: 280px;
        margin: auto;
        filter: drop-shadow(2px 2px 5px rgba(0,0,0,0.5));
    }

    .text {
        text-align: center;
        justify-content: center;
        margin: 300px 0px 0px 100px;
    }
    .text h1{
        font-size: 35px;
        letter-spacing: 2px;
    }
  
    nav {
        flex-direction: column;
        align-items: center;
        gap: 20px;
    }

    .nav-links {
        margin: 0px auto;
    }

    .first, .second, .third {
        width: 100%;
        height: 30vh;
    }
    .second{
        order: 3;
    }
    .third{
        order: 2;
        height: 40vh;
    }
}

/* Mobile Styling */
@media (max-width: 480px) {
    .hero img {
        width: 200px;
        height: 200px;
    }

    .text {
        font-size: 24px;
    }

    nav .nav-links {
        gap: 5px;
        margin: 0 auto;
    }

    .first, .second, .third {
        height: 30vh;
    }
    .third{
        height: 40vh;
    }
}
ye home section mai ny responsive kr dia ha 768px or large screen ki b styling kr li ha lekin ye responsive ni ho rahi all device ky liye 768px pixels ky bd img agy peechy arahi ye set kr dey 