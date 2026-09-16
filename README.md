<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="description"
content="Farman Ullah - Amazon affiliate product recommendations for shoppers in the USA.">

<title>Farman Ullah | Smart Amazon Picks USA</title>

<style>

/* ==============================
   RESET
================================ */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #f6f7f9;
    color: #172033;
    line-height: 1.6;
}

a {
    text-decoration: none;
    color: inherit;
}

button,
input {
    font: inherit;
}

.container {
    width: min(1180px, 92%);
    margin: auto;
}


/* ==============================
   TOP BAR
================================ */

.topbar {
    background: #131a25;
    color: white;
    text-align: center;
    padding: 9px 15px;
    font-size: 13px;
}

.topbar b {
    color: #ffb000;
}


/* ==============================
   NAVBAR
================================ */

.navbar {
    position: sticky;
    top: 0;
    z-index: 1000;

    background: white;

    border-bottom: 1px solid #e5e7eb;

    box-shadow:
        0 4px 18px rgba(0,0,0,.06);
}

.nav-inner {
    min-height: 76px;

    display: flex;
    align-items: center;

    gap: 24px;
}


/* LOGO */

.brand {
    font-weight: 900;
    font-size: 22px;

    white-space: nowrap;
}

.brand span {
    color: #ff9900;
}

.brand small {
    display: block;

    color: #788395;

    font-size: 9px;

    letter-spacing: 1.5px;
}


/* NAV LINKS */

.nav-links {
    display: flex;

    align-items: center;
    justify-content: center;

    gap: 25px;

    list-style: none;

    flex: 1;
}

.nav-links a {
    font-size: 14px;

    font-weight: 700;

    color: #364152;

    padding: 10px 0;

    position: relative;
}

.nav-links a::after {
    content: "";

    position: absolute;

    left: 0;
    bottom: 4px;

    width: 0;
    height: 2px;

    background: #ff9900;

    transition: .25s;
}

.nav-links a:hover {
    color: #e88900;
}

.nav-links a:hover::after {
    width: 100%;
}


/* NAV BUTTON */

.nav-cta {
    background: #ff9900;

    color: #171717;

    padding: 11px 17px;

    border-radius: 8px;

    font-weight: 800;

    font-size: 13px;

    white-space: nowrap;
}

.nav-cta:hover {
    background: #e88900;
}


/* MOBILE MENU */

.menu {
    display: none;

    background: white;

    border: 1px solid #d8dde5;

    border-radius: 8px;

    padding: 8px 11px;

    cursor: pointer;

    font-size: 20px;
}


/* ==============================
   HERO
================================ */

.hero {
    padding: 85px 0;

    background:
        radial-gradient(
            circle at 82% 20%,
            rgba(255,153,0,.15),
            transparent 28%
        ),

        linear-gradient(
            135deg,
            #fff,
            #eef2f6
        );
}

.hero-grid {
    display: grid;

    grid-template-columns:
        1.05fr
        .95fr;

    align-items: center;

    gap: 70px;
}


/* HERO TEXT */

.badge {
    display: inline-block;

    background: #fff4df;

    color: #a85c00;

    border: 1px solid #ffd48b;

    padding: 7px 13px;

    border-radius: 30px;

    font-size: 12px;

    font-weight: 800;

    margin-bottom: 20px;
}

.hero h1 {
    font-size:
        clamp(
            48px,
            7vw,
            82px
        );

    line-height: .96;

    letter-spacing: -4px;

    margin-bottom: 24px;
}

.hero h1 span {
    color: #ff9900;
}

.hero p {
    max-width: 650px;

    color: #5d6878;

    font-size: 18px;

    margin-bottom: 28px;
}


/* BUTTONS */

.actions {
    display: flex;

    gap: 12px;

    flex-wrap: wrap;
}

.btn {
    display: inline-flex;

    align-items: center;
    justify-content: center;

    padding: 13px 20px;

    border-radius: 9px;

    font-weight: 800;

    font-size: 14px;

    transition: .25s;
}

.btn:hover {
    transform: translateY(-3px);

    box-shadow:
        0 12px 25px rgba(0,0,0,.12);
}

