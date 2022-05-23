<script setup>
// import { RouterLink, RouterView } from 'vue-router'
import AppHeader from '@/components/AppHeader.vue'
</script>

<template>
  <header>
    <div class="wrapper">
      <AppHeader msg="Product Design, UXUI, Frontend Development" />
      <!-- <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav> -->
    </div>
  </header>
  <main>
    <section>
      <div class="wrapper">
        <div class="marquee flex-row">
          <div class="flex-child">
            <h1 class="bold">Aaron Wilson</h1>
            <h2>Product Design,<br>
              UXUI,<br>
              Frontend Development</h2>
            <h3>25+ years designing and building exciting and intuitive user centric web solutions.</h3>
          </div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
    </section>
    <section>
      <div class="gray-row 80">
        <div class="product-design flex-row wrapper">
          <div class="flex-child">Product Design</div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
      <div class="gray-row 60">
        <div class="uiux-design flex-row wrapper">
          <div class="flex-child">UI/UX</div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
      <div class="gray-row 40">
        <div class="fe-development flex-row wrapper">
          <div class="flex-child">Frontend Dev</div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
    </section>
  </main>

  <!-- <RouterView /> -->
</template>

<style>
@import '@/assets/base.css';
header {
  background-color: black;
}

.marquee {
  background-color: white;
}

.gray-row {
  background-color: gray;
  /* & .80 {
    background-color: #7d7d7d;
  } */
}

.product-design {
  background-color: gray;
}

.uiux-design {
  background-color: gray;
}

.fe-development {
  background-color: gray;
}

</style>
