<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">
        <img class="logo" src="@/assets/Y-logo.jpg" alt="Logo" />
      </router-link>
      <div class="routs">
        <router-link to="/">
          <div @mouseover="home = true" @mouseleave="home = false" class="divLink">
            <transition name="rout" mode="out-in">
              <i class="rout fas fa-home" v-if="home == false"></i>
              <a v-else>home</a>
            </transition>
          </div>
        </router-link>
        <router-link to="/about">
          <div @mouseover="about = true" @mouseleave="about = false" class="divLink">
            <transition name="rout" mode="out-in">
              <i class="rout fas fa-user" v-if="about == false"></i>
              <a v-else>about</a>
            </transition>
          </div>
        </router-link>
        <router-link to="/projects">
          <div @mouseover="projects = true" @mouseleave="projects = false" class="divLink">
            <transition name="rout" mode="out-in">
              <i class="rout fas fa-brain" v-if="projects == false"></i>
              <a class="contact" v-else>projects</a>
            </transition>
          </div>
        </router-link>
        <router-link to="/contact">
          <div @mouseover="contact = true" @mouseleave="contact = false" class="divLink">
            <transition name="rout" mode="out-in">
              <i class="rout far fa-envelope" v-if="contact == false"></i>
              <a class="contact" v-else>contact</a>
            </transition>
          </div>
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
      contact: false,
    };
  },
};
</script>

<style>
@media (max-width: 1000px) {
  .content {
    max-width: 500px;
  }
}
@media (max-width: 670px) {
  .content {
    max-width: 200px;
    font-size: 10px;
  }
}
@media (max-width: 500px) {
  .content {
    font-size: 10px;
  }
}
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
  margin-left: 15%;
  width: 1000px;
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
.divLink {
  height: 20px;
  width: 25px;
  margin-left: -10px;
  padding: 10px 12px;
}
.rout-enter-active,
.rout-leave-active {
  transition: opacity 0.5s;
}
.rout-enter,
.rout-leave-to {
  opacity: 0;
}
</style>