.orange {
    background: #ff9900;

    color: #111;
}

.dark {
    background: #172033;

    color: white;
}


/* ==============================
   PHOTO
================================ */

.photo-wrap {
    max-width: 440px;

    margin: auto;

    position: relative;
}

.photo-wrap::before {
    content: "";

    position: absolute;

    inset: -14px;

    border: 2px solid #ff9900;

    border-radius: 27px;

    transform: rotate(4deg);

    opacity: .45;
}

.photo-card {
    position: relative;

    background: white;

    padding: 10px;

    border-radius: 22px;

    box-shadow:
        0 28px 65px rgba(0,0,0,.18);
}

.photo-card img {
    width: 100%;

    height: 500px;

    object-fit: cover;

    border-radius: 15px;
}

.photo-caption {
    position: absolute;

    left: 22px;
    right: 22px;
    bottom: 22px;

    background:
        rgba(17,24,39,.92);

    color: white;

    border-radius: 12px;

    padding: 13px 15px;
}

.photo-caption strong {
    display: block;
}

.photo-caption small {
    color: #d0d6df;
}


/* ==============================
   SEARCH
================================ */

.search-area {
    background: white;

    border-bottom:
        1px solid #e5e7eb;

    padding: 25px 0;
}

.search {
    max-width: 720px;

    margin: auto;

    display: flex;

    border:
        1px solid #cfd5dd;

    border-radius: 10px;

    overflow: hidden;

    background: #f8fafc;
}

.search input {
    flex: 1;

    border: 0;

    outline: 0;

    background: transparent;

    padding: 14px 16px;
}

.search button {
    border: 0;

    background: #ff9900;

    padding: 0 22px;

    font-weight: 800;

    cursor: pointer;
}


/* ==============================
   SECTIONS
================================ */

section {
    padding: 85px 0;
}

.heading {
    text-align: center;

    margin-bottom: 38px;
}

.heading small {
    color: #df8500;

    font-size: 11px;

    font-weight: 900;

    letter-spacing: 2px;

    text-transform: uppercase;
}

.heading h2 {
    font-size:
        clamp(
            32px,
            5vw,
            50px
        );

    letter-spacing: -2px;

    margin-top: 6px;
}

.heading p {
    max-width: 650px;

    margin: 10px auto 0;

    color: #6b7280;
}


/* ==============================
   CATEGORIES
================================ */

.categories {
    display: grid;

    grid-template-columns:
        repeat(4,1fr);

    gap: 16px;
}

.category {
    background: white;

    border:
        1px solid #e3e7ec;

    border-radius: 16px;

    padding: 26px;

    text-align: center;

    transition: .25s;

    cursor: pointer;
}

.category:hover {
    transform: translateY(-6px);

    border-color: #ff9900;

    box-shadow:
        0 15px 30px rgba(0,0,0,.08);
}

.category .icon {
    font-size: 34px;

    margin-bottom: 8px;
}

.category p {
    font-size: 13px;

    color: #727c8c;
}


/* ==============================
   PRODUCTS
================================ */

.products-section {
    background: #eef1f4;
}

.products {
    display: grid;

    grid-template-columns:
        repeat(4,1fr);

    gap: 20px;
}

.product {
    background: white;

    border:
        1px solid #e1e5ea;

    border-radius: 16px;

    overflow: hidden;

    transition: .3s;
}

.product:hover {
    transform: translateY(-7px);

    box-shadow:
        0 18px 40px rgba(0,0,0,.1);
}

.product-image {
    height: 190px;

    background: #f7f8fa;

    display: flex;

    align-items: center;
    justify-content: center;

    font-size: 72px;
}

.product-info {
    padding: 19px;
}

.product-cat {
    color: #e28a00;

    font-size: 10px;

    font-weight: 900;

    letter-spacing: 1px;

    text-transform: uppercase;
}

.product h3 {
    font-size: 17px;

    margin: 6px 0;
}

.stars {
    color: #f59e0b;

    font-size: 13px;
}

