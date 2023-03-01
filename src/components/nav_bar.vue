<script setup></script>
<template>
  <div class="container">
    <input type="checkbox" name="" id="check" />

    <div class="logo-container">
      <h3 class="logo">My<span>Home</span></h3>
    </div>

    <div class="nav-btn">
      <div class="nav-links">
        <ul id="nav_el">
          <li class="nav-link" style="--i: 0.6s">
            <a href="#">Acceuil</a>
          </li>
          <li class="nav-link" style="--i: 0.85s">
            <a href="#">Services<i class="fas fa-caret-down"></i></a>
            <div class="dropdown">
              <ul>
                <li class="dropdown-link">
                  <a href="#">Link 1</a>
                </li>
                <li class="dropdown-link">
                  <a href="#">Link 2</a>
                </li>
                <li class="dropdown-link">
                  <a href="#">Link 3<i class="fas fa-caret-down"></i></a>
                  <div class="dropdown second">
                    <ul>
                      <li class="dropdown-link">
                        <a href="#">Link 1</a>
                      </li>
                      <li class="dropdown-link">
                        <a href="#">Link 2</a>
                      </li>
                      <li class="dropdown-link">
                        <a href="#">Link 3</a>
                      </li>
                      <li class="dropdown-link">
                        <a href="#">More<i class="fas fa-caret-down"></i></a>
                        <div class="dropdown second">
                          <ul>
                            <li class="dropdown-link">
                              <a href="#">Link 1</a>
                            </li>
                            <li class="dropdown-link">
                              <a href="#">Link 2</a>
                            </li>
                            <li class="dropdown-link">
                              <a href="#">Link 3</a>
                            </li>
                            <div class="arrow"></div>
                          </ul>
                        </div>
                      </li>
                      <div class="arrow"></div>
                    </ul>
                  </div>
                </li>
                <li class="dropdown-link">
                  <a href="#">Link 4</a>
                </li>
                <div class="arrow"></div>
              </ul>
            </div>
          </li>
          <li class="nav-link" style="--i: 1.1s">
            <a href="#">A propos<i class="fas fa-caret-down"></i></a>
            <div class="dropdown">
              <ul>
                <li class="dropdown-link">
                  <a href="#">Service 1</a>
                </li>
                <li class="dropdown-link">
                  <a href="#">Service 2</a>
                </li>
                <li class="dropdown-link">
                  <a href="#">Service 3<i class="fas fa-caret-down"></i></a>
                  <div class="dropdown second">
                    <ul>
                      <li class="dropdown-link">
                        <a href="#">Service 1</a>
                      </li>
                      <li class="dropdown-link">
                        <a href="#">Service 2</a>
                      </li>
                      <li class="dropdown-link">
                        <a href="#">Service 3</a>
                      </li>
                      <li class="dropdown-link">
                        <a href="#">More<i class="fas fa-caret-down"></i></a>
                        <div class="dropdown second">
                          <ul>
                            <li class="dropdown-link">
                              <a href="#">Link 1</a>
                            </li>
                            <li class="dropdown-link">
                              <a href="#">Link 2</a>
                            </li>
                            <li class="dropdown-link">
                              <a href="#">Link 3</a>
                            </li>
                            <div class="arrow"></div>
                          </ul>
                        </div>
                      </li>
                      <div class="arrow"></div>
                    </ul>
                  </div>
                </li>
                <li class="dropdown-link">
                  <a href="#">Link 4</a>
                </li>
                <div class="arrow"></div>
              </ul>
            </div>
          </li>
          <li class="nav-link" style="--i: 1.35s">
            <a href="#">Contact</a>
          </li>
        </ul>
      </div>
      <div id="aa"></div>
      <div class="log-sign" style="--i: 1.8s">
        <a href="#" class="btn transparent">Log in</a>
      </div>
    </div>

    <div class="hamburger-menu-container">
      <div class="hamburger-menu">
        <div></div>
      </div>
    </div>
  </div>
</template>
<style scoped>
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
</style>
