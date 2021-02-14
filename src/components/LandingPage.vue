<template>
    <div class="container-element">
        <div style="background-color: #EEEEEE; text-align: center" class="promo p-3">
            Get 15% off wears on your first order, T%Cs apply. 
            <a href="#">ORDER NOW</a> 
        </div>

        <header class="mt-3 mb-3">
            <div class="countries">
                <b-dropdown id="dropdown-left" text="United Kingdom" class="button" variant="none">
                    <b-dropdown-item class = 'e' href="#">United Kingdom</b-dropdown-item>
                    <b-dropdown-item href="#">United States</b-dropdown-item>
                    <b-dropdown-item href="#">Nigeria</b-dropdown-item>
                </b-dropdown>
                <span class="lang">English</span>
            </div>
            <div class = 'logo'>
                <img src="../assets/logo.svg" alt="img">
            </div>
            <div>
                <div class="desktop">
                    <span class="register"><a href="#">Register</a></span>
                    <span><a href="#">Sign In</a></span>
                </div>
                <div class="mobile">
                    <i class="fas fa-sign-in-alt fa-lg mr-2" v-b-tooltip.hover title="sign-in" aria-hidden="true"></i>
                    <i class="fas fa-sign-out-alt fa-lg" v-b-tooltip.hover title="sign-out" aria-hidden="true"></i>
                </div>
            </div>
        </header>

        <div class="promo-code text-center bg-dark text-white p-1 mb-5" >Get 20% off when you use our promo code "Styleest"</div>
        
        <div class="container-fluid">
            <div class="img-container">
                <img src="../assets/pexels-godisable-jacob-794064.jpg" alt="img">
            </div>
            <div>
                <h1>WHY WAIT FOR BLACK FRIDAY?</h1>
                <p>Dont't be left out, Check out all the amazing offers we have for you this season of LOVE.</p>
                <a href="#" class="shop">Shop now</a>
            </div>
        </div>

        <div class="container-row p-4 mt-5 mb-3">
            <div>
                <h1>What's New ?</h1>
                <p class="sub-text">Stay home and shop online</p>
                <button class="btn btn-info">SHOP WHAT IS NEW</button>
                <!-- <a href="#">Shop what is new</a> -->
            </div>
            <div class="img-slide">
                <!-- <img src="../assets/brands/pexels-erik-mclean-4061385.jpg" alt="img"> -->
                <div class="mr-3">
                    <img src="../assets/brands/pexels-wesner-rodrigues-1892629.jpg" alt="img">
                    <p>ADIDAS</p>
                </div>
                <div class="mr-3">
                    <img src="../assets/brands/pexels-godisable-jacob-1374910.jpg" alt="img">
                    <p>GUCCI</p>
                </div>
                <div class="mr-3">
                    <img src="../assets/brands/pexels-ralph-rabago-3214701.jpg" alt="img">
                    <p>JORDAN</p>
                </div>
                <div>
                    <img src="../assets/brands/pexels-mateusz-dach-3660471.jpg" alt="img">
                    <p>DIOR</p>
                </div>
            </div>
        </div>

        <div class="section-three">
            <div>
                <a href="#">
                    <img src="../assets/pexels-kai-pilger-996329.jpg" alt="">
                </a>
                <p>Check out some of our fashionable T-shirts</p>
                <a href="#">Shop for them now</a>
            </div>
            <div>
                <a href="#">
                    <img src="../assets/pexels-christ-geremie-darly's-oyembo-5128756.jpg" alt="img">
                </a>
                <p>We have the perfect outfit just for your occassion</p>
                <a href="#">Shop for them now</a>
            </div>
        </div>

        <div class="py-4 mt-3 bg-dark">
            <h1 class="text-center text-white mb-4">Top deals just for you</h1>
            <div class="offer-container">
                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../assets/offers/ankara splitted.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">Ankara</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="text">Shop now</a>
                    </div>
                </div>

                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../assets/offers/brown shoe.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">Brown Show</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="text">Shop now</a>
                    </div>
                </div>

                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../assets/offers/ribbon skirt.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">Ribbon Skirt</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="text">Shop now</a>
                    </div>
                </div>

                
                <div class="card" style="width: 18rem;">
                    <img class="card-img-top" src="../assets/offers/Brown Tuxedo.jpg" alt="Card image cap">
                    <div class="card-body">
                        <h5 class="card-title">Brown Tuxedo</h5>
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                        <a href="#" class="text">Shop now</a>
                    </div>
                </div>

            </div>
        </div>

        <footer  style="background-color: #EEEEEE;" class="text-center p-3">
            Styleest.Fashion
        </footer>
    </div>
</template>