.product p {
    color: #6b7280;

    font-size: 13px;

    min-height: 43px;

    margin-top: 5px;
}

.amazon-btn {
    display: block;

    text-align: center;

    background: #ff9900;

    color: #111;

    padding: 10px;

    border-radius: 7px;

    font-size: 13px;

    font-weight: 900;

    margin-top: 14px;
}

.amazon-btn:hover {
    background: #e88b00;
}


/* ==============================
   WHY
================================ */

.dark-section {
    background: #131a25;

    color: white;
}

.dark-section .heading p {
    color: #aab4c3;
}

.why-grid {
    display: grid;

    grid-template-columns:
        repeat(3,1fr);

    gap: 20px;
}

.why-card {
    background:
        rgba(255,255,255,.06);

    border:
        1px solid rgba(255,255,255,.1);

    border-radius: 18px;

    padding: 30px;
}

.why-card .icon {
    font-size: 30px;

    margin-bottom: 13px;
}

.why-card p {
    color: #aab4c3;

    font-size: 14px;

    margin-top: 7px;
}


/* ==============================
   ABOUT
================================ */

.about {
    display: grid;

    grid-template-columns:
        .8fr 1.2fr;

    gap: 60px;

    align-items: center;
}

.about-img {
    background: white;

    padding: 10px;

    border-radius: 20px;

    box-shadow:
        0 20px 50px rgba(0,0,0,.1);
}

.about-img img {
    height: 400px;

    width: 100%;

    object-fit: cover;

    border-radius: 14px;
}

.about-text h2 {
    font-size:
        clamp(
            34px,
            5vw,
            52px
        );

    line-height: 1.03;

    letter-spacing: -2px;

    margin-bottom: 20px;
}

.about-text p {
    color: #697485;

    margin-bottom: 15px;
}


/* STATS */

.stats {
    display: grid;

    grid-template-columns:
        repeat(3,1fr);

    gap: 12px;

    margin-top: 24px;
}

.stat {
    background: #f0f2f5;

    border-radius: 12px;

    padding: 17px;
}

.stat strong {
    display: block;

    color: #e28a00;

    font-size: 23px;
}

.stat span {
    color: #6b7280;

    font-size: 11px;
}


/* ==============================
   DISCLOSURE
================================ */

.disclosure {
    background: #fff7e6;

    border-top:
        1px solid #ffd58a;

    border-bottom:
        1px solid #ffd58a;

    padding: 22px 0;
}

.disclosure p {
    text-align: center;

    color: #6d511e;

    font-size: 12px;
}


/* ==============================
   CONTACT
================================ */

.contact {
    background: white;
}

.contact-box {
    max-width: 850px;

    margin: auto;

    text-align: center;

    padding: 60px 25px;

    border-radius: 25px;

    background:
        linear-gradient(
            135deg,
            #fff8e9,
            #fff
        );

    border:
        1px solid #efd49a;
}

.contact-box h2 {
    font-size:
        clamp(
            32px,
            5vw,
            50px
        );

    letter-spacing: -2px;
}

.contact-box p {
    max-width: 600px;

    color: #6b7280;

    margin: 12px auto 25px;
}


/* ==============================
   FOOTER
================================ */

footer {
    background: #131a25;

    color: white;

    padding: 38px 0;
}

.footer-grid {
    display: grid;

    grid-template-columns:
        1.3fr 1fr 1fr;

    gap: 40px;
}

footer h3 {
    margin-bottom: 10px;
}

footer p,
footer a {
    color: #9ca7b6;

    font-size: 13px;
}

footer a:hover {
    color: #ff9900;
}

.footer-list {
    list-style: none;
}

.footer-list li {
    margin-bottom: 6px;
}

.copyright {
    text-align: center;

    border-top:
        1px solid rgba(255,255,255,.1);

    margin-top: 28px;

    padding-top: 20px;

    color: #6f7988;

    font-size: 11px;
}


/* ==============================
   ANIMATION
================================ */

.reveal {
    opacity: 0;

    transform:
        translateY(25px);

    transition: .7s;
}

