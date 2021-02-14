<template>
    <div>
        <div class="desktop">
            <div class="upper">
                <nav>
                    <ul>
                        <li><a href="#"> Become a vendor </a></li>
                        <li><a href="#"> Help </a></li>
                        <li><a href="#"> ENG </a></li>
                        <li><a href="#"> USD </a></li>
                    </ul>
                </nav>
            </div>

            <div class="container-fluid">
                <div class="row lower">
                    <div class="col-7">
                        <div>
                            <nav class="section-one">
                                <div class="logo-cont d-flex">
                                    <span>
                                        <i style="width: 50px" class="fa fa-bars fa-2x" v-b-toggle.sidebar-footer></i>
                                    </span>
                                    <img src="../assets/logo.svg" alt="">
                                </div>
                                <ul class="desktop-ul">
                                    <li><a href="#">Wears</a></li>
                                    <li><a href="#">Accessories</a></li>
                                    <li><a href="#">Brands</a></li>
                                    <li><a href="#">Fabrics</a></li>
                                </ul>
                            </nav>
                        </div>
                    </div>

                    <div class="col">
                        <div>
                            <nav class="section-two">
                                <div class="form">
                                    <div class="form-group has-search">
                                        <span class="fa fa-search form-control-feedback"></span>
                                        <input type="text" class="form-control" placeholder="Search">
                                    </div>            
                                </div>
                                
                                <div>
                                    <a href="#login">Log In</a> /
                                    <a href="#/singup">Sign Up</a>
                                </div>
                            </nav>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Mobile -->
        <div class="mobile">
            <div>
                <div class="d-flex p-2 head">
                    <span>
                        <i style="width: 50px" class="fa fa-bars fa-2x" v-b-toggle.sidebar-footer></i>
                    </span>
                    <div class="logo-cont">
                        <img src="../assets/logo.svg" alt="">
                    </div>
                </div>
                <b-sidebar id="sidebar-footer" no-header backdrop>
                    <template #footer>
                        <div class="upper">
                            <nav>
                                <ul class="d-flex m-0 in">
                                    <li><a href="#"> Become a vendor </a></li>
                                    <li><a href="#"> Help </a></li>
                                </ul>
                                <ul class="d-flex m-0 in">
                                    <li><a href="#"> ENG </a></li>
                                    <li><a href="#"> USD </a></li>
                                </ul>
                            </nav>
                        </div>
                    </template>
                    <div class="px-3 py-3">
                        <div>
                            <nav class="section-one">
                                <div class="form-group has-search">
                                    <span class="fa fa-search form-control-feedback"></span>
                                    <input type="text" class="form-control" placeholder="Search">
                                </div>
                                <ul class="mt-5 a">
                                    <li><a href="#">Wears</a></li>
                                    <li><a href="#">Accessories</a></li>
                                    <li><a href="#">Brands</a></li>
                                    <li><a href="#">Fabrics</a></li>
                                </ul>
                                <hr>
                            </nav>
                        </div>  
                        <div>
                            <nav class="section-two">
                                <div class="form">  
                                    <div class="info text-center">
                                        <div>
                                            <a href="#login">Log In</a>
                                        </div>
                                        <hr>
                                        <div>
                                            <a href="#/singup">Sign Up</a>
                                        </div>
                                    </div>          
                                </div>
                            </nav>
                        </div>                  
                    </div>
                </b-sidebar>
            </div>
        </div>    
    </div>
</template>

<style lang="css" scoped>
    .fa:focus {
        outline: none;
    }

    @media screen and (min-width: 1170px) {
        .upper nav {
            background: #EBEBEB;
            padding: 0 10px;
        }

        .upper ul {
            display: flex;
            justify-content: flex-end;
            list-style-type: none;
            /* padding: 1px 0; */
        }

        .upper ul li+li:before {
            content: "|"; 
            padding: 0 .5em;
            opacity: .5;
        }

        .lower a:focus {
            color: red;
            border-bottom: 1.5px solid red;
        }

        a {
            color: black;
        }

        a:hover {
            text-decoration: none;
        }


        .section-one {
            display: flex;
        }

        .has-search .form-control {
        padding-left: 2.375rem;
        margin: 0;
        align-self: center;
        float: right;
        }

        .has-search .form-control-feedback {
            position: absolute;
            z-index: 2;
            display: block;
            width: 2.375rem;
            height: 2.375rem;
            line-height: 2.375rem;
            text-align: center;
            pointer-events: none;
            color: #aaa;
        }

        .section-two {
            display: flex;
            justify-content: space-around;
        }

        .section-one ul {
            display: flex;
            list-style: none;
            flex-wrap: wrap;
        }

        .section-one ul {
            width: 80%;
            list-style: none;
            display: flex;
            margin: 0;
            justify-content: space-around;
        }

        nav.section-two, nav.section-one {
            align-items: center;
        }
        
        .mobile {
            display: none;
        }
    }


    /* @media screen and (max-width: 1170px) {
         .section-one ul {
            width: 60%;
            list-style: none;
            display: flex;
            margin: 0;
            justify-content: space-around;
        }
    } */
    /* Mobile */
    @media screen and (max-width: 650px) {
        .desktop {
            display: none;
        }

        .mobile {
            display: block;
        }

        ul {
            list-style: none;
            padding: 0;
            text-align: center;
        }

        ul>li {
           margin: 10px 0; 
        }

        .a a, .info a {
            color: black;
            font-weight: 600;
            font-size: 1.3em;
        }

        .a, a:focus {
            color: red;
            border-bottom: red;
        }

        
        .info a{
            color: red;
        }

        .head span {
            align-self: center;
        }

        .in {
            justify-content: space-between;
            padding: 0 60px;
            text-align: center;
        }

        .in a {
            color: black;
        }
    }

    /* Tablet */

    @media screen and (max-width: 1170px) and (min-width: 650px) {
       .upper {
           display: none;
       }
        .has-search .form-control {
            padding-left: 2.375rem;
            margin: 0;
            align-self: center;
        }

        .has-search .form-control-feedback {
            position: absolute;
            z-index: 2;
            display: block;
            width: 2.375rem;
            height: 2.375rem;
            line-height: 2.375rem;
            text-align: center;
            pointer-events: none;
            color: #aaa;
        }

        .head {
            display: none !important;
        }

        .lower {
            padding: 20px;
        }

        ul {
            list-style-type: none;
        }

        .desktop-ul {
            display: none;
        }

        .logo-cont span {
            align-self: center;
        }

        .section-two {
            display: flex;
            justify-content: space-between;
        }

        .mobile .section-two {
            display: none !important;
        }

        .mobile hr {
            display: none;
        }

        .mobile input, .mobile .form-control-feedback {
            display: none;
        }
    }
</style>