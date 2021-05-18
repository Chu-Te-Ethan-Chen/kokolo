<template lang='pug'>
label.close-nested-menu(for='close-menu-toggle' style='display: none')
nav.ggr-nav.ggr-nav--dark.ggr-nav--scrolling-bg
  input#nav-menustate.nav-menustate.gc-hide(type='checkbox')
  .ggr-nav-container(ref='mainNavbar' style='transform: translateY(0px)' :style='{ \'background-color\': `rgba(18, 18, 21, ${mainNavbarOpacity})` }')
    .ggr-header-container
      .gc-container
        ul.ggr-header
          li.ggr-header-item.menuicon-item
            nav-menu-icon(@click='activateGGRNavNoscroll')
          li.ggr-header-item.logo-item
            logo.
          li.ggr-header-item.my-gogoro-item
            nav-login.        
    transition(name='nav-list')
      .ggr-nav-list-container(v-show='isActive')
        .gc-container
          ul.ggr-nav-list
            li.ggr-nav-item.ggr-nav-item--logo.gc-desktop-visible
              logo.       
            li.ggr-nav-item
              a.ggr-nav-link.nav-list__link--dark(href='/smartscooter/')
                span Smartscooter®
            li.ggr-nav-item
              a.ggr-nav-link.nav-list__link--dark(href='/gogoro-network/')
                span Gogoro Network®
            li.ggr-nav-item
              a.ggr-nav-link.nav-list__link--dark(href='/news/')
                span News
            li.ggr-nav-item.ggr-nav-item--divider.gc-desktop-visible
</template>

<script>
import Logo from "@/common/components/Logo";
import NavMenuIcon from "@/common/components/NavMenuIcon";
import NavLogin from "@/common/components/NavLogin";

export default {
  name: "DefaultBar",
  data() {
    return {
      isMounted: false,
      mainNavbarOpacity: 0,
      isActive: false,
    };
  },
  components: {
    Logo,
    NavMenuIcon,
    NavLogin,
  },
  created() {
    window.addEventListener("scroll", this.handlescroll);
  },
  mounted() {
    this.isMounted = true;
  },
  unmounted() {
    window.removeEventListener("scroll", this.handlescroll);
  },
  methods: {
    handlescroll() {
      // Any code to be executed when the window is scrolled
      if (!this.isMounted) return;
      const mainNavbar = this.$refs.mainNavbar;
      const height = mainNavbar.clientHeight;
      let scroll =
        document.documentElement.scrollTop || document.body.scrollTop;
      const ratio = scroll / parseInt(height);
      this.mainNavbarOpacity = ratio <= 1 ? ratio : 1;
      return;
    },
    activateGGRNavNoscroll(){
      this.isActive = !this.isActive;
      if (this.isActive) {
        const dom = window.document
        const htmlNode = dom.getElementsByTagName('html')
        htmlNode[0].classList.add('ggr-nav-noscroll')
      } else {
        const dom = window.document
        const htmlNode = dom.getElementsByTagName('html')
        htmlNode[0].classList.remove('ggr-nav-noscroll')
      }
    }
  },
};
</script>