.reveal.show {
    opacity: 1;

    transform:
        translateY(0);
}


/* ==============================
   TABLET
================================ */

@media(max-width:1000px) {

    .hero-grid,
    .about {
        grid-template-columns: 1fr;
    }

    .photo-wrap {
        order: -1;
    }

    .categories,
    .products {
        grid-template-columns:
            repeat(2,1fr);
    }

    .footer-grid {
        grid-template-columns:
            1fr 1fr;
    }
}


/* ==============================
   MOBILE
================================ */

@media(max-width:700px) {

    .container {
        width: 92%;
    }

    .nav-inner {
        min-height: 68px;
    }

    .menu {
        display: block;

        margin-left: auto;
    }

    .nav-links {

        display: none;

        position: absolute;

        top: 68px;

        left: 4%;

        width: 92%;

        background: white;

        border:
            1px solid #e1e5ea;

        border-radius: 12px;

        box-shadow:
            0 15px 30px rgba(0,0,0,.12);

        flex-direction: column;

        align-items: stretch;

        gap: 0;

        padding: 8px;
    }

    .nav-links.active {
        display: flex;
    }

    .nav-links a {
        display: block;

        padding: 12px;
    }

    .nav-cta {
        display: none;
    }

    .hero {
        padding: 60px 0;
    }

    .hero p {
        font-size: 16px;
    }

    .hero h1 {
        letter-spacing: -3px;
    }

    .photo-card img {
        height: 400px;
    }

    .categories,
    .products,
    .why-grid,
    .footer-grid {
        grid-template-columns: 1fr;
    }

    .stats {
        grid-template-columns: 1fr;
    }

    section {
        padding: 70px 0;
    }

}


/* ==============================
   SMALL PHONE
================================ */

@media(max-width:400px) {

    .hero h1 {
        font-size: 50px;
    }

    .photo-card img {
        height: 340px;
    }

    .actions .btn {
        width: 100%;
    }

}

</style>
</head>


<body>


<!-- ==============================
     TOP BAR
================================ -->

<div class="topbar">

    🇺🇸
    <b>USA-focused</b>
    product recommendations · Amazon affiliate website

</div>



<!-- ==============================
     NAVIGATION
================================ -->

<nav class="navbar">

<div class="container nav-inner">


<a href="#home" class="brand">

    Farman<span>.</span>

    <small>
        AMAZON AFFILIATE
    </small>

</a>


<button
    class="menu"
    id="menuBtn"
    aria-label="Open navigation">

    ☰

</button>


<ul class="nav-links" id="navLinks">

    <li>
        <a href="#home">
            Home
        </a>
    </li>

    <li>
        <a href="#categories">
            Categories
        </a>
    </li>

    <li>
        <a href="#products">
            Products
        </a>
    </li>

    <li>
        <a href="#why">
            Why Us
        </a>
    </li>

    <li>
        <a href="#about">
            About
        </a>
    </li>

    <li>
        <a href="#contact">
            Contact
        </a>
    </li>

</ul>


<a
    href="#products"
    class="nav-cta">

    🛒 Shop Picks

</a>


</div>

</nav>



<!-- ==============================
     HERO
================================ -->

<section class="hero" id="home">

<div class="container hero-grid">


<div>

    <div class="badge">

        🇺🇸 AMAZON USA
        ·
        AFFILIATE MARKETING

    </div>


    <h1>

        Discover.
        <br>

        Compare.
        <br>

        <span>
            Shop Smart.
        </span>

    </h1>


    <p>

        Hi, I'm Farman Ullah.

        I research useful products and create
        simple product recommendations for
        shoppers in the United States.

    </p>


    <div class="actions">

        <a
            href="#products"
            class="btn orange">

            Explore Products →

        </a>


        <a
            href="#about"
            class="btn dark">

            Learn About Me

        </a>

    </div>

</div>



<!-- YOUR PHOTO -->

<div class="photo-wrap">

    <div class="photo-card">

        <img
            src="1000060169.png"
            alt="Farman Ullah">

        <div class="photo-caption">

            <strong>
                Farman Ullah
            </strong>

            <small>
                Amazon Affiliate Marketer · USA Market
            </small>

        </div>

    </div>

