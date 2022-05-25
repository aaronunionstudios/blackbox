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
            <h1 class="bold">Aaron Wilson 2</h1>
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

February 2017 - Present
CastleBranch

Location: Wilmington, NC

Position: UI/UX Manager

Manage team of Front End Designers and Developers to craft solutions for new features and functionality within the suite of CastleBrach product offerings, with a focus on usability and user flow. Develop new functionality and features within a Laravel stack using KendoUI, Vue.js, Vanilla Javascript, SASS and HTML. Work directly with Product Management to review business requirements and create functional requirements, as well as wireframes, mockups and clickable prototypes. Conduct key stakeholder meetings to review prototypes and present solutions for approval. Work directly with leadership to construct new SDLC process and implement within the engineering department. Interact with Quality Assurance department to review test plans and to help with feature testing. Manage all Front End development projects with emphasis on delivery dates, update leadership team on deliverables and the projects status.

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
}
.work-experience {
  padding: 40px 0;
}
.marquee {
  background-color: white;
  h1 {
    font-size:4rem;
    padding: 20px 0;
  }
  h2 {
    font-size: 2.8rem;
    padding: 20px 0;
  }
  h3 {
    font-size: 1.8rem;
    padding: 20px 0;
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
