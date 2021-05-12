<template>
  <div class="section-hero">
    <div class="banner-container">
      <div
        class="banner-list slick-initialized slick-slider slick-dotted"
        role="toolbar"
      >
        <div aria-live="polite" class="slick-list draggable">
          <div
            class="slick-track"
            role="listbox"
            style="opacity: 1; width: 2708px;"
          >
            <div
              class="banner banner--viva-mix slick-slide slick-current slick-active"
              data-theme="dark"
              data-slick-index="0"
              aria-hidden="false"
              tabindex="-1"
              role="option"
              aria-describedby="slick-slide00"
              style="width: 1354px; position: relative; left: 0px; top: 0px; z-index: 999; opacity: 1;"
            >
              <div class="banner-content-layer">
                <h2 class="banner-title">
                  Gogoro <span class="banner-title__model">VIVA MIX</span>
                </h2>
                <div class="banner-slogan">
                  MIX IT UP
                </div>
                <div class="banner-actions">
                  <a
                    class="banner-cta"
                    href="/smartscooter/viva/mix/"
                    tabindex="0"
                    >learn more</a
                  >
                </div>
              </div>
            </div>
            <a
              href="/about/"
              class="hero gs-hero slick-slide"
              data-theme="dark"
              data-slick-index="1"
              aria-hidden="true"
              tabindex="-1"
              role="option"
              aria-describedby="slick-slide01"
              style="width: 1354px; position: relative; left: -1354px; top: 0px; z-index: 998; opacity: 0; transition: opacity 500ms ease 0s;"
            >
              <video
                class="gs-video"
                muted=""
                playsinline=""
                autoplay=""
                loop=""
                onplay="this.style.opacity = 1;"
                style="opacity: 1;"
              >
                <source
                  src="//cdn.gogoro.com/resources/pages/landing-page/gs0528/home_vision_1080_v02.mp4"
                  type="video/mp4"
                />
              </video>
              <span class="gs-content-layer">
                <span class="gs-content">
                  <h1 class="gs-title">
                    A Better Way Forward to
                    <span class="d-inline-block">Smarter, Cleaner Cities</span>
                  </h1>
                  <span class="gs-desc"
                    >Gogoro is reinventing urban transportation with an
                    ecosystem of sustainable energy solutions for the world’s
                    modern cities.</span
                  >
                </span>
              </span>
            </a>
          </div>
        </div>

        <ul class="slick-dots" style="" role="tablist">
          <li
            aria-hidden="false"
            role="presentation"
            aria-selected="true"
            aria-controls="navigation00"
            id="slick-slide00"
            @click="activateSlickDot(1)"
            :class="{ 'slick-active': slickItemActive == 1 }"
          >
            <button type="button" data-role="none" role="button" tabindex="0">
              1
            </button>
          </li>
          <li
            aria-hidden="true"
            role="presentation"
            aria-selected="false"
            aria-controls="navigation01"
            id="slick-slide01"
            @click="activateSlickDot(2)"
            :class="{ 'slick-active': slickItemActive == 2 }"
          >
            <button type="button" data-role="none" role="button" tabindex="0">
              2
            </button>
          </li>
        </ul>
      </div>
    </div>
  </div>
  <section class="landing-page-section section-campaigns">
    <ul class="campaign-list campaign-list--3">
      <li class="campaign-item">
        <a
          class="campaign
        campaign--dark
        campaign--top"
          href="http://www.gogoro.com/gogoro-network/"
          target="_self"
        >
          <div class="campaign-copy-wrapper">
            <div class="campaign-copy">
              <h2 class="campaign-title">Smarter Energy</h2>
              <div class="campaign-subtitle">
                Battery swapping is cleaner, faster &amp; easier
              </div>
            </div>
          </div>
          <span
            class="campaign-bg"
            :style="{
              'background-image': `url(${require('@/assets/2-campaign1-background-e3b88377e474f0386c7bfbc9f442227c73d79865.png')})`,
            }"
          ></span>
        </a>
      </li>
      <li class="campaign-item">
        <a
          class="campaign
        campaign--dark
        campaign--top"
          href="http://www.gogoro.com/smartscooter/2-series/plus/"
          target="_self"
        >
          <div class="campaign-copy-wrapper">
            <div class="campaign-copy">
              <h2 class="campaign-title">Smarter Rides</h2>
              <div class="campaign-subtitle">
                Experience a ride like no other
              </div>
            </div>
          </div>
          <span
            class="campaign-bg"
            :style="{
              'background-image': `url(${require('@/assets/2-campaign2-background-a4b8ef537d3b88a684eee733d9886a9634c9564a.png')})`,
            }"
          ></span>
        </a>
      </li>
      <li class="campaign-item">
        <a
          class="campaign
        campaign--dark
        campaign--top"
          href="https://www.ridegoshare.com/"
          target="_self"
        >
          <div class="campaign-copy-wrapper">
            <div class="campaign-copy">
              <h2 class="campaign-title">Smarter Sharing</h2>
              <div class="campaign-subtitle">
                Ride when you like, swap as you go
              </div>
            </div>
          </div>
          <span
            class="campaign-bg"
            :style="{
              'background-image': `url(${require('@/assets/2-campaign3-background-e608d89f7f5e1dd4ca01da871c9f2d18fa4ceb3b.png')})`,
            }"
          ></span>
        </a>
      </li>
    </ul>
  </section>
  <section class="landing-page-section section-station">
    <div class="station-content-container">
      <div class="station-brand">Gogoro Network</div>
      <div class="station-caption">
        The largest battery swapping network
        <span class="d-inline-block">in the world</span>
      </div>
      <div class="station-desc">
        Gogoro Network® manages over
        <span class="em">200,000 battery swaps a day</span> at
        <span data-dynamic-var="stationsCount">2,093</span> GoStation® across
        Taiwan, that's enough power to ride 15,000,000 km.
      </div>
      <a href="https://network.gogoro.com/tw/en/coverage/" class="gs-cta">
        SEE OUR NETWORK
      </a>
    </div>

    <figure class="image-station"></figure>
  </section>
  <section class="landing-page-section section-media">
    <div class="media-container-wrapper">
      <div class="media-container blog-posts-container">
        <div class="media-section-name">
          5 Partners and Growing
        </div>
        <ul class="blog-post-list slick-initialized slick-slider">
          <div aria-live="polite" class="slick-list draggable">
            <div
              class="slick-track"
              role="listbox"
              style="opacity: 1; width: 567px;"
            >
              <li
                class="social-post-item slick-slide slick-current slick-active"
                data-slick-index="0"
                aria-hidden="false"
                tabindex="-1"
                role="option"
                aria-describedby="slick-slide10"
                style="width: 567px; position: relative; left: 0px; top: 0px; z-index: 999; opacity: 1;"
              >
                <a
                  class="social-post social-post--light"
                  target="_blank"
                  href="https://network.gogoro.com/tw/en/scooter/"
                  tabindex="0"
                >
                  <div class="social-post-copy-wrapper">
                    <div class="social-post-copy">
                      <h3 class="social-post-title media-item-title">
                        Powered by<br />Gogoro Network
                      </h3>
                      <div class="social-post-subtitle"></div>
                    </div>
                  </div>
                  <span
                    class="social-post-bg"
                    :style="{
                      'background-image': `url(${require('@/assets/2-blog-post1-background-cd09a35997763fe78b226f247857bef12f02d0a6.png')})`,
                    }"
                  ></span>
                </a>
              </li>
            </div>
          </div>
        </ul>
      </div>
      <div class="media-container social-media-container">
        <div class="media-section-name">
          Blog
        </div>
        <ul class="social-post-list">
          <li class="social-post-item">
            <a
              class="social-post social-post--"
              target="_blank"
              href="https://www.gogoro.com/news/Gogoro-Battery-Swapping-India-Hero/"
            >
              <div class="social-post-copy-wrapper">
                <div class="social-post-copy">
                  <h3 class="social-post-title media-item-title">
                    Hero &amp; Gogoro<br />heads to India
                  </h3>
                  <div class="social-post-subtitle"></div>
                </div>
              </div>
              <span
                class="social-post-bg"
                :style="{
                  'background-image': `url(${require('@/assets/2-social-post-background-56588be5a509ae7d8125699fa4a6a5757930e33a.jpg')})`,
                }"
              ></span>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </section>
  <section class="landing-page-section section-eeyo">
    <div class="eeyo-content">
      <h3 class="eeyo-title">
        Introducing <br class="d-sm-none" />Gogoro Eeyo
      </h3>
      <p class="eeyo-desc">
        From the cloud to the road, this is eBike reimagined. Ultralight,
        totally digital, and an absolute blast to ride.
      </p>
      <a class="gs-cta" target="_blank" href="https://eeyo.bike">LEARN MORE</a>
    </div>
    <figure class="image-eeyo"></figure>
  </section>
  <section class="landing-page-section section-quotes">
    <div class="quote-text-list slick-initialized slick-slider">
      <div aria-live="polite" class="slick-list draggable">
        <div
          class="slick-track"
          role="listbox"
          style="opacity: 1; width: 6720px;"
        >
          <a
            target="_blank"
            class="quote-link slick-slide"
            href="http://www.wired.co.uk/article/al-gore-generation-sustainable-capitalism"
            data-slick-index="0"
            aria-hidden="true"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide30"
            style="width: 1120px; position: relative; left: 0px; top: 0px; z-index: 998; opacity: 0; transition: opacity 500ms ease 0s;"
          >
            <blockquote>
              <q class="quote-text"
                >You have to see it to really appreciate how cool it is,</q
              >
              <footer>
                <cite class="quote-cite">Al Gore, Wired, December 2017</cite>
              </footer>
            </blockquote> </a
          ><a
            target="_blank"
            class="quote-link slick-slide"
            href="http://time.com/4169302/ces-2016-coolest/"
            data-slick-index="1"
            aria-hidden="true"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide31"
            style="width: 1120px; position: relative; left: -1120px; top: 0px; z-index: 998; opacity: 0; transition: opacity 500ms ease 0s;"
          >
            <blockquote>
              <q class="quote-text">The 9 Coolest Gadgets from CES 2016</q>
              <footer>
                <cite class="quote-cite">Time</cite>
              </footer>
            </blockquote> </a
          ><a
            target="_blank"
            class="quote-link slick-slide"
            href="https://www.cleantech.com/release/cleantech-group-unveils-the-2018-global-cleantech-100-list/"
            data-slick-index="2"
            aria-hidden="true"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide32"
            style="width: 1120px; position: relative; left: -2240px; top: 0px; z-index: 998; opacity: 0; transition: opacity 500ms ease 0s;"
          >
            <blockquote>
              <q class="quote-text">2018 Asian Company of the Year</q>
              <footer>
                <cite class="quote-cite">Cleantech 100</cite>
              </footer>
            </blockquote> </a
          ><a
            target="_blank"
            class="quote-link slick-slide slick-current slick-active"
            href="https://www.theverge.com/2015/1/9/7509787/verge-awards-best-of-ces-2015"
            data-slick-index="3"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide33"
            style="width: 1120px; position: relative; left: -3360px; top: 0px; z-index: 999; opacity: 1;"
          >
            <blockquote>
              <q class="quote-text">2015 CES Best In Show Award</q>
              <footer>
                <cite class="quote-cite">The Verge</cite>
              </footer>
            </blockquote> </a
          ><a
            target="_blank"
            class="quote-link slick-slide"
            href="https://asia.nikkei.com/magazine/20180111/Business/Gogoro-wins-the-Nikkei-Asian-Review-Award-for-Excellence"
            data-slick-index="4"
            aria-hidden="true"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide34"
            style="width: 1120px; position: relative; left: -4480px; top: 0px; z-index: 998; opacity: 0; transition: opacity 500ms ease 0s;"
          >
            <blockquote>
              <q class="quote-text"
                >2017 Nikkei Asian Review Award for Excellence</q
              >
              <footer>
                <cite class="quote-cite">Nikkei Asian Review</cite>
              </footer>
            </blockquote> </a
          ><a
            target="_blank"
            class="quote-link slick-slide"
            href="http://blog.gogoro.com/en/gogoro-selected-for-the-2016-sustainia100"
            data-slick-index="5"
            aria-hidden="true"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide35"
            style="width: 1120px; position: relative; left: -5600px; top: 0px; z-index: 998; opacity: 0; transition: opacity 500ms ease 0s;"
          >
            <blockquote>
              <q class="quote-text">Selected for the 2016 Sustainia 1000</q>
              <footer>
                <cite class="quote-cite">Sustainia</cite>
              </footer>
            </blockquote>
          </a>
        </div>
      </div>
    </div>
    <div class="quote-logo-list slick-initialized slick-slider">
      <div aria-live="polite" class="slick-list draggable">
        <div
          class="slick-track"
          role="listbox"
          style="opacity: 1; width: 30000px; transform: translate3d(-60px, 0px, 0px);"
        >
          <div
            class="quote-logo-item slick-slide slick-active"
            data-slick-index="0"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide20"
          >
            <div class="quote-logo quote-logo--wired"></div>
          </div>
          <div
            class="quote-logo-item slick-slide slick-active"
            data-slick-index="1"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide21"
          >
            <div class="quote-logo quote-logo--time"></div>
          </div>
          <div
            class="quote-logo-item slick-slide slick-active"
            data-slick-index="2"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide22"
          >
            <div class="quote-logo quote-logo--cleantech"></div>
          </div>
          <div
            class="quote-logo-item slick-slide slick-current slick-active"
            data-slick-index="3"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide23"
          >
            <div class="quote-logo quote-logo--verge"></div>
          </div>
          <div
            class="quote-logo-item slick-slide slick-active"
            data-slick-index="4"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide24"
          >
            <div class="quote-logo quote-logo--nikkei"></div>
          </div>
          <div
            class="quote-logo-item slick-slide slick-active"
            data-slick-index="5"
            aria-hidden="false"
            tabindex="-1"
            role="option"
            aria-describedby="slick-slide25"
          >
            <div class="quote-logo quote-logo--sustania"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section class="landing-page-section section-impact">
    <div class="container">
      <div class="impact-headline">Our community’s impact</div>
      <div class="row">
        <div class="col-lg-8 col-lg-offset-2">
          <div class="impact-item-list">
            <div
              @click="activateImpactDot(1)"
              :class="{ active: impactItemAcitve == 1 }"
              class="impact-item"
            >
              <div class="impact-animation impact-animation--co2">
                <div
                  class="impact-co2-cloud"
                  style="transform: translate3d(0px, 1.6608px, 0px);"
                ></div>
                <div
                  class="impact-co2-arrow"
                  style="opacity: 0.4152; transform: translate3d(0px, 3.8925px, 0px);"
                ></div>
                <div class="impact-co2-tree"></div>
              </div>
              <div class="impact-badge">
                <span class="impact-value">
                  <span class="impact-value" data-dynamic-var="CO2"
                    >276,034,626</span
                  >
                  <span class="impact-unit">KG</span>
                </span>
                <div class="impact-caption">CO2 saved</div>
                <div class="impact-desc">
                  As many as the amount of CO2 that
                  <span
                    data-dynamic-var="CO2"
                    data-dynamic-eval="Math.floor($/10)"
                    >27,603,462</span
                  >
                  trees consume every year.
                </div>
              </div>
            </div>

            <div
              @click="activateImpactDot(2)"
              :class="{ active: impactItemAcitve == 2 }"
              class="impact-item "
            >
              <div class="impact-animation impact-animation--batteries">
                <div class="impact-battery-charger">
                  <div class="impact-battery-seat impact-battery-seat--left">
                    <div
                      class="impact-battery"
                      style="opacity: 0; transform: matrix(1, 0, 0, 1, 0, 0);"
                    >
                      <div
                        class="impact-battery-energy"
                        style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 30);"
                      ></div>
                    </div>
                  </div>
                  <div class="impact-battery-seat impact-battery-seat--right">
                    <div
                      class="impact-battery"
                      style="opacity: 0; transform: matrix(1, 0, 0, 1, 0, 0);"
                    >
                      <div
                        class="impact-battery-energy"
                        style="opacity: 1; transform: matrix(1, 0, 0, 1, 0, 30);"
                      ></div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="impact-badge">
                <span class="impact-value">
                  <span class="impact-value" data-dynamic-var="Swap"
                    >182,489,080</span
                  >
                  <span class="impact-unit"></span>
                </span>
                <div class="impact-caption">Batteries swapped</div>
                <div class="impact-desc">
                  There are more than
                  <span
                    data-dynamic-var="SwapAvg30Days"
                    data-dynamic-eval="Math.floor($)"
                    >280,801</span
                  >
                  batteries swapped per day in the last 30 days.
                </div>
              </div>
            </div>

            <div
              @click="activateImpactDot(3)"
              :class="{ active: impactItemAcitve == 3 }"
              class="impact-item"
            >
              <div class="impact-animation impact-animation--earth">
                <div
                  class="impact-earth"
                  style="transform: translate3d(0px, -1.557px, 0px);"
                >
                  <div
                    class="impact-earth-track"
                    style="transform: matrix3d(0.918066, -0.396427, 0, 0, 0.396427, 0.918066, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1);"
                  ></div>
                </div>
              </div>
              <div class="impact-badge">
                <span class="impact-value">
                  <span class="impact-value" data-dynamic-var="Mileage"
                    >3,347,075,143</span
                  >
                  <span class="impact-unit">KM</span>
                </span>
                <div class="impact-caption">Total distance covered</div>
                <div class="impact-desc">
                  As long as the distance traveling around the Earth via equator
                  <span
                    data-dynamic-var="Mileage"
                    data-dynamic-eval="Math.floor($/40000)"
                    >83,676</span
                  >
                  times.
                </div>
              </div>
            </div>
          </div>
          <div class="impact-dots">
            <div
              @click="activateImpactDot(1)"
              :class="{ active: impactItemAcitve == 1 }"
              class="impact-dot"
            ></div>
            <div
              @click="activateImpactDot(2)"
              :class="{ active: impactItemAcitve == 2 }"
              class="impact-dot"
            ></div>
            <div
              @click="activateImpactDot(3)"
              :class="{ active: impactItemAcitve == 3 }"
              class="impact-dot"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Home",
  data() {
    return {
      impactItemAcitve: 1,
      slickItemActive: 1,
    };
  },
  methods: {
    activateImpactDot(el) {
      this.impactItemAcitve = el;
    },
    activateSlickDot(el){
      this.slickItemActive = el;
    }
  },
};
</script>