</div>


</div>

</section>



<!-- ==============================
     SEARCH
================================ -->

<div class="search-area">

<div class="container">

<div class="search">

<input
    id="searchInput"
    type="search"
    placeholder="Search kitchen, electronics, home, travel...">

<button id="searchBtn">

    🔍 Search

</button>

</div>

</div>

</div>



<!-- ==============================
     CATEGORIES
================================ -->

<section id="categories">

<div class="container">


<div class="heading">

    <small>
        Browse
    </small>

    <h2>
        Popular Categories
    </h2>

    <p>
        Explore focused product categories
        for everyday shopping.
    </p>

</div>



<div class="categories">


<div
    class="category reveal"
    data-category="kitchen">

    <div class="icon">
        🍳
    </div>

    <h3>
        Kitchen
    </h3>

    <p>
        Useful kitchen essentials
    </p>

</div>



<div
    class="category reveal"
    data-category="home">

    <div class="icon">
        🏠
    </div>

    <h3>
        Home
    </h3>

    <p>
        Home products & organization
    </p>

</div>



<div
    class="category reveal"
    data-category="electronics">

    <div class="icon">
        💻
    </div>

    <h3>
        Electronics
    </h3>

    <p>
        Tech and useful gadgets
    </p>

</div>



<div
    class="category reveal"
    data-category="travel">

    <div class="icon">
        🎒
    </div>

    <h3>
        Travel
    </h3>

    <p>
        Travel essentials
    </p>

</div>


</div>

</div>

</section>



<!-- ==============================
     PRODUCTS
================================ -->

<section
    id="products"
    class="products-section">

<div class="container">


<div class="heading">

    <small>
        Featured Picks
    </small>

    <h2>
        Recommended Products
    </h2>

    <p>
        Product examples for your
        Amazon USA affiliate website.
    </p>

</div>



<div
    class="products"
    id="productGrid">



<!-- PRODUCT 1 -->

<div
    class="product reveal"
    data-name="kitchen organizer kitchen">

    <div class="product-image">
        🍳
    </div>

    <div class="product-info">

        <span class="product-cat">
            Kitchen
        </span>

        <h3>
            Kitchen Organization Pick
        </h3>

        <div class="stars">
            ★★★★★
        </div>

        <p>
            A useful kitchen product
            for everyday organization.
        </p>


        <!-- REPLACE # WITH AMAZON LINK -->

        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 2 -->

<div
    class="product reveal"
    data-name="wireless headphones electronics audio">

    <div class="product-image">
        🎧
    </div>

    <div class="product-info">

        <span class="product-cat">
            Electronics
        </span>

        <h3>
            Wireless Audio Pick
        </h3>

        <div class="stars">
            ★★★★★
        </div>

        <p>
            A practical audio product
            for work and entertainment.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 3 -->

<div
    class="product reveal"
    data-name="home organizer home">

    <div class="product-image">
        🏠
    </div>

    <div class="product-info">

        <span class="product-cat">
            Home
        </span>

        <h3>
            Home Organization Pick
        </h3>

        <div class="stars">
            ★★★★☆
        </div>

        <p>
            A simple home product
            designed for organization.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 4 -->

<div
    class="product reveal"
    data-name="desk office electronics">

    <div class="product-image">
        💻
    </div>

    <div class="product-info">

        <span class="product-cat">
            Office
        </span>

        <h3>
            Desk Setup Pick
        </h3>

        <div class="stars">
            ★★★★★
        </div>

        <p>
            Useful accessories for
            a cleaner workspace.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 5 -->

<div
    class="product reveal"
    data-name="travel backpack travel">

    <div class="product-image">
        🎒
    </div>

    <div class="product-info">

        <span class="product-cat">
            Travel
        </span>

        <h3>
            Travel Essential
        </h3>

        <div class="stars">
            ★★★★☆
        </div>

        <p>
            A practical travel product
            for everyday trips.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 6 -->