<style scoped>
    .container-element {
        font-family: GillSans,"Gill Sans MT",sans-serif;
    }

    .promo:not(.a) {
        font-style: italic;
    }

    .button:after {
        content: "|";
        padding: 0 0.5em;
        margin-top: 3px;
        opacity: 0.5;
    }

    .register:after {
        content: "|";
        padding: 0 0.5em;
        margin-top: 3px;
        opacity: 0.5;
    }

    header {
        display: flex;
        width: 100%;
        justify-content: space-around;
        /* margin-top: 70px !important; */
    }

    header>* {
        width: 33.3%;
        text-align: center;
    }

    .logo img {
        max-width: 100px;
    }

    .lang {
        cursor: pointer;
    }

    .mobile {
        display: none;
    }

    a {
        color: black;
    }

    .container-fluid {
        display: flex;
    }

    .container-fluid div img {
        width: 100%;
        height: auto;
        object-fit: cover;
        object-position: top;
    }

    .container-fluid>* {
        width: 50%;
        height: 100%;
    }

    .container-fluid div:not(.img-container) {
        max-width: 400px;
        margin: 0 auto;
        align-self: center;
    }

    h1 {
        font-weight: 500;
    }

    .shop {
        font-weight: 500;
        margin-bottom: 30px;
    }

    .shop{
        padding: 12px 25px ;
        background-color: none;
        border: 3px solid #666 ;
        color: #666;
        top: 20px;
        font-size: .8rem;
        letter-spacing: 2px;
        position: relative;
        overflow: hidden;
        transition: .5s;
        display: inline-block;
    }

    .shop:hover{
        color: #fff;
        text-decoration: none;
    }

    .shop::before{
        content: "";
        background-color: #666;
        position: absolute;
        left: 0px;
        top: 0px;
        width: 100%;
        height: 0%;
        z-index: -1;
        transition: .5s;
    }
    .shop:hover::before{
        height: 100%;
    }

    @media screen and (max-width: 755px) {
        .container-fluid {
            flex-direction: column;
        }

        .container-fluid>* {
            width: 100%;
            height: 100%;
        }

        .countries {
            display: none;
        }

        .desktop {
            display: none;
        }

        .mobile {
            display: block;
            height: 100%;
            align-self: center;
        }

        header {
            display: flex;
            justify-content: center;
            text-align: center;
            align-items: center;
        }

        .logo {
            margin-left: auto;
        }

        .container-row {
            flex-direction: column;
            padding: 20px !important;
            margin: 0 auto !important;
            align-self: center;
        }

        .container-row>* {
            width: 100% !important;
        }

        .img-slide {
            margin-top: 30px;
        }

        .img-slide img {
            width: 70%;
            display: flex;
            flex-direction: column !important;
            justify-content: space-between;
        }

        .container-fluid div:not(.img-container) {
            max-width: 100%;
            margin: 20px 0 auto;
            align-self: center;
        }

        .section-three {
            display: block !important;
            margin-top: 0 !important;
        }

        .section-three div {
            padding: 20px;
            width: 100% !important;
        }

        .offer-container {
            /* display: block !important; */
            flex-wrap: wrap;
        }

        .offer-container .card {
            width: 100% !important;
        }
    }

    .container-row {
        display: flex;
        width: 100%;
    }

    .container-row div:not(.img-slide){
        width: 30%;
        margin: auto;
    }

    .container-row div.img-slide {
        width: 70%;
        display: flex;
        justify-content: space-between;
    }

    .container-row a {
        border-bottom: 2px solid black;
        font-size: 1.2em;
    }

    .container-row a:hover {
        text-decoration: none;
        border-bottom: 2px solid #007bff;
    }

    .img-slide div {
        height: 100%;
        text-align: center;
    }

    .img-slide img {
        height: 100%;
        width: 100%;
        object-fit: cover;
    }

    .img-slide p {
        margin-top: 5px !important;
        font-weight: 600;
    }

    .container-row h1 {
        font-size: 3.7em;
    }

    .sub-text {
        font-size: 1.2em;
    }

    .section-three {
        display: flex;
        justify-content: space-around;
        margin-top: 50px;
        text-align: center;
    }

    .section-three p {
        font-size: 1.3em;
        margin: 10px 0 0;
    }

    .section-three a, .text {
        border-bottom: 2px solid black;
        font-size: 1.2em;
    }

    .section-three a:hover, .text:hover {
        text-decoration: none;
        border-bottom: 2px solid #007bff;
    }

    .section-three div {
        width: 46%;
    }

    .section-three img {
        width: 100%;
        height: auto;
        object-position: top;
        object-fit: cover;
    }

    .offer-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }
</style>