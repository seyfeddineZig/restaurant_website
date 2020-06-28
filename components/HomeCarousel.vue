<template>
  <div id="home-carousel" class="carousel slide" data-ride="carousel">
    <!--<ul class="carousel-indicators">
          <li
            data-target="#home-carousel"
            data-slide-to="0"
            class="active"
          ></li>
          <li data-target="#home-carousel" data-slide-to="1"></li>
          <li data-target="#home-carousel" data-slide-to="2"></li>
    </ul>-->
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/img/restaurant_3.jpg" alt="Los Angeles" width="1100" height="500" />
        <div class="carousel-caption">
          <h1 class="special-font">
            <i class="fas fa-utensils"></i>
            <br />Oxymore
          </h1>
          <h3 class="special-font">Bienvenue sur notre site</h3>
          <p>réservez une table et célébrez votre succès avec nous</p>
          <div class="mb-4"></div>
          <a
            class="oxymore-btn special-font"
            href="#"
            @click="$emit('toggle-booking-form')"
          >Réserver maintenant !</a>
        </div>
      </div>
      <!--<div class="carousel-item">
            <img
              src="img/restaurant_2.jpg"
              alt="Chicago"
              width="1100"
              height="500"
            />
            <div class="carousel-caption">
              <h3>Chicago</h3>
              <p>Thank you, Chicago!</p>
            </div>
          </div>
          <div class="carousel-item">
            <img
              src="img/restaurant_3.jpg"
              alt="New York"
              width="1100"
              height="500"
            />
            <div class="carousel-caption">
              <h3>New York</h3>
              <p>We love the Big Apple!</p>
            </div>
          </div>
      -->
    </div>
    <!--<a
          class="carousel-control-prev"
          href="#home-carousel"
          data-slide="prev"
        >
          <span class="carousel-control-prev-icon"></span>
        </a>
        <a
          class="carousel-control-next"
          href="#home-carousel"
          data-slide="next"
        >
          <span class="carousel-control-next-icon"></span>
    </a>-->
    <div class="contact-infos-container">
      <div class="row">
        <div class="col-md-12 contact-infos">
          <ul>
            <li class="mr-4">
              <i class="fas fa-map-marker-alt"></i> 05 Rue Lorem ipsum Lorem
              ipsum Lorem ipsum ....
            </li>
            <li class="mr-4">
              <i class="fas fa-phone fa-flip-horizontal"></i>
              +213662891428 / +213662891428
            </li>
            <li class>
              <i class="fab fa-facebook"></i>
            </li>
            <li>
              <i class="fab fa-twitter-square"></i>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style>
</style>