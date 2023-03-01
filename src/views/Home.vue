<script setup>
import Navbar from "../components/nav_bar.vue";
import Footer from "../components/footer.vue";
</script>

<template>
  <header class="acceuil">
    <Navbar />
    <div class="search">
      <div class="wrapper">
        <div class="search_box">
          <select name="Ville" id="Ville">
            <option value="volvo">Yaounde</option>
            <option value="saab">Douala</option>
          </select>
          <select name="Quartier" id="Quartier">
            <option value="volvo">Biyem Assi</option>
            <option value="saab">Simbok</option>
            <option value="mercedes">Etok koss</option>
            <option value="audi">TKC</option>
          </select>

          <button>
            <i class="fas fa-search"></i>
          </button>
        </div>
      </div>
    </div>
    <div class="titre">
      <h1>COIN MOBILIER</h1>
    </div>
    <div class="bouton">
      <a href="" class="btn">PARCOURIR</a>
      <a href="" class="btn">SUR MESURE</a>
    </div>
  </header>
  <Footer />
</template>

<style scoped>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "poppins", sans-serif;
}
body {
  width: 100vw;
  height: 100vh;
  overflow-x: hidden;
}
header {
  background-image: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)),
    url("../assets/images/bg_home.jpg");
  height: 100vh;
  width: 100vw;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}
/* ------------------------------------------------- */
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap");

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
}

.container {
  max-width: 94%;
  padding: 20px 2rem;
  margin: 0 auto;
  display: flex;
  position: relative;
  font-weight: 500;
}

.logo-container {
  flex: 1;
  display: flex;
  align-items: center;
}

.nav-btn {
  flex: 3;
  display: flex;
  font-size: 1.2rem;
  justify-content: space-between;
}

.nav-links {
  flex: 3;
}
#aa {
  flex: 2;
  max-width: 3rem;
}
.log-sign {
  display: flex;
  align-items: center;
  flex: 1;
  max-width: max-content;
}
.logo {
  color: #fff;
  font-size: 1.8vw;
  font-weight: 600;
  letter-spacing: 2px;
  text-transform: uppercase;
  line-height: 3rem;
}

.logo span {
  font-weight: 300;
}

.btn {
  display: inline-block;
  padding: 0.5rem 1.3rem;
  font-size: 1.2rem;
  border: 2px solid #fff;
  border-radius: 2rem;
  line-height: 1;
  margin: 0 0.2rem;
  transition: 0.3s;
  text-transform: uppercase;
}

.btn.solid,
.btn.transparent:hover {
  background-color: #fff;
  color: black;
}

.btn.transparent,
.btn.solid:hover {
  background-color: transparent;
  color: #fff;
}

.nav-links > ul {
  display: flex;
  justify-content: center;
  align-items: center;
}

.nav-link {
  position: relative;
}

.nav-link > a {
  line-height: 3rem;
  color: #fff;
  padding: 0 0.8rem;
  letter-spacing: 1px;
  font-size: 1.2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  transition: 0.5s;
}

.nav-link > a > i {
  margin-left: 0.2rem;
}

.nav-link:hover > a {
  transform: scale(1.1);
}

.dropdown {
  position: absolute;
  top: 100%;
  left: -5.2px;
  width: 10rem;
  transform: translateY(10px);
  opacity: 0;
  pointer-events: none;
  transition: 0.5s;
  z-index: 100;
}

.dropdown ul {
  position: relative;
}

.dropdown-link > a {
  display: flex;
  background-color: #fff;
  color: black;
  padding: 0.5rem 1rem;
  font-size: 0.9rem;
  align-items: center;
  justify-content: space-between;
  transition: 0.3s;
}

.dropdown-link:hover > a {
  background-color: black;
  color: #fff;
}

.dropdown-link:not(:nth-last-child(2)) {
  border-bottom: 1px solid #efefef;
}

.dropdown-link i {
  transform: rotate(-90deg);
}

.arrow {
  position: absolute;
  width: 11px;
  height: 11px;
  top: -5.5px;
  left: 32px;
  background-color: #fff;
  transform: rotate(45deg);
  cursor: pointer;
  transition: 0.3s;
  z-index: -1;
}

.dropdown-link:first-child:hover ~ .arrow {
  background-color: black;
}

.dropdown-link {
  position: relative;
}

.dropdown.second {
  top: 0;
  left: 100%;
  padding-left: 0.8rem;
  cursor: pointer;
  transform: translateX(10px);
}

.dropdown.second .arrow {
  top: 10px;
  left: -5.5px;
}

.nav-link:hover > .dropdown,
.dropdown-link:hover > .dropdown {
  transform: translate(0, 0);
  opacity: 1;
  pointer-events: auto;
}

