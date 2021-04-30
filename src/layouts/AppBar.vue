<template>
  <nav class="ggr-nav ggr-nav--dark ggr-nav--scrolling-bg">
    <div
      ref="mainNavbar"
      class="ggr-nav-container"
      :style="{'background-color': `rgba(18, 18, 21, ${mainNavbarOpacity})`}"
    >
      <div class="ggr-header-container"></div>
      <div class="ggr-nav-list-container d-lg-none">
        <div class="gc-container">
          <ul class="ggr-nav-list">
            <li class="ggr-nav-item ggr-nav-item--logo gc-desktop-visible">
              <logo />
            </li>
            <li class="ggr-nav-item">
              <a href="/smartscooter/" class="ggr-nav-link nav-list__link--dark">
                <span>Smartscooter®</span>
              </a>
            </li>
            <li class="ggr-nav-item">
              <a href="/gogoro-network/" class="ggr-nav-link nav-list__link--dark">
                <span>Gogoro Network®</span>
              </a>
            </li>
            <li class="ggr-nav-item">
              <a href="/news/" class="ggr-nav-link nav-list__link--dark">
                <span>News</span>
              </a>
            </li>
            <li class="ggr-nav-item ggr-nav-item--divider gc-desktop-visible"></li>
          </ul>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
import Logo from '@/common/components/Logo'
export default {
  name: "DefaultBar",
  data(){
    return {
      isMounted: false,
      mainNavbarOpacity: 0
    }
  },
  components: {
    Logo,
  },
  created () {
    window.addEventListener('scroll', this.handlescroll);
  },
  mounted(){
    this.isMounted = true;
  },
  unmounted () {
    window.removeEventListener('scroll', this.handlescroll);
  },
  methods: {
    handlescroll () {
      // Any code to be executed when the window is scrolled
        if(!this.isMounted) return;
        const mainNavbar = this.$refs.mainNavbar
        const height = mainNavbar.clientHeight
        let scroll = document.documentElement.scrollTop || document.body.scrollTop;
        const ratio = scroll / parseInt(height)
        this.mainNavbarOpacity = ratio <= 1 ? ratio : 1
        return
    }
  }
}
</script>

<style lang="scss" scoped>
.ggr-nav {
  position: relative;
}
.ggr-nav {
    font-family: $--font-family-base;
    font-weight: 400;
    -webkit-font-smoothing: antialiased;
}
.ggr-nav {
    z-index: 3000;
}
.ggr-nav-container {
    top: 0;
    left: 0;
    position: fixed;
    width: 100%;
    height: 50px;
    -webkit-transition: backgroundColor .3s;
    transition: backgroundColor .3s;
}
.ggr-nav-list-container {
    background-color: $--nav-list-bg-color;
}
.ggr-nav-list-container {
    position: fixed;
    left: 0;
    width: 100%;
    top: 50px;
    height: calc(100vh - 50px);
    overflow: auto;
    -webkit-transform: translateZ(0);
    transform: translateZ(0);
}
.gc-container {
    margin-left: auto;
    margin-right: auto;
    padding-left: 15px;
    padding-right: 15px;
}
.ggr-nav-list {
    padding-bottom: 100px;
}
.ggr-nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
}
.ggr-nav-item--logo {
    width: 105px;
    height: 100%;
}

.ggr-nav-item {
    -webkit-transition: background-color .3s;
    transition: background-color .3s;
    display: block;
}
.ggr-nav-link {
    display: block;
    padding: 20px;
    text-decoration: none;
    text-align: center;
    -webkit-transition: color .3s;
    transition: color .3s;
    cursor: pointer;
    white-space: nowrap;
}
.nav-list__link--dark, .nav-list__link--dark:focus, .nav-list__link--dark:visited {
    color: #fff;
}
@include media-breakpoint-up(sm){
  .ggr-nav-list-container {
      background-color: $--nav-sm-list-bg-color;
  }
  .ggr-nav-list-container {
    height: auto;
    overflow: visible;
    position: absolute;
  }
  .gc-container {
    max-width: 576px;
  }
  .ggr-nav-list {
    padding-bottom: 0;
  }
  .ggr-nav-link[data-v-088e2fe8] {
    font-size: 13px;
    height: 54px;
    line-height: 54px;
    padding: 0 10px;
  }
}
@include media-breakpoint-up(md){
  .gc-container {
    max-width: 720px;
  }
  .ggr-nav-link {
    font-size: 14px;
    padding: 0 14px;
    height: 60px;
    line-height: 60px;
  }
  .ggr-nav-item:last-child {
    margin-right: -10px;
  }
}
@include media-breakpoint-up(lg){
  .ggr-nav--dark .ggr-nav-container{
      background-color: #fff;
  }
  .ggr-nav-container {
      height: 60px;
      &:hover{
        background: rgb(18, 18, 21) !important;
      }
  }
  .ggr-nav--scrolling-bg .ggr-nav-list-container, .ggr-nav-list-container .ggr-nav-list {
      background-color: transparent;
  }
  .ggr-nav-list-container {
    top: 0;
    display: block!important;
  }
  .gc-container {
    max-width: 940px;
  }
  .ggr-nav-list {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    height: 60px;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
  }
  .ggr-nav-item--logo {
    margin-right: 16px;
  }
  .ggr-nav-link {
    font-size: 14px;
    padding: 0 12px;
  }
  .ggr-nav-item--divider {
    margin-left: auto!important;
  }
}
</style>