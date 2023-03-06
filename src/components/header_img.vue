<template>
  <div class="content">
    <div class="cont_bx">
      <h1>
        Search <br />
        house
      </h1>
      <p>3 bedrooms, 1 kitchen, 2 bathrooms</p>
      <div class="weather">
        <h6>42 °C <span>Very Hot</span></h6>
      </div>
      <div class="btns_cont">
        <i class="bi bi-arrow-left" id="btn_left"></i>
        <i class="bi bi-arrow-right" id="btn_right"></i>
      </div>
      <div class="images_bx">
        <div class="card">
          <img src="../assets/images/img11.jpg" alt="" />
        </div>
        <div class="card">
          <img src="../assets/images/im2.jpg" alt="" />
        </div>
        <div class="card">
          <img src="../assets/images/img12.jpg" alt="" />
          <h6 id="h6">+6</h6>
        </div>
      </div>
    </div>
    <div class="choose_bx">
      <div class="stay_bx">
        <button><i class="bi bi-house-door-fill"></i></button>
        <button>
          <span class="material-symbols-rounded" style="font-size: 16px"> chair </span>
        </button>
        <button><i class="bi bi-tv-fill"></i></button>
      </div>
      <div class="select">
        <div class="card">
          <h5>Localisation</h5>
          <input type="text" value="Quartier ..." />
          <input type="text" value="ville ..." />
        </div>
        <div class="card">
          <h5>Categorie</h5>
          <input type="text" value="Appartement" id="categorie" />
          <button id="people_less">prev</button>
          <button id="people_more">next</button>
        </div>
      </div>
    </div>
  </div>
</template>
