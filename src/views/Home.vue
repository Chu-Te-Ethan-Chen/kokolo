<template>
  <div class="section-hero">
    <div class="banner-container">
      <div
        id="carouselExampleIndicators"
        class="carousel slide baner-list"
        data-bs-ride="carousel"
      >
        <div class="carousel-indicators">
          <button
            type="button"
            data-bs-target="#carouselExampleIndicators"
            data-bs-slide-to="0"
            class="active"
            aria-current="true"
            aria-label="Slide 1"
          ></button>
          <button
            type="button"
            data-bs-target="#carouselExampleIndicators"
            data-bs-slide-to="1"
            aria-label="Slide 2"
          ></button>
        </div>
        <div class="carousel-inner">
          <div class="carousel-item active" style="background-color: #F77E36;">
            <!-- <img src="https://source.unsplash.com/XghsTOU2W24" class="d-block w-100" alt="..."> -->
          </div>
          <div class="carousel-item" style="background-color: aquamarine;">
            <span class="gs-content-layer">
              <span class="gs-content">
                <h1 class="gs-title">
                  A Better Way Forward to
                  <span class="d-inline-block">Smarter, Cleaner Cities</span>
                </h1>
                <span class="gs-desc"
                  >Gogoro is reinventing urban transportation with an ecosystem
                  of sustainable energy solutions for the world’s modern
                  cities.</span
                >
              </span>
            </span>
            <!-- <img src="https://source.unsplash.com/Nh6NsnqYVsI" class="d-block w-100" alt="..."> -->
          </div>
        </div>
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
  <section
    class="landing-page-section section-impact"
    style="height: 525px; background-color: lightgreen;"
  ></section>
</template>

<script>
export default {
  name: "Home",
};
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
.banner-list,
.slick-list,
.slick-track {
  height: 100% !important;
}
.slick-slider .slick-track,
.slick-slider .slick-list {
  transform: translate3d(0, 0, 0);
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
@include media-breakpoint-up(sm) {
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
}
@include media-breakpoint-up(md) {
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
}
@include media-breakpoint-up(lg) {
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
}
@include media-breakpoint-up(xl) {
  :lang(en) .station-content-container {
    padding: 0 100px;
  }
  .image-station {
    width: 688px;
  }
}
</style>