<div
    class="product reveal"
    data-name="smart home home electronics">

    <div class="product-image">
        🏡
    </div>

    <div class="product-info">

        <span class="product-cat">
            Smart Home
        </span>

        <h3>
            Smart Home Pick
        </h3>

        <div class="stars">
            ★★★★★
        </div>

        <p>
            Explore convenient
            smart-home accessories.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 7 -->

<div
    class="product reveal"
    data-name="fitness exercise lifestyle">

    <div class="product-image">
        🏃
    </div>

    <div class="product-info">

        <span class="product-cat">
            Fitness
        </span>

        <h3>
            Fitness Essential
        </h3>

        <div class="stars">
            ★★★★☆
        </div>

        <p>
            Everyday fitness accessories
            worth exploring.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>



<!-- PRODUCT 8 -->

<div
    class="product reveal"
    data-name="phone accessories electronics">

    <div class="product-image">
        📱
    </div>

    <div class="product-info">

        <span class="product-cat">
            Tech
        </span>

        <h3>
            Phone Accessory Pick
        </h3>

        <div class="stars">
            ★★★★★
        </div>

        <p>
            Useful accessories for
            smartphones and devices.
        </p>


        <a
            href="#"
            class="amazon-btn"
            target="_blank"
            rel="nofollow sponsored noopener">

            View on Amazon →

        </a>

    </div>

</div>


</div>

</div>

</section>



<!-- ==============================
     WHY US
================================ -->

<section
    id="why"
    class="dark-section">

<div class="container">


<div class="heading">

    <small>
        Our Approach
    </small>

    <h2>
        Simple. Useful. Focused.
    </h2>

    <p>
        Product discovery should help
        people make informed shopping decisions.
    </p>

</div>



<div class="why-grid">


<div class="why-card reveal">

    <div class="icon">
        🔎
    </div>

    <h3>
        Product Research
    </h3>

    <p>
        Research products and organize
        recommendations around specific
        shopping needs.
    </p>

</div>



<div class="why-card reveal">

    <div class="icon">
        🇺🇸
    </div>

    <h3>
        USA Focus
    </h3>

    <p>
        Content is designed for shoppers
        looking for products on Amazon's
        US marketplace.
    </p>

</div>



<div class="why-card reveal">

    <div class="icon">
        💡
    </div>

    <h3>
        Useful Content
    </h3>

    <p>
        The goal is to provide helpful
        product discovery instead of
        random affiliate links.
    </p>

</div>


</div>

</div>

</section>



<!-- ==============================
     ABOUT
================================ -->

<section id="about">

<div class="container about">


<div class="about-img reveal">

    <img
        src="1000060169.png"
        alt="Farman Ullah - Affiliate Marketer">

</div>



<div class="about-text reveal">


<div
    class="heading"
    style="text-align:left;margin-bottom:20px">

    <small>
        About Me
    </small>

    <h2>
        Building a useful
        affiliate brand.
    </h2>

</div>


<p>

    I'm Farman Ullah, an aspiring
    digital entrepreneur and
    affiliate marketer.

</p>


<p>

    My focus is Amazon affiliate
    marketing for the United States
    market. I want to create useful
    product content, recommendations
    and comparison pages that help
    visitors discover products.

</p>


<p>

    I also combine web development,
    content creation, research and
    AI-assisted workflows to build
    digital projects.

</p>



<div class="stats">


<div class="stat">

    <strong>
        USA
    </strong>

    <span>
        Target Market
    </span>

</div>


<div class="stat">

    <strong>
        Amazon
    </strong>

    <span>
        Affiliate Platform
    </span>

</div>


<div class="stat">

    <strong>
        24/7
    </strong>

    <span>
        Learning Mindset
    </span>

</div>


</div>

</div>

</div>

</section>



<!-- ==============================
     DISCLOSURE
================================ -->

<div class="disclosure">

<div class="container">

<p>

<b>Affiliate Disclosure:</b>

As an Amazon Associate, I may earn
from qualifying purchases made
through links on this website.
Product prices, availability and
information can change on Amazon.

</p>

</div>

</div>



<!-- ==============================
     CONTACT
================================ -->

