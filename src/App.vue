<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="yiduo">
    <div class="top">
      <span class="top-text">北京壹朵视觉科技有限公司</span>
      <span class="top-text">123456789@163.com</span>
      <span class="top-text">17864270133</span>
    </div>
    <div class="nav">
      <img alt="Vue logo" class="nav-logo" src="@/assets/logo.png" />
      <div class="nav-center">
        <div class="nav-items"></div>
      </div>
      <div class="nav-left"></div>
    </div>
    <!-- <RouterLink to="/about">About</RouterLink> -->

    <RouterView />
  </div>
</template>

<style scoped>
.yiduo {
  height: 100%;
  width: 100vw;
  display: flex;
  flex-direction: column;
}
.top {
  height: 26px;
  background-color: #000;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
}
.top-text {
  margin-left: 40px;
  color: #fff;
  font-size: 12px;
}
.nav {
  height: 50px;
  background-color: #fff;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
}

.nav-logo {
  height: 40px;
  width: 120px;
  margin-left: 40px;
}
header {
  line-height: 1.5;
  max-height: 100vh;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