<style lang="scss" scoped>
.banner-container {
  position: relative;
  height: calc(100vh - 80px);
  min-height: 420px;
  max-height: 760px;
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
.section-campaigns {
  margin: 6px auto;
  overflow: hidden;
}
.campaign-list {
  padding: 0;
  margin: 0;
  list-style: none;
  text-align: center;
}
:lang(en) .campaign {
  padding-bottom: 0;
  height: 510px;
}
.campaign {
  position: relative;
  display: block;
  padding-bottom: 56.25%;
}
.campaign-copy-wrapper {
  position: absolute;
  height: 35%;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  display: flex;
  box-pack: center;
  -moz-justify-content: center;
  -ms-justify-content: center;
  -o-justify-content: center;
  justify-content: center;
  -ms-flex-pack: center;
  box-align: center;
  -moz-align-items: center;
  -ms-align-items: center;
  -o-align-items: center;
  align-items: center;
  -ms-flex-align: center;
}
:lang(en) .campaign-copy-wrapper {
  height: initial;
  top: 60px;
}
.campaign-title {
  font-family: "graphik-semib", "PingFangTC-Semibold", "Noto Sans Bold";
  font-size: 18px;
  margin-bottom: 0px;
  color: #323237;
}
.campaign-title {
  font-size: 28px;
  line-height: 28px;
  font-weight: 500;
  font-family: var(--font-family-base);
}
.campaign-subtitle {
  font-size: 16px;
  color: #323237;
}
:lang(en) .campaign-subtitle {
  line-height: 1.25;
  margin: 8px 0 0 0;
}
.campaign-bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  display: block;
  background-size: auto 100%;
  background-position: center;
  background-repeat: no-repeat;
}
.section-station {
  overflow: hidden;
  position: relative;
  margin: 6px auto;
  background-image: linear-gradient(52deg, #40fdcb, #40fdcb 7%, #24ee2c);
}
.station-content-container {
  width: 100%;
  text-align: center;
  padding: 52px 0 16px 0;
}
:lang(en) .station-content-container {
  display: block;
  height: initial;
  padding: 0 32px;
  text-align: center;
}
.station-content-container > div {
  width: 100%;
}
:lang(en) .station-brand {
  font-size: 18px;
  font-weight: 600;
  opacity: 0.7;
  margin: 0 0 24px 0;
}
:lang(en) .station-caption {
  font-size: 28px;
  font-weight: 500;
  line-height: 1.1;
  letter-spacing: -0.5px;
  margin: 4px auto 20px auto;
  max-width: 380px;
}
:lang(en) .station-desc {
  font-size: 16px;
  line-height: 1.25;
  max-width: 400px;
  margin: 0 auto 32px auto;
}
.gs-cta {
  display: inline-flex;
  align-items: center;
  letter-spacing: 0.1668em;
  opacity: 0.7;
  font-size: 16px;
  font-weight: 800;
  font-family: var(--font-family-italic);
}
.gs-cta,
.gs-cta:focus,
.gs-cta:hover {
  color: inherit;
}
:lang(en) .section-station .gs-cta {
  margin: 0 0 40px 0;
}
.image-station {
  max-width: 380px;
  margin: 0 auto;
}
.image-station::before {
  content: "";
  display: block;
  padding-bottom: 94.54409567%;
  background: url("~@/assets/station-gn@2x.png") center bottom/contain no-repeat;
}
.section-media {
  margin: 6px auto;
  overflow: hidden;
}
.media-container {
  position: relative;
}
.media-section-name {
  pointer-events: none;
  position: absolute;
  z-index: 3;
  text-align: center;
  left: 0;
  top: 0;
  width: 100%;
  margin-top: 0.75em;
}
.media-item-title,
.media-section-name {
  color: #fff;
  font-family: "graphik-b", "Noto Sans Black";
  line-height: 1.28;
}
.media-section-name {
  font-size: 20px;
}
:lang(en) .media-section-name {
  font-size: 18px;
  margin: 0;
  top: 40px;
  font-weight: 600;
  font-family: var(--font-family-base);
}
.slick-slider {
  position: relative;
  display: block;
  box-sizing: border-box;
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  touch-action: pan-y;
  -webkit-tap-highlight-color: transparent;
}
.social-post-list,
.blog-post-list {
  position: relative;
  list-style: none;
  margin: 0;
}
.blog-post-list {
  padding-bottom: 56.25%;
}
:lang(en) .social-post-list,
:lang(en) .blog-post-list {
  padding-bottom: 0;
  height: 510px;
}
.slick-list {
  position: relative;
  overflow: hidden;
  display: block;
  margin: 0;
  padding: 0;
}
.social-post-list .slick-list,
.blog-post-list .slick-list {
  position: absolute;
  left: 0;
  width: 100%;
}
.slick-track {
  position: relative;
  left: 0;
  top: 0;
  display: block;
}
.banner-list,
.slick-list,
.slick-track {
  height: 100% !important;
}
.banner-list {
  visibility: hidden;
}
.slick-dotted.slick-slider {
  margin-bottom: 30px;
}
.slick-dotted.slick-slider {
  margin-bottom: 0;
}
.banner-list.slick-initialized {
  visibility: visible;
}
.slick-slider .slick-track,
.slick-slider .slick-list {
  transform: translate3d(0, 0, 0);
}
.slick-track:before,
.slick-track:after {
  content: "";
  display: table;
}
.slick-track:after {
  clear: both;
}
.slick-slide {
  float: left;
  height: 100%;
  min-height: 1px;
  display: none;
}
.banner-content-layer {
  position: absolute;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  bottom: 8.5%;
}
.banner--viva-mix .banner-content-layer {
  bottom: 0;
  top: 65%;
}
:lang(en) .banner--viva-mix .banner-content-layer {
  top: 72%;
}
.banner-title {
    font-family: inherit;
    font-weight: 400;
    line-height: 1;
    margin: 0 0 .428em 0;
    font-size: 8vw;
}
.banner--viva-mix .banner-title {
    display: none;
}
.banner-title__model {
    font-weight: 700;
}
.banner-slogan {
    letter-spacing: .1em;
    font-weight: 700;
    margin: 0 0 1.26em 0;
    font-size: 3.76vw;
}
.banner--viva-mix {
    background: url(//cdn.gogoro.com/resources/images/landing-page/viva-mix/hb-viva-mix-scooter-mobile.png) center/180% no-repeat,url(//cdn.gogoro.com/resources/images/landing-page/viva-mix/hb-viva-mix-bg-mobile.jpg?v1) center/cover no-repeat;
}
.banner--viva-mix .banner-slogan {
    color: #ffffff;
    font-size: 0;
    width: 90vw;
    max-width: 305px;
    height: 96px;
    overflow: hidden;
    text-indent: -199%;
    background: url(//cdn.gogoro.com/resources/images/landing-page/viva-mix/hb-viva-mix-slogan.svg) center/contain no-repeat;
}
:lang(en) .banner--viva-mix .banner-slogan {
    height: 70px;
    background-image: url(//cdn.gogoro.com/resources/images/landing-page/viva-mix/hb-viva-mix-slogan-en.svg);
}
.banner-actions {
    display: flex;
    justify-content: center;
}
.banner-cta {
    display: flex;
    align-items: center;
    font-size: 15px;
    letter-spacing: 0.15em;
    padding: 0 1.66em 0 1.8em;
    height: 40px;
    border-radius: 20px;
    cursor: pointer;
    font-weight: 500;
    background-color: transparent;
    transition: color .25s, background-color .25s;
}
.banner--viva-mix .banner-cta {
    margin-top: 16px;
    color: #ffffff;
    border: 2px solid #ffffff;
}
.banner--viva-mix .banner-cta:lang(en) {
    font-weight: 700;
    text-transform: uppercase;
    font-family: var(--font-family-italic);
}
.gs-hero {
    display: block;
    background: center/cover no-repeat url(//cdn.gogoro.com/resources/pages/landing-page/gs0528/web_global_video_still_image.jpg);
}
.gs-video {
    opacity: 0;
    display: block;
    width: 100%;
    height: 100%;
    position: absolute;
    -o-object-fit: cover;
    object-fit: cover;
    left: 0;
    top: 0;
}
.slick-dots {
    position: absolute;
    bottom: -25px;
    list-style: none;
    display: block;
    text-align: center;
    padding: 0;
    margin: 0;
    width: 100%;
}
.slick-dots.slick-dots {
    bottom: 8px;
    left: 0;
}
.slick-dots li {
    position: relative;
    display: inline-block;
    height: 20px;
    width: 20px;
    margin: 0 5px;
    padding: 0;
    cursor: pointer;
}
.slick-dots li button {
    border: 0;
    background: transparent;
    display: block;
    height: 20px;
    width: 20px;
    outline: none;
    line-height: 0px;
    font-size: 0px;
    color: transparent;
    padding: 5px;
    cursor: pointer;
}
.slick-dots li button:before {
    position: absolute;
    top: 0;
    left: 0;
    content: "•";
    width: 20px;
    height: 20px;
    font-family: "slick";
    font-size: 6px;
    line-height: 20px;
    text-align: center;
    color: black;
    opacity: 0.25;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
.slick-dots.slick-dots button:before {
    height: 8px;
    width: 8px;
    opacity: 1 !important;
    border-radius: 50%;
    border: 2px solid #737d82;
    background-color: #737d82;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
}
.slick-dots.slick-dots button::before {
    content: '';
}
.slick-dots li button:hover:before, .slick-dots li button:focus:before {
    opacity: 1;
}
.slick-dots li.slick-active button:before {
    color: black;
    opacity: 0.75;
}
.slick-dots.slick-dots .slick-active button:before {
    border: 2px solid #fff;
    background-color: rgba(115,125,130,0);
}
.slick-dots.slick-dots button:before {
    height: 8px;
    width: 8px;
    opacity: 1 !important;
    border-radius: 50%;
    border: 2px solid #737d82;
    background-color: #737d82;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
}
.social-post-item,
.social-post-copy-wrapper,
.social-post-bg {
  position: absolute;
  left: 0;
  width: 100%;
  top: 0;
  height: 100%;
}
.slick-initialized .slick-slide {
  display: block;
}
.social-post-item,
.social-post-copy-wrapper,
.social-post-bg {
  position: absolute;
  left: 0;
  width: 100%;
  top: 0;
  height: 100%;
}
.social-post-copy-wrapper {
  z-index: 2;
  display: flex;
  box-align: center;
  -moz-align-items: center;
  -ms-align-items: center;
  -o-align-items: center;
  align-items: center;
  -ms-flex-align: center;
  box-pack: center;
  -moz-justify-content: center;
  -ms-justify-content: center;
  -o-justify-content: center;
  justify-content: center;
  -ms-flex-pack: center;
  text-align: center;
}
:lang(en) .social-post-copy-wrapper {
  background-color: rgba(0, 0, 0, 0.4);
}
.media-item-title,
.media-section-name {
  color: #fff;
  font-family: "graphik-b", "Noto Sans Black";
  line-height: 1.28;
}
.media-item-title {
  font-size: 27px;
}
.social-post-title {
  margin-bottom: 0;
}
:lang(en) .social-post-title {
  line-height: 1.1;
  font-family: var(--font-family-base);
  font-weight: 500;
}
.social-post-subtitle {
  color: #fff;
  font-family: "graphik-b", "PingFangTC-Semibold", "Noto Sans Bold";
  line-height: 1.5;
  font-size: 20px;
  position: absolute;
  bottom: 20px;
  left: 0;
  width: 100%;
}
.social-post-item,
.social-post-copy-wrapper,
.social-post-bg {
  position: absolute;
  left: 0;
  width: 100%;
  top: 0;
  height: 100%;
}
.social-post-bg {
  background-size: auto 100%;
  background-position: center;
  background-repeat: no-repeat;
}
:lang(en) .social-post-bg {
  background-size: cover;
}
.section-eeyo {
  overflow: hidden;
  font-family: var(--font-family-base);
  padding: 40px 0 16px 0;
  color: #000000;
  background-color: #f2f2f2;
}
.eeyo-content {
  padding: 0 32px;
  text-align: center;
}
.eeyo-title {
  line-height: 1.1;
  letter-spacing: -0.012em;
  font-family: inherit;
  font-size: 42px;
  font-weight: 500;
  margin: 0 0 20px 0;
}
.eeyo-desc {
  font-size: 16px;
  max-width: 464px;
  margin: auto;
}
.section-eeyo .gs-cta {
  margin: 36px 0 40px 0;
}
.gs-cta::after {
  content: "";
  display: block;
  width: 24px;
  height: 24px;
  margin: 0 0 0 7px;
  background: center/contain no-repeat url("~@/assets/icon-arrow.svg");
}
.image-eeyo {
  position: relative;
  transform: translateX(-50%);
  left: 50%;
  width: 500px;
}
.image-eeyo::before {
  content: "";
  display: block;
  padding-bottom: 60%;
  background: url("~@/assets/05_Profileshot_Right_Side.png") center/contain
    no-repeat;
}
.section-quotes {
  margin: 6px auto;
  padding: 1px 0 0 0;
  background-color: #fff;
}
.quote-logo-list,
.quote-text-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.slick-slider {
  position: relative;
  display: block;
  box-sizing: border-box;
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  touch-action: pan-y;
  -webkit-tap-highlight-color: transparent;
}
.quote-text-list {
  text-align: center;
  padding: 9rem 1rem 6rem 1rem;
}
.quote-text-list {
  padding: 6rem 1rem 3rem 1rem;
}
.quote-text-list .slick-track {
  display: flex;
  align-items: center;
}
.section-quotes blockquote {
  margin-bottom: 0;
}
.quote-text {
  color: #323237;
  font-family: "graphik-li";
}
.quote-text {
  font-size: 24px;
}
.quote-cite {
  font-style: normal;
  color: #b9bcbf;
}
.quote-cite {
  font-size: 18px;
}
.quote-cite::before {
  content: "- ";
}
.quote-logo-list {
  width: 100%;
  background-color: #e6e6e6;
}
.quote-logo-item {
  position: relative;
  cursor: pointer;
  padding: 0 10px;
}
.quote-logo {
  position: relative;
  width: 150px;
  height: 80px;
}
.quote-logo--wired::before {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_wired_off.jpg);
}
.quote-logo--wired::after {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_wired_on.jpg);
}
.quote-logo--time::before {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_time_off.jpg);
}
.quote-logo--time::after {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_time_on.jpg);
}
.quote-logo--cleantech::before {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_cleantech_off.jpg);
}
.quote-logo--cleantech::after {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_cleantech_on.jpg);
}
.quote-logo--verge::before {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_verge_off.jpg);
}
.quote-logo--verge::after {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_verge_on.jpg);
}
.quote-logo--nikkei::before {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_nikkei_off.jpg);
}
.quote-logo--nikkei::after {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_nikkei_on.jpg);
}
.quote-logo--sustania::before {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_sustania_off.jpg);
}
.quote-logo--sustania::after {
  background: url(//cdn.gogoro.com/resources/images/landing-page/quotes_logo_sustania_on.jpg);
}
.quote-logo::after {
  transition: opacity 0.3s;
  opacity: 0;
}
.quote-logo-item.slick-current::after {
  content: "";
  display: block;
  position: absolute;
  left: 50%;
  top: 0;
  margin-left: -10px;
  border-width: 15px 10px;
  border-color: #fff transparent transparent transparent;
  border-style: solid;
}
.quote-logo::before,
.quote-logo::after {
  content: "";
  display: block;
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-size: auto 90%;
  background-position: center;
  background-repeat: no-repeat;
}
.section-impact {
  margin: 6px auto;
  padding: 1px 0;
  background-color: #fff;
}
.container {
  margin-left: auto;
  margin-right: auto;
  padding-left: 1.5rem;
  padding-right: 1.5rem;
}
.impact-headline {
  font-family: "Graphik", "Noto Sans Black", sans-serif;
  line-height: 1.28;
  font-weight: 500;
  letter-spacing: -0.01em;
  font-size: 27px;
  text-align: center;
  margin-top: 1.5em;
  margin-bottom: 1em;
}
:lang(en) .impact-headline {
  font-family: var(--font-family-base);
  font-size: 28px;
  font-weight: 500;
  line-height: 1.21;
}
.row {
  margin-left: -1.5rem;
  margin-right: -1.5rem;
}
.col-xl-12,
.col-xl-11,
.col-xl-10,
.col-xl-9,
.col-xl-8,
.col-xl-7,
.col-xl-6,
.col-xl-5,
.col-xl-4,
.col-xl-3,
.col-xl-2,
.col-xl-1,
.col-lg-12,
.col-lg-11,
.col-lg-10,
.col-lg-9,
.col-lg-8,
.col-lg-7,
.col-lg-6,
.col-lg-5,
.col-lg-4,
.col-lg-3,
.col-lg-2,
.col-lg-1,
.col-md-12,
.col-md-11,
.col-md-10,
.col-md-9,
.col-md-8,
.col-md-7,
.col-md-6,
.col-md-5,
.col-md-4,
.col-md-3,
.col-md-2,
.col-md-1,
.col-sm-12,
.col-sm-11,
.col-sm-10,
.col-sm-9,
.col-sm-8,
.col-sm-7,
.col-sm-6,
.col-sm-5,
.col-sm-4,
.col-sm-3,
.col-sm-2,
.col-sm-1,
.col-xs-12,
.col-xs-11,
.col-xs-10,
.col-xs-9,
.col-xs-8,
.col-xs-7,
.col-xs-6,
.col-xs-5,
.col-xs-4,
.col-xs-3,
.col-xs-2,
.col-xs-1 {
  position: relative;
  min-height: 1px;
  padding-left: 1.5rem;
  padding-right: 1.5rem;
}
.impact-item-list {
  position: relative;
  height: 330px;
}
.impact-item {
  position: absolute;
  left: 0;
  width: 100%;
  top: 0;
  height: 100%;
  text-align: center;
}
.impact-animation {
  position: relative;
  width: 103px;
  height: 138px;
  margin: 0 auto 20px auto;
  transform: scale(0.5);
  transform-origin: left top;
}
.impact-animation {
  opacity: 0;
  transition: all 0.5s;
}
.inview .impact-item.active .impact-animation {
  opacity: 1;
  transition: all 0.5s 0.5s;
}
.impact-co2-cloud {
  width: 144px;
  height: 93px;
  position: absolute;
  left: 30px;
  top: 11px;
  background: url("~@/assets/impact-co2-cloud-fad788e12ddf2d3d9c00ffd0998748d275a6c8062aac8adbde4954402c94bc50.svg")
    center/144px 83px no-repeat;
}
.impact-badge {
  box-flex: 1;
  -moz-flex: 1;
  flex: 1;
}
.impact-badge {
  opacity: 0;
  transform: translateY(10px);
  transition: all 0.5s;
}
.impact-item.active .impact-badge {
  opacity: 1;
  transform: translateY(0px);
  transition: all 0.5s 0.5s;
}
.impact-value {
  position: relative;
  line-height: 1;
  font-family: "flamasc-ul";
  font-size: 54px;
}
.impact-unit {
  position: absolute;
  top: 11px;
  font-size: 24px;
  font-family: "flamasc-book";
  margin-left: 3px;
}
.impact-caption {
  font-size: 20px;
  margin: 0.5em 0;
  font-family: "graphik-semib", "PingFangTC-Semibold", "Noto Sans Bold";
}
.impact-desc {
  font-size: 16px;
}
.impact-dots {
  text-align: center;
  padding: 20px 0 30px 0;
}
.impact-dot {
  padding: 10px;
  display: inline-block;
  cursor: pointer;
}
.impact-dot:before {
  content: "";
  display: block;
  width: 12px;
  height: 12px;
  border-radius: 6px;
  border: 2px solid #f1f3f3;
  background-color: #f1f3f3;
  transition: all 0.3s;
}
.impact-dot.active:before {
  border: 2px solid #00d7ff;
  background-color: #fff;
}
.row::after {
  content: "";
  display: table;
  clear: both;
}
.container::after {
  content: "";
  display: table;
  clear: both;
}
@media (min-width: 375px){
.slick-dots.slick-dots {
    bottom: 10px;
}
}
@include media-breakpoint-up(sm) {
  .banner-container {
    height: calc(100vh - 120px);
    min-height: 560px;
    max-height: 1140px;
  }
  :lang(en) .banner--viva-mix .banner-content-layer {
    top: 76%;
  }
  .banner-title {
    font-size: 42px;
}
.banner-slogan {
    font-size: 19px;
}
.banner-cta {
    height: 48px;
    border-radius: 24px;
    padding: 0 1.86em 0 2em;
}
.slick-dots.slick-dots {
    bottom: 20px;
}
  .section-station {
    background-image: linear-gradient(40deg, #40fdcb, #40fdcb 7%, #24ee2c);
  }
  .media-item-title {
    font-size: 32px;
  }
  .section-eeyo {
    padding: 60px 0 0 0;
  }
  .d-sm-none {
    display: none;
  }
  .image-eeyo {
    width: 700px;
  }
  .quote-text {
    font-size: 32px;
  }
  .container {
    max-width: 576px;
  }
}
@include media-breakpoint-up(md) {
  .banner-container {
    height: calc(100vh - 120px);
    min-height: 680px;
    max-height: 1200px;
  }
  .banner-content-layer {
    bottom: 80px;
  }
  .banner--viva-mix .banner-content-layer {
    top: 69%;
  }
  :lang(en) .banner--viva-mix .banner-content-layer {
    top: 66%;
  }
  .banner--viva-mix {
    background: url(//cdn.gogoro.com/resources/images/landing-page/viva-mix/hb-viva-mix-scooter.png?v1) center/contain no-repeat, url(//cdn.gogoro.com/resources/images/landing-page/viva-mix/hb-viva-mix-bg.png?v1) center/cover no-repeat;
}
  .campaign-list {
    margin: 0 -3px;
  }
  .campaign {
    padding-bottom: 100%;
  }
  .campaign-copy-wrapper {
    height: 25%;
  }
  .section-station {
    background-image: linear-gradient(60deg, #40fdcb, #40fdcb 7%, #24ee2c);
  }
  :lang(en) .section-station {
    color: #000000;
    font-family: var(--font-family-base);
    padding: 40px 0 0 0;
  }
  :lang(en) .section-station {
    padding: 0;
  }
  :lang(en) .station-content-container {
    text-align: left;
    padding: 0 60px;
  }
  .station-content-container {
    text-align: left;
    padding: 0 90px;
    position: absolute;
    top: 50%;
    height: 70%;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  :lang(en) .station-brand {
    margin: 0 0 46px 0;
  }
  :lang(en) .station-caption {
    font-size: 32px;
    margin: 0 0 20px 0;
    max-width: 9em;
  }
  :lang(en) .station-desc {
    margin: 0 0 32px 0;
  }
  :lang(en) .section-station .gs-cta {
    margin: 0;
  }
  .image-station {
    width: 70%;
    max-width: 100%;
    float: right;
    transform: translateX(20%);
  }
  .image-station::before {
    background-image: url("~@/assets/station-gn@2x.png");
  }
  .media-container-wrapper {
    margin: 0 -3px;
  }
  .media-container {
    float: left;
    border: 3px solid #f8f8f8;
    border-width: 0 3px 0 3px;
  }
  .blog-posts-container {
    width: 66.66%;
  }
  .social-media-container {
    width: 33.33%;
  }
  :lang(en) .blog-posts-container,
  :lang(en) .social-media-container {
    width: 50%;
  }
  .blog-post-list {
    padding-bottom: 50%;
  }
  :lang(en) .social-post-list,
  :lang(en) .blog-post-list {
    padding-bottom: 0;
    height: 340px;
  }
  .image-eeyo {
    width: 900px;
    margin: 0 0 -132px 0;
  }
  .quote-text-list {
    padding: 8rem 1rem 5rem 1rem;
  }
  .quote-text {
    font-size: 36px;
  }
  .container {
    max-width: 720px;
  }
  .impact-headline {
    font-size: 41px;
  }
  :lang(en) .impact-headline {
    font-size: 32px;
  }
  .impact-item-list {
    height: 278px;
  }
  .impact-item {
    display: flex;
    box-align: center;
    -moz-align-items: center;
    -ms-align-items: center;
    -o-align-items: center;
    align-items: center;
    -ms-flex-align: center;
    text-align: left;
  }
  .impact-animation {
    width: 206px;
    height: 278px;
    transform: scale(1);
    transform-origin: center;
    margin: 0 70px 0 0;
  }
  .impact-desc {
    font-size: 20px;
  }
}
@include media-breakpoint-up(lg) {
  :lang(en) .banner--viva-mix .banner-content-layer {
    top: 70%;
  }
  .slick-dots.slick-dots button:before {
    height: 12px;
    width: 12px;
}
  .campaign-list {
    margin: 0 -3px;
  }
  .campaign-item:first-child:nth-last-child(3),
  .campaign-item:first-child:nth-last-child(3) ~ .campaign-item {
    width: 33.33%;
  }
  .campaign-item {
    float: left;
    border: 3px solid #f8f8f8;
    border-width: 0 3px 0 3px;
  }
  :lang(en) .station-caption {
    font-size: 42px;
  }
  .image-station {
    transform: none;
    width: 688px;
  }
  .media-section-name {
    font-size: 32px;
  }
  .media-item-title {
    font-size: 42px;
  }
  .quote-logo-list .slick-track {
    width: auto !important;
    transform: none !important;
    text-align: center;
  }
  .quote-logo-item {
    display: inline-block !important;
    vertical-align: middle;
    float: none !important;
  }
  .container {
    max-width: 940px;
  }
  :lang(en) .impact-headline {
    font-size: 42px;
  }
  .col-lg-12,
  .col-lg-11,
  .col-lg-10,
  .col-lg-9,
  .col-lg-8,
  .col-lg-7,
  .col-lg-6,
  .col-lg-5,
  .col-lg-4,
  .col-lg-3,
  .col-lg-2,
  .col-lg-1 {
    float: left;
  }
  .col-lg-8 {
    width: 66.6666666667%;
  }
  .col-lg-offset-2 {
    margin-left: 16.6666666667%;
  }
  .impact-value {
    letter-spacing: -2px;
    font-size: 72px;
  }
  .impact-unit {
    margin-left: 5px;
    top: 16px;
  }
}
@include media-breakpoint-up(xl) {
  .banner-container {
    height: calc(100vh - 200px);
    max-height: 1640px;
    min-height: 820px;
  }
  :lang(en) .banner--viva-mix .banner-content-layer {
    top: 74%;
  }
  .banner--viva-mix .banner-slogan {
    max-width: 402px;
    height: 126px;
}
  :lang(en) .station-content-container {
    padding: 0 100px;
  }
  .image-station {
    width: 688px;
  }
  .container {
    max-width: 1140px;
  }
}
</style>
