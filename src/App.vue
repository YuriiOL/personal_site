<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">
        <img class="logo" src="@/assets/Y-logo.jpg" alt="Logo" />
      </router-link>
      <div class="routs">
        <router-link to="/">
          <i class="rout fas fa-home" @mouseover="home = true" v-if="home == false"></i>
          <a v-else @mouseleave="home = false">home</a>
        </router-link>
        <router-link to="/about">
          <i class="rout fas fa-user" @mouseover="about = true" v-if="about == false"></i>
          <a v-else @mouseleave="about = false">about</a>
        </router-link>
        <router-link to="/projects">
          <i class="rout fas fa-brain" @mouseover="projects = true" v-if="projects == false"></i>
          <a class="contact" v-else @mouseleave="projects = false">projects</a>
        </router-link>
        <router-link to="/contact">
          <i class="rout far fa-envelope" @mouseover="contact = true" v-if="contact == false"></i>
          <a class="contact" v-else @mouseleave="contact = false">contact</a>
        </router-link>
      </div>
      <div class="links">
        <a href="https://www.instagram.com/beerjurassic/">
          <i class="link fab fa-instagram"></i>
        </a>
        <a href="https://www.facebook.com/yura.oleksovskiy">
          <i class="link fab fa-facebook"></i>
        </a>
        <a href="https://github.com/YuriiOL">
          <i class="link fab fa-github"></i>
        </a>
      </div>
    </div>
    <transition name="slide" mode="out-in">
      <router-view class="content" />
    </transition>
  </div>
</template>
<script>
export default {
  data() {
    return {
      home: false,
      about: false,
      projects: false,
      contact: false
    };
  }
};
</script>

<style>
.slide-enter-active,
.slide-leave-active {
  transition: opacity 0.7s, transform 0.7s;
}
.slide-enter {
  opacity: 0;
  transform: translateX(-30%);
}
.slide-leave-to {
  opacity: 0;
  transform: translateX(30%);
}

body {
  margin: 0px;
  background-color: rgb(29, 29, 29);
}
.link {
  color: white;
  margin-left: 5px;
}

#nav {
  display: flex;
  width: 50px;
  height: 100%;
  flex-direction: column;
  position: fixed;
  top: 0;
  min-height: 500px;
  background-color: rgb(24, 24, 24);
  justify-content: space-between;
  z-index: 1;
}

.routs,
.links {
  height: 70px;
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
  flex-direction: column;
  padding: 15px;
}

a {
  color: orangered;
  font-size: 15px;
  text-decoration: none;
  margin-left: -5px;
}
.contact {
  margin-left: -7px;
  font-size: 13px;
}

.routs {
  height: 180px;
}
.fab:hover {
  color: orangered;
}
.content {
  position: fixed;
  margin-left: 50px;
  width: 100%;
  height: 100%;
  background-color: rgb(29, 29, 29);
  color: white;
  display: flex;
  align-items: center;
  padding-left: 10%;
}
.logo {
  width: 55px;
  height: auto;
  margin: 0 auto;
}
.rout {
  color: white;
}
</style>
