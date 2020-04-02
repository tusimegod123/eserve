<template>
  <center>
    <div id="home" class="home">
      <AppHeader />

      <div class="container">
        <!--Nav Bar-->
        <AppNav />
        <!--Online videos-->
        <online-videos />
        <!--container2-->
        <presentations />
        <!--Cheat sheets-->
        <cheat-sheets />
        <!--Books-->
        <books />
      </div>

      <!-- <div class="footer">-->
      <Footer />
    </div>
  </center>
</template>

<script lang="ts">


import AppHeader from "./AppHeader.vue";
import Footer from "./Footer.vue";
import AppNav from "./AppNav.vue";
import OnlineVideos from "./OnlineVideos.vue";
import Presentations from "./Presentations.vue";
import CheatSheets from "./CheatSheets.vue";
import Books from "./Books.vue";

export default {
  name: "Home",
  components: {
    AppHeader,
    Footer,
    AppNav,
    OnlineVideos,
    Presentations,
    CheatSheets,
    Books
    
  }
};
</script>

<style>
h1 {
  background-color: blueviolet;
  color: white;
  /* margin-left: 100px; */
  border-radius: 2px;
}
.form-row {
  color: blueviolet;
  font-weight: bolder;
  font-size: larger;
  text-align: left;
}
.container1 {
  background: rgb(192, 191, 189);
}

.container2 {
  background: rgb(192, 191, 189);
  width: 100%;
}
#footerParagraph1 {
  font-size: 160%;
}
#footerParagraph2 {
  font-size: 120%;
}
.appHeader {
  overflow: hidden;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1000;
}

.navbar a {
  float: left;
  display: block;
  color: #f2f2f2;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}
</style>