<section
    id="contact"
    class="contact">

<div class="container">


<div class="contact-box reveal">


<div class="heading">

    <small>
        Contact
    </small>

    <h2>
        Let's Connect
    </h2>

</div>


<p>

    For affiliate marketing projects,
    product research, content
    collaborations or digital opportunities.

</p>


<a
    href="mailto:far205744@gmail.com"
    class="btn orange">

    ✉ far205744@gmail.com

</a>


</div>

</div>

</section>



<!-- ==============================
     FOOTER
================================ -->

<footer>

<div class="container">


<div class="footer-grid">


<div>

<h3>
    Farman<span style="color:#ff9900;">
        .
    </span>
</h3>

<p>
    Amazon affiliate product discovery
    for shoppers in the USA.
</p>

</div>



<div>

<h3>
    Navigation
</h3>

<ul class="footer-list">

<li>
    <a href="#home">
        Home
    </a>
</li>

<li>
    <a href="#categories">
        Categories
    </a>
</li>

<li>
    <a href="#products">
        Products
    </a>
</li>

<li>
    <a href="#about">
        About
    </a>
</li>

</ul>

</div>



<div>

<h3>
    Contact
</h3>

<ul class="footer-list">

<li>
    <a href="mailto:far205744@gmail.com">
        far205744@gmail.com
    </a>
</li>

<li>
    🇺🇸 USA Market
</li>

<li>
    Amazon Affiliate
</li>

</ul>

</div>


</div>



<div class="copyright">

    © 2026 Farman Ullah
    ·
    Independent affiliate website

</div>


</div>

</footer>



<script>

/* =========================================
   MOBILE NAVIGATION
========================================= */

const menuBtn =
    document.getElementById("menuBtn");

const navLinks =
    document.getElementById("navLinks");


menuBtn.addEventListener(
    "click",
    function() {

        navLinks.classList.toggle("active");

    }
);


/* Close menu after clicking a link */

document
    .querySelectorAll(".nav-links a")
    .forEach(function(link) {

        link.addEventListener(
            "click",
            function() {

                navLinks.classList.remove("active");

            }
        );

    });



/* =========================================
   SEARCH
========================================= */

const searchInput =
    document.getElementById("searchInput");

const products =
    document.querySelectorAll(".product");


function searchProducts() {

    const query =
        searchInput
        .value
        .toLowerCase()
        .trim();


    products.forEach(
        function(product) {

            const name =
                product
                .dataset
                .name
                .toLowerCase();


            if (
                query === "" ||
                name.includes(query)
            ) {

                product.style.display = "";

            }

            else {

                product.style.display = "none";

            }

        }
    );

}


document
    .getElementById("searchBtn")
    .addEventListener(
        "click",
        searchProducts
    );


searchInput.addEventListener(
    "keydown",
    function(event) {

        if (event.key === "Enter") {

            searchProducts();

        }

    }
);



/* =========================================
   CATEGORY FILTER
========================================= */

document
    .querySelectorAll(".category")
    .forEach(function(category) {

        category.addEventListener(
            "click",
            function() {

                const selected =
                    category
                    .dataset
                    .category;


                searchInput.value =
                    selected;


                products.forEach(
                    function(product) {

                        const name =
                            product
                            .dataset
                            .name;


                        if (
                            name.includes(selected)
                        ) {

                            product.style.display =
                                "";

                        }

                        else {

                            product.style.display =
                                "none";

                        }

                    }
                );


                document
                    .getElementById("products")
                    .scrollIntoView({
                        behavior: "smooth"
                    });

            }
        );

    });



/* =========================================
   SCROLL ANIMATION
========================================= */

const observer =
    new IntersectionObserver(
        function(entries) {

            entries.forEach(
                function(entry) {

                    if (
                        entry.isIntersecting
                    ) {

                        entry.target
                            .classList
                            .add("show");

                    }

                }
            );

        },
        {
            threshold: 0.12
        }
    );


document
    .querySelectorAll(".reveal")
    .forEach(function(element) {

        observer.observe(element);

    });

</script>

</body>
</html>
