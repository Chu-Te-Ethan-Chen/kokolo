<template>
  <div class="section-hero">
    <div class="banner-container">
      <div id="carouselExampleIndicators" class="carousel slide baner-list" data-bs-ride="carousel">
        <div class="carousel-indicators">
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
          <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active" style="background-color: #F77E36;">
            <!-- <img src="https://source.unsplash.com/XghsTOU2W24" class="d-block w-100" alt="..."> -->
          </div>
          <div class="carousel-item" style="background-color: aquamarine;">
            <span class="gs-content-layer">
              <span class="gs-content">
                <h1 class="gs-title">A Better Way Forward to <span class="d-inline-block">Smarter, Cleaner Cities</span></h1>
                <span class="gs-desc">Gogoro is reinventing urban transportation with an ecosystem of sustainable energy solutions for the world’s modern cities.</span>
              </span>
            </span>
            <!-- <img src="https://source.unsplash.com/Nh6NsnqYVsI" class="d-block w-100" alt="..."> -->
          </div>
        </div>
      </div>
    </div>
  </div>
  <section class="landing-page-section section-campaign" style="height: 510px; background-color: cornflowerblue;"></section>
  <section class="landing-page-section section-station" style="height: 645px; background-color: lightgreen;"></section>
  <section class="landing-page-section section-media" style="height: 340px; background-color: bisque;"></section>
  <section class="landing-page-section section-eeyo" style="height: 682px; background-color: aliceblue;"></section>
  <section class="landing-page-section section-quotes" style="height: 292px; background-color: lightgreen;"></section>
  <section class="landing-page-section section-impact" style="height: 525px; background-color: lightgreen;"></section>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style lang="scss" scoped>
.banner-container {
  height: calc(100vh - 120px);
  min-height: 680px;
  max-height: 1200px;
}
.baner-list {
  height: 100% !important;
}
.carousel-inner {
  height: 100%;
}
.carousel-item {
  height: 100%;
}
.gs-content-layer {
    position: absolute;
    width: 100%;
    height: 100%;
    left: 0;
    top: 0;
    display: flex;
    align-items: center;
    justify-content: center;
}
.gs-content {
    display: block;
    color: #ffffff;
    max-width: 660px;
    text-align: center;
    padding: 0 16px;
}
.gs-title {
    font-size: 54px;
    margin: 0 0 24px 0;
}
.gs-desc {
    font-size: 20px;
    line-height: 1.2;
    max-width: 500px;
}
.landing-page-section {
    max-width: 1140px;
    margin: auto;
}
.campaign {
    padding-bottom: 0;
    height: 510px;
}
</style>