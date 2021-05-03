<template lang="pug">
a.nav-list__link.nav-list__link--login.nav-list__link--dark(href='//my.gogoro.com?lang=en-US') Login
</template>

<script>
export default {
  name: "NavLogin",
};
</script>

<style lang="scss" scoped>
.nav-list__link--login{
    display: block;
    width: 50px;
    height: 50px;
    overflow: hidden;
    text-indent: 101%;
    white-space: nowrap;
    background: url("~@/assets/login.svg") 50%/24px 24px no-repeat;
}
</style>