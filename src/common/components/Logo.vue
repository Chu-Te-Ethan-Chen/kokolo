<template>
  <a href="/" class="nav-logo nav-logo--dark">Gogoro</a>
</template>

<script>
export default {
  name: "Logo",
};
</script>

<style lang="scss" scoped>
.nav-logo {
  overflow: hidden;
  text-indent: 101%;
  white-space: nowrap;
  display: block;
  width: 100px;
  height: 100%;
  background-size: 78px 22px;
  background-repeat: no-repeat;
  background-position: 50%;
  background-clip: content-box;
  background-origin: content-box;
}
.nav-logo--dark {
  background-image: url("~@/assets/logo.svg");
}
@include media-breakpoint-up(lg) {
  .nav-logo {
    width: 100%;
    background-size: auto 27px;
    background-position: 0;
    background-position: 0 calc(50% + 1px);
  }
}
</style>
