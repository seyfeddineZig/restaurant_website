<template>
  <div>
    <nuxt />
  </div>
</template>

<style>
body {
  position: relative;
  padding: 0;
  margin: 0;
  overflow-x: hidden;
}
.carousel-inner img {
  width: 100%;
  height: 100%;
}
* {
  font-family: "Montserrat", sans-serif;
}
.navbar-brand {
  font-family: "Lobster", cursive;
  font-size: 3em;
}
.special-font {
  font-family: "Lobster", cursive;
}
.navbar.bg-transparent {
  position: absolute;
  top: 0;
  width: 100%;
  background: transparent !important;
  z-index: 1000;
}
.navbar.bg-transparent .nav-link {
  font-size: 0.9em;
}
#home-carousel {
  position: relative;
  height: 100vh;
}
#home-carousel .carousel-inner {
  height: 100vh;
}
#home-carousel .carousel-inner img {
  height: 110%;
  width: auto;
}
#home-carousel:before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: rgb(0, 19, 53);
  opacity: 0.9;
  z-index: 1;
}
/* #home-carousel:after {
  content: ".";
  position: absolute;
  left: 50%;
  bottom: 30px;
  width: 30px;
  height: 50px;
  z-index: 1;
  color: #ffd000;
  overflow: hidden;
  text-align: center;
  border: 1px solid white;
  font-size: 50px;
  border: 1px solid white;
  border-radius: 25px;
  line-height: 1cm;
  animation: 0.8s infinite cursorDown;
} */
@keyframes cursorDown {
  0% {
    bottom: 80px;
  }
  50% {
    bottom: 85px;
  }
  100% {
    bottom: 80px;
  }
}

.carousel-caption {
  width: 100vw;
  height: 65%;
  padding: 0%;
  top: 50%;
  left: 50%;
  bottom: inherit;
  transform: translate(-50%, -50%);
}
.carousel-caption h1 {
  font-size: 4em;
  color: #ffd000;
  text-decoration: underline;
}
.carousel-caption h3 {
  font-size: 2.7em;
}
.oxymore-btn {
  text-decoration: none;
  color: #ffd000;
  background: transparent;
  padding: 15px;
  font-size: 1.4em;
  transition: all 0.2s;
  position: relative;
}
.oxymore-btn:hover {
  text-decoration: none;
  color: #ca9e00;
}
.navbar-oxymore-btn {
  text-decoration: none;
  color: #ffd000 !important;
  background: transparent;
  font-size: 0.8em;
  transition: all 0.2s;
}

.contact-infos-container {
  position: absolute;
  background: transparent;
  bottom: 0;
  margin: 0;
  width: 100vw;
  color: #fff;
  z-index: 5;
  font-size: 0.85em;
}
.contact-infos ul {
  list-style: none;
  padding: 0;
}
.contact-infos ul li {
  display: inline;
  margin-left: 5px;
}
.contact-infos-container > .row {
  margin: 0;
}
.contact-infos-container .contact-infos i,
.contact-infos-container .social-media i {
  color: #ffd000;
}

.title {
  position: relative;
  z-index: 1;
  font-size: 3em;
}
.text-on-bg {
  position: absolute;
  font-family: "Lobster", cursive;
  font-size: 1.8em;
  transform: translate(-10%, -50%);
  color: rgb(0, 19, 53);
  opacity: 0.1;
  z-index: 0;
}
.dark .text-on-bg {
  color: #ca9e00;
}

.menus-container {
  background: url("../assets/img/bg.jpg");
  background-size: cover;
  color: white;
}

.menu-item {
  font-family: "Lobster", cursive;
  border-bottom: 1px dotted #ccc;
}
.menu-item .price {
  color: #ca9e00;
}
.menu-item p {
  font-size: 0.85em;
  opacity: 0.7;
}

.event-item .img {
  height: 200px;
  width: 100%;
  background-size: cover;
  background-repeat: no-repeat;
}
.event-item .event-date {
  color: #ca9e00;
}
.event-item .title {
  color: rgb(0, 19, 53);
  font-size: 1.5em;
}
.event-item p {
  font-size: 0.85;
  color: #555;
}
.footer {
  background: rgb(0, 19, 53);
  color: white;
}

.footer table {
  width: 100%;
}
.footer p {
  font-size: 0.85em;
  color: #eee;
}
.footer table td {
  padding: 10px;
}
table.opening td {
  padding-bottom: 20px;
  padding-top: 20px;
}
.opening tr {
  border-bottom: 1px solid #888;
}
.special-color {
  color: #ffd000;
}
.special-color-2 {
  color: rgb(0, 19, 53);
}
.special-btn-2 {
  width: 100%;
  padding: 20px;
  background: rgb(0, 19, 53);
  color: #fff;
  font-family: "Lobster", cursive;
  border: none;
  outline: none;
  font-size: 1.1em;
  border-bottom: 4px solid #ca9e00;
}
</style>
