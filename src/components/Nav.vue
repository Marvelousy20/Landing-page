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

      <div class="container-fluid cont-container">
        <div class="main">
          <div class="logo-cont">
            <span>
              <i
                style="width: 50px"
                class="fa fa-bars fa-2x"
                v-b-toggle.sidebar-footer
              ></i>
            </span>
            <img
              src="../assets/logo.svg"
              alt=""
            />
          </div>

          <!-- Tablet and mobile Sidebar -->
          <b-sidebar id="sidebar-footer" no-header backdrop class="sidebar">
            <template #footer>
              <!-- <div>
                <nav>
                    
                </nav>
              </div> -->
            </template>
            <div class="px-3 py-3">
                <img src="../assets/logo.svg" alt="" class="mb-5">
              <div>
                <div class="form-group has-search mobile">
                  <span class="fa fa-search form-control-feedback"></span>
                  <input
                    type="text"
                    class="form-control"
                    placeholder="Search"
                  />
                </div>
                <ul class="a">
                  <li><a href="#"> <span>Wears</span><i class="fa fa-chevron-right" aria-hidden="true"></i></a></li>
                  <hr>
                  <li><a href="#"> <span>Accessories</span> <i class="fa fa-chevron-right" aria-hidden="true"></i></a></li>
                  <hr>
                  <li><a href="#"><span>Brands</span> <i class="fa fa-chevron-right" aria-hidden="true"></i></a></li>
                  <hr>
                  <li><a href="#"><span>Fabrics</span> <i class="fa fa-chevron-right" aria-hidden="true"></i></a></li>
                  <hr>
                  <div class="li">
                    <a href="#login"><span>Log In </span> <i class="fa fa-chevron-right" aria-hidden="true"></i></a>
                  </div>
                  <hr>
                   <div class="li">
                      <a href="#/singup"><span>Sign Up</span> <i class="fa fa-chevron-right" aria-hidden="true"></i></a>
                    </div>
                </ul>
                
              </div>
            </div>
          </b-sidebar>
          <!-- Mobile sidebar ends -->

          <div class="ul-div">
            <ul class="desktop-ul">
              <li><a href="#">Wears</a></li>
              <li><a href="#">Accessories</a></li>
              <li><a href="#">Brands</a></li>
              <li><a href="#">Fabrics</a></li>
            </ul>
          </div>

          <div class="form desktop-form">
            <div class="form-group has-search">
              <span class="fa fa-search form-control-feedback"></span>
              <input type="text" class="form-control" placeholder="Search" />
            </div>
          </div>

          <div class="desktop-form">
            <a href="#login">Log In</a> /
            <a href="#/singup">Sign Up</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="css" scoped>

.ul-div, .li li, .desktop-form >* {
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}

.ul-div a, .desktop-form > a {
    font-size: 1.15em;
    font-weight: 600; 
}

.ul-div a:hover {
    color: black;
    border-bottom: 2px solid black;
}

.fa:focus {
  outline: none;
}

.form-control {
    border: 1px solid #555;
    border-radius: none !important;
}

input.form-control:focus{
    box-shadow: none;
    outline: none;
    border: 1px solid #555;
}

.main {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

ul {
  list-style-type: none;
  display: flex;
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
  color: #555;
}

a {
  color: black;
}

.ul-div ul {
  list-style-type: none;
  display: flex;
  align-items: center;
  margin: 0;
  justify-content: space-between;
  padding: 0;
}

.ul-div {
  align-self: center;
  width: 40%;
}

.upper nav {
  background: #ebebeb;
  padding: 0 10px;
}

.upper ul {
  display: flex;
  justify-content: flex-end;
  list-style-type: none;
  /* padding: 1px 0; */
}

.upper ul li + li:before {
  content: "|";
  padding: 0 0.5em;
  opacity: 0.5;
}

@media screen and (min-width: 990px) {
  .logo-cont span, .sidebar {
    display: none;
  }

  .has-search .form-control {
    float: right;
  }

  ul {
    margin: 0 0 5px;
  }

    a:active {
        color: red;
        border-bottom: 1px solid red;
    }
}

/* Tablet */
@media screen and (max-width: 990px) and (min-width: 640px) {
  .logo-cont {
    display: flex;
    align-items: center;
  }
  .upper,
  .ul-div,
  .mobile input,
  .form .info,
  .mobile .has-search,
  .mobile .form-control-feedback {
    display: none;
  }

  input {
    width: 300px;
  }

  .cont-container {
    padding: 15px;
  }

  .section-two,
  .section-one .has-search {
    display: none;
  }

  .has-search .form-control {
    float: right;
  }

  ul {
    display: block;
    list-style: none;
    padding: 0;
  }

  ul >* {
    margin: 20px 0;
  }

    li a, .li a  {
    display: flex;
    justify-content: space-between !important;
    align-items: center !important;
    }

.a a {
    font-size: 1.4em;
    font-weight: 600;  
}
}

/* mobile */

@media screen and (max-width: 639px) {
  .cont-container {
    padding: 15px;
  }

  .upper,
  .desktop-form,
  .ul-div {
    display: none;
  }

  ul {
    display: block;
    list-style: none;
    padding: 0;
    
  }

  ul > *{
    margin: 20px 0;
  }

  .a a {
    font-size: 1.4em;
    font-weight: 600;  
  }

  li a, .li a {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .a {
    margin-top: 40px;
  }
  /* .a a,
  .info a {
    color: black;
    font-weight: 600;
    font-size: 1.3em;
  } */

  /* .a,
  a:focus {
    color: red;
    border-bottom: red;
  }

  .info > * {
    margin: 10px 0;
  }

  .info a {
    color: red;
  } */

  /* .in {
    justify-content: space-between;
    padding: 0 60px;
    text-align: center;
  }

  .in a {
    color: black;
  } */

  div.logo-cont {
    align-items: center;
    display: flex;
  }

}

a:hover {
  text-decoration: none;
}

</style>
