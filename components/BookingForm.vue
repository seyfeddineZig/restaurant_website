<template>
  <div
    v-bind:class="['container-fluid booking-form-container', display?' active':'']"
    v-bind:style="{'left': display?'0%':'100%'}"
  >
    <div class="row form-container">
      <div class="col-md-8" @click="$emit('toggle-booking-form')"></div>
      <div class="col-md-4 booking-form p-5">
        <button class="close-btn" @click="$emit('toggle-booking-form')"></button>
        <form action class="p-5 pt-3">
          <h2 class="special-font mb-5 special-color-2">Réserver une table</h2>
          <div class="form-group">
            <label for="booking-date" class="special-font">Date de résrevation</label>
            <input type="text" class="form-control" />
          </div>
          <div class="form-group">
            <label for="booking-date" class="special-font">Durée</label>
            <input type="text" class="form-control" />
          </div>
          <div class="form-group">
            <label for="booking-date" class="special-font">Nombre de personnes</label>
            <input type="text" class="form-control" />
          </div>
          <div class="form-group mt-5">
            <button type="submit" class="special-btn-2">Vérifier la disponibilité</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  props: ["display"]
};
</script>
<style>
.booking-form-container {
  position: fixed;
  top: 0;
  left: 100%;
  height: 100vh;
  width: 100vw;
  transition: all 0.7s;
  z-index: 10000;
}
.booking-form {
  background: white;
  height: 100vh;
}
.booking-form-container:before {
  content: "";
  position: absolute;
  left: 100%;
  top: 0;
  height: 100%;
  width: 100%;
  background: rgb(0, 19, 53);
  opacity: 0.7;
  transition: all 0.6s;
  transition-delay: 0.3s;
}
.booking-form-container.active:before {
  left: 0%;
}
.form-group label {
  font-size: 1em;
  color: rgb(0, 19, 53);
}
.form-control {
  padding: 30px;
  border-radius: 0px;
  border-color: #ccc;
}
.close-btn {
  position: absolute;
  right: 50px;
  top: 10px;
  height: 40px;
  width: 40px;
  background: transparent;
  border: 1px solid #111;
  outline: none;
  box-shadow: none;
  cursor: pointer;
}
.close-btn:before {
  content: "";
  position: absolute;
  left: 0%;
  top: 50%;
  width: 100%;
  height: 1px;
  background: #111;
  transform: rotate(45deg);
  cursor: pointer;
}
.close-btn:after {
  content: "";
  position: absolute;
  left: 0%;
  top: 50%;
  width: 100%;
  height: 1px;
  background: #111;
  transform: rotate(45deg);
  transition: all 0.2s;
  cursor: pointer;
}
.close-btn:hover::after {
  transform: rotate(135deg);
}
</style>