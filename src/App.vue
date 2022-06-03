<template>
  <header>
    <div class="wrapper">
    <div class="header flex-row">
      <div class="flex-child">AW</div>
      <div class="flex-child">Product Design, UXUI, Frontend Development</div>
    </div>
    </div>
  </header>
  <main>
    <section>
      <div class="wrapper">
        <div class="marquee flex-row">
          <div class="flex-child">
            <h1 class="bold">AARON WILSON</h1>
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
      <div class="gray-row eighty">
        <div class="product-design flex-row wrapper">
          <div class="flex-child">Product Design</div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
      <div class="gray-row sixty">
        <div class="uiux-design flex-row wrapper">
          <div class="flex-child">UI/UX</div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
      <div class="gray-row forty">
        <div class="fe-development flex-row wrapper">
          <div class="flex-child">Frontend Dev</div>
          <div class="flex-child">Graphic Area</div>
        </div>
      </div>
    </section>
    <section>
      <div class="work-experience">
        <div class="wrapper">
          <div class="arrow-left"></div>
          <div class="content-area">
          <SlideShow/>
          </div>
          <div class="arrow-right"></div>
        </div>
      </div>
    </section>
  </main>
  <footer>
    <div class="wrapper">
      This is the footer
    </div>
  </footer>

  <!-- <RouterView /> -->
</template> 

<style lang="scss" scoped>
@import '@/assets/normalize.scss';
@import '@/assets/base.scss';

header, footer {
  background-color: black;
}
footer {
  color: white;
  padding:20px;
}
.work-experience {
  padding: 40px 0;
}
.marquee {
  background-color: white;
  h1 {
    font-family: 'Open Sans', sans-serif;
    font-size:6rem;
    padding:  20px 0 0 0;
    margin:0;
    font-weight: 800;
    line-height:6rem;
  }
  h2 {
    font-size: 2.2rem;
    padding: 10px 0 0 0;
    margin:0;
  }
  h3 {
    font-size: 1.6rem;
    padding: 20px 0;
    margin:0;
  }
}

.gray-row {
  font-size: 2rem;
  color: white;
  &.eighty {
    background-color: green;
  }
  &.sixty {
    background-color: blue;
  }
  &.forty {
    background-color: orange;
  }
  
}

.product-design,
.uiux-design,
.fe-development
 {
  padding: 40px 0px;
}

</style>
<script>
import SlideShow from './components/SlideShow.vue';

export default {
  components: {
    SlideShow
  }
}
</script>