<style lang="scss" scoped>
.close-nested-menu {
    position: fixed;
    left: 0;
    width: 100%;
    top: 0;
    height: 100%;
}
.ggr-nav {
  position: relative;
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
    background-color: var(--nav-list-bg-color);
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
.ggr-header-container .gc-container {
    max-width: 100%;
    padding: 0;
}
.ggr-header {
    position: relative;
    z-index: 1;
    height: 50px;
}
.ggr-header {
    background-color: var(--nav-header-bg-color);
}
.ggr-header-item {
    position: absolute;
    top: 0;
    height: 100%;
}
.logo-item {
    left: 50%;
    -webkit-transform: translate(-50%);
    transform: translate(-50%);
}
.my-gogoro-item {
    right: 0;
}
.ggr-nav-list {
    padding-bottom: 100px;
}
.ggr-nav-list:before {
    content: "";
    display: block;
    position: absolute;
    left: 0;
    top: 0;
    right: 0;
    bottom: 0;
    z-index: -1;
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
ol, ul, dl {
    margin-top: 0;
    margin-bottom: 0;
}
ol, ul {
    padding-left: 0;
}
@include media-breakpoint-down(sm){
  .nav-list-enter-active{
    -webkit-transition:max-height .5s ease-in;
    transition:max-height .5s ease-in
  }
  .nav-list-leave-active{
    -webkit-transition:max-height .5s;
    transition:max-height .5s
  }
  .nav-list-enter,.nav-list-leave-to{
    max-height:0
  }
  .nav-list-enter-to,.nav-list-leave{
    overflow:hidden;
    max-height:calc(100vh - 50px)
  }
  .nav-list__link--dark,.nav-list__link--dark:focus,.nav-list__link--dark:hover,.nav-list__link--dark:visited,.nav-list__link--light,.nav-list__link--light:focus,.nav-list__link--light:hover,.nav-list__link--light:visited{
      color:#fff
  }
}
@include media-breakpoint-up(sm){
  .ggr-nav-list-container {
      background-color: var(--nav-sm-list-bg-color);
  }
  .ggr-nav-list-container {
    height: auto;
    overflow: visible;
    position: absolute;
  }
  .ggr-nav-list {
    padding-bottom: 0;
  }
  .ggr-nav-link {
    font-size: 13px;
    height: 54px;
    line-height: 54px;
    padding: 0 10px;
  }
}
@include media-breakpoint-up(md){
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
@include media-breakpoint-between(sm, lg) {
  .ggr-nav-list{
    bottom: auto;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: center;
    -ms-flex-pack: center;
    justify-content: center;
    pointer-events: none;
    z-index: -1;
    opacity: 0;
    -webkit-transform: translateY(-30px);
    transform: translateY(-30px);
    -webkit-transition: opacity .3s,-webkit-transform .6s;
    transition: opacity .3s,-webkit-transform .6s;
    transition: opacity .3s,transform .6s;
    transition: opacity .3s,transform .6s,-webkit-transform .6s;
  }
  #nav-menustate:checked~.ggr-nav-container .ggr-nav-list {
    pointer-events: auto;
    -webkit-transform: none;
    transform: none;
    opacity: 1;
  }
  .nav-list__link--dark:active,.nav-list__link--dark:focus,.nav-list__link--dark:hover,.nav-list__link--light:active,.nav-list__link--light:focus,.nav-list__link--light:hover{
      color:#00d7ff
  }
  .nav-list__link--dark:active .ggr-nav-link-text,.nav-list__link--dark:focus .ggr-nav-link-text,.nav-list__link--dark:hover .ggr-nav-link-text,.nav-list__link--light:active .ggr-nav-link-text,.nav-list__link--light:focus .ggr-nav-link-text,.nav-list__link--light:hover .ggr-nav-link-text{
      border-color:#00d7ff
  }
  .ggr-nav-item--active .nav-list__link--dark,.ggr-nav-item--active .nav-list__link--light{
      color:#00d7ff
  }
  .ggr-nav-item--active .nav-list__link--dark .ggr-nav-link-text,.ggr-nav-item--active .nav-list__link--light .ggr-nav-link-text{
      border-color:#00d7ff
  }
}
@include media-breakpoint-between(md, xl) {
  .nav-list-enter-active,.nav-list-leave-active{
    -webkit-transition:opacity .3s,-webkit-transform .5s;
    transition:opacity .3s,-webkit-transform .5s;
    transition:transform .5s,opacity .3s;
    transition:transform .5s,opacity .3s,-webkit-transform .5s
  }
  .nav-list-enter,.nav-list-leave-to{
    opacity:0;-webkit-transform:translateY(-50px);
    transform:translateY(-50px)
  }
}
@include media-breakpoint-down(lg) { 
  .gc-desktop-visible {
    display: none;
  }
 }
@include media-breakpoint-up(lg){
  .ggr-nav--dark .ggr-nav-container, .ggr-nav--light.ggr-nav--nested-menu-opened .ggr-nav-list:before, .ggr-nav--light .ggr-nav-container, .ggr-nav--light:hover .ggr-nav-list:before {
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
  .ggr-header-container .gc-container {
    display: none;
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
  .ggr-nav-item--active .nav-list__link--dark,.ggr-nav-item--active .nav-list__link--light,.nav-list__link--dark:active,.nav-list__link--dark:hover,.nav-list__link--light:active,.nav-list__link--light:hover{
      color:#00d7ff
  }
}
</style>