<template>
  <div class="wrapper">
    <Navbar v-on:toggle-booking-form="toggleBookingForm"></Navbar>
    <HomeCarousel v-on:toggle-booking-form="toggleBookingForm"></HomeCarousel>
    <About></About>
    <Menus></Menus>
    <Events></Events>
    <Footer></Footer>
    <BookingForm :display="showBookingForm" v-on:toggle-booking-form="toggleBookingForm"></BookingForm>
    <BookingForm :display="showLoginForm" v-on:toggle-login-form="toggleLoginForm"></BookingForm>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import HomeCarousel from "@/components/HomeCarousel";
import About from "@/components/About";
import Menus from "@/components/Menus";
import Events from "@/components/Events";
import Footer from "@/components/Footer";
import BookingForm from "@/components/BookingForm";
import LoginForm from "@/components/LoginForm";

export default {
  data() {
    return {
      showBookingForm: false,
      showLoginForm: false
    };
  },
  components: {
    Navbar,
    HomeCarousel,
    About,
    Menus,
    Events,
    Footer,
    BookingForm,
    LoginForm
  },
  methods: {
    toggleBookingForm() {
      this.showBookingForm = !this.showBookingForm;
    },
    toggleLoginForm() {
      this.showLoginForm = !this.showLoginForm;
    }
  }
};
</script>

<style>
</style>