.hamburger-menu-container {
  flex: 1;
  display: none;
  align-items: center;
  justify-content: flex-end;
}

.hamburger-menu {
  width: 2.5rem;
  height: 2.5rem;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.hamburger-menu div {
  width: 1.6rem;
  height: 3px;
  border-radius: 3px;
  background-color: #fff;
  position: relative;
  z-index: 1001;
  transition: 0.5s;
}

.hamburger-menu div:before,
.hamburger-menu div:after {
  content: "";
  position: absolute;
  width: inherit;
  height: inherit;
  background-color: #fff;
  border-radius: 3px;
  transition: 0.5s;
}

.hamburger-menu div:before {
  transform: translateY(-7px);
}

.hamburger-menu div:after {
  transform: translateY(7px);
}

#check {
  position: absolute;
  top: 50%;
  right: 1.5rem;
  transform: translateY(-50%);
  width: 2.5rem;
  height: 2.5rem;
  z-index: 90000;
  cursor: pointer;
  opacity: 0;
  display: none;
}

#check:checked ~ .hamburger-menu-container .hamburger-menu div {
  background-color: transparent;
}

#check:checked ~ .hamburger-menu-container .hamburger-menu div:before {
  transform: translateY(0) rotate(-45deg);
}

#check:checked ~ .hamburger-menu-container .hamburger-menu div:after {
  transform: translateY(0) rotate(45deg);
}

@keyframes animation {
  from {
    opacity: 0;
    transform: translateY(15px);
  }
  to {
    opacity: 1;
    transform: translateY(0px);
  }
}

@media (max-width: 920px) {
  .hamburger-menu-container {
    display: flex;
  }

  #check {
    display: block;
  }

  .nav-btn {
    position: fixed;
    height: calc(100vh - 3rem);
    top: 3rem;
    left: 0;
    width: 100%;
    background-color: black;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    overflow-x: hidden;
    overflow-y: auto;
    transform: translateX(100%);
    transition: 0.65s;
    z-index: 10000;
  }

  #check:checked ~ .nav-btn {
    transform: translateX(0);
  }

  #check:checked ~ .nav-btn .nav-link,
  #check:checked ~ .nav-btn .log-sign {
    animation: animation 0.5s ease forwards var(--i);
  }

  .nav-links {
    flex: initial;
    width: 100%;
  }

  .nav-links > ul {
    flex-direction: column;
  }

  .nav-link {
    width: 100%;
    opacity: 0;
    transform: translateY(15px);
  }

  .nav-link > a {
    line-height: 1;
    padding: 1.6rem 2rem;
  }

  .nav-link:hover > a {
    transform: scale(1);
    background-color: black;
  }

  .dropdown,
  .dropdown.second {
    position: initial;
    top: initial;
    left: initial;
    transform: initial;
    opacity: 1;
    pointer-events: auto;
    width: 100%;
    padding: 0;
    background-color: black;
    display: none;
  }

  .nav-link:hover > .dropdown,
  .dropdown-link:hover > .dropdown {
    display: block;
  }

  .nav-link:hover > a > i,
  .dropdown-link:hover > a > i {
    transform: rotate(360deg);
  }

  .dropdown-link > a {
    background-color: transparent;
    color: #fff;
    padding: 1.2rem 2rem;
    line-height: 1;
  }

  .dropdown.second .dropdown-link > a {
    padding: 1.2rem 2rem 1.2rem 3rem;
  }

  .dropdown.second .dropdown.second .dropdown-link > a {
    padding: 1.2rem 2rem 1.2rem 4rem;
  }

  .dropdown-link:not(:nth-last-child(2)) {
    border-bottom: none;
  }

  .arrow {
    z-index: 1;
    background-color: black;
    left: 10%;
    transform: scale(1.1) rotate(45deg);
    transition: 0.5s;
  }

  .nav-link:hover .arrow {
    background-color: black;
  }

  .dropdown .dropdown .arrow {
    display: none;
  }

  .dropdown-link:hover > a {
    background-color: black;
  }

  .dropdown-link:first-child:hover ~ .arrow {
    background-color: black;
  }

  .nav-link > a > i {
    font-size: 1.1rem;
    transform: rotate(-90deg);
    transition: 0.7s;
  }

  .dropdown i {
    font-size: 1rem;
    transition: 0.7s;
  }

  .log-sign {
    flex: initial;
    width: 100%;
    padding: 1.5rem 1.9rem;
    justify-content: flex-start;
    opacity: 0;
    transform: translateY(15px);
  }
}

#nav_el {
  list-style: none;
  float: right;
  display: flex;
  justify-content: space-between;
  text-align: center;
}

#nav_el:first-child li:not-child a {
  text-decoration: none;
  color: white;
  padding: 10px 20px;
  text-transform: uppercase;
  border: 1px solid transparent;
  margin: 10px;
  font-weight: 500;
  transition: 0.6s ease;
}

#nav_el:first-child li a:hover {
  background: white;
  color: black;
}

#nav_el li.active:first-child a {
  background: white;
  color: black;
}

.principale {
  max-width: 124rem;
  margin: 0 auto;
}

.titre {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.titre {
  color: white;
  font-size: 3.2vw;
}

.bouton {
  position: absolute;
  top: 64%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.bouton a {
  color: white;
  text-decoration: none;
  border: 1px solid white;
  padding: 10px 20px;
  font-size: 1.5vw;
}

.btn {
  transition: 00.6s ease;
}

.bouton .btn:hover {
  background-color: white;
  color: black;
  letter-spacing: 4px;
}
/* -------------------------------------------------- search bar ---------------------------------------------- */
.search {
  position: absolute;
  top: 28%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 19vh;
  background-color: #181818ad;
}
.wrapper {
  width: 100%;
  height: 100%;
  background-size: cover;
  display: flex;
  justify-content: space-between;
  justify-content: center;
  align-items: center;
  position: relative;
}

.search_box {
  width: 50%;
  max-width: 70%;
  position: relative;
}

.search_box button {
  width: 10%;
  box-sizing: border-box;
  background: rgba(0, 0, 0, 0.3);
  border: 1.5px solid #fff;
  border-radius: 90px;
  font-size: 1.2vw;
  color: white;
  outline: none;
}
option {
  background-color: rgba(49, 43, 43, 0.11);
}
.search_box select {
  width: 40%;
  margin: 10px;
  padding: 20px;
  box-sizing: border-box;
  background: rgba(0, 0, 0, 0.3);
  border: 1.5px solid #fff;
  border-radius: 10px;
  font-size: 1.2vw;
  color: #fff;
  outline: none;
}
.fa-search {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  right: 25px;
  color: #fff;
  font-size: 25px;
}

::-webkit-input-placeholder {
  /* Chrome/Opera/Safari */
  color: #fff;
}
::-moz-placeholder {
  /* Firefox 19+ */
  color: #fff;
}
:-ms-input-placeholder {
  /* IE 10+ */
  color: #fff;
}

@media screen and (max-width: 425px) {
  .search_box {
    width: 95%;
  }
}
/* -------------------------- footer ------------------------------------- */
.copyright-text {
  margin: 0;
  padding-bottom: 10px;
  padding-top: 7px;
  text-align: center;
  width: 100%;
  color: #bbbbbb;
  font-size: 15px;
  background-color: #24262b;
}
.copyright-text p {
  margin: 0;
  padding: 0;
}
.container_footer {
  max-width: 1170px;
  margin: auto;
}
.row {
  display: flex;
  flex-wrap: wrap;
}
.footer {
  background-color: white;
  padding: 70px 0;
}
.footer-col {
  width: 25%;
  padding: 0 15px;
}
.footer-col h4 {
  font-size: 18px;
  color: #24262b;
  text-transform: capitalize;
  margin-bottom: 35px;
  font-weight: 500;
  position: relative;
}
.footer-col h4::before {
  content: "";
  position: absolute;
  left: 0;
  bottom: -10px;
  background-color: #e91e63;
  height: 2px;
  box-sizing: border-box;
  width: 50px;
}
.footer-col ul li:not(:last-child) {
  margin-bottom: 10px;
}
.footer-col ul li a {
  font-size: 16px;
  text-transform: capitalize;
  color: #ffffff;
  text-decoration: none;
  font-weight: 300;
  color: #24262b;
  display: block;
  transition: all 0.3s ease;
}
.footer-col ul li a:hover {
  color: black;
  padding-left: 8px;
  font-weight: 600;
}
.footer-col .social-links a {
  display: inline-block;
  height: 40px;
  width: 40px;
  background-color: rgba(255, 255, 255, 0.2);
  margin: 0 10px 10px 0;
  text-align: center;
  line-height: 40px;
  border-radius: 50%;
  color: #24262b;
  transition: all 0.5s ease;
}
.footer-col .social-links a:hover {
  color: #ffffff;
  background-color: #24262b;
}

/*responsive*/
@media (max-width: 767px) {
  .footer-col {
    width: 50%;
    margin-bottom: 30px;
  }
}
@media (max-width: 574px) {
  .footer-col {
    width: 100%;
  }
}
</style>
