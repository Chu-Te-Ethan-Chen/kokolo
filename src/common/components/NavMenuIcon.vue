<template lang="pug">
label.nav-menuicon(for='nav-menustate' :class='{\'nav-menuicon--open\' : isActive}' @click='isActive = !isActive')
  span.nav-menuicon-bread.nav-menuicon-bread--top
    span.nav-menuicon-crust.nav-menuicon-crust--top
  span.nav-menuicon-bread.nav-menuicon-bread--middle
    span.nav-menuicon-crust.nav-menuicon-crust--middle
  span.nav-menuicon-bread.nav-menuicon-bread--bottom
    span.nav-menuicon-crust.nav-menuicon-crust--bottom
</template>
<script>
export default {
  name: "NavMenuIcon",
  data() {
    return   {
      isActive: false,
    };
  },
};
</script>
<style lang="scss" scoped>
.nav-menuicon {
  position: absolute;
  width: 50px;
  height: 50px;
  left: 0;
  top: 0;
}
.nav-menuicon-crust--top {
  top: 19px;
}
.nav-menuicon-crust--middle {
  top: 24px;
}
.nav-menuicon-crust--bottom {
  top: 29px;
}
.nav-menuicon--open .nav-menuicon-crust--top {
  top: 24px;
  -webkit-transform: rotate(135deg);
  transform: rotate(135deg);
}
.nav-menuicon--open .nav-menuicon-crust--middle {
  top: 29px;
  opacity: 0;
}
.nav-menuicon--open .nav-menuicon-crust--bottom {
  top: 24px;
  -webkit-transform: rotate(-135deg);
  transform: rotate(-135deg);
}
.nav-menuicon-crust {
  -webkit-transition: all 0.6s cubic-bezier(0.6, 0, 0, 1);
  transition: all 0.6s cubic-bezier(0.6, 0, 0, 1);
  position: absolute;
  width: 20px;
  height: 2px;
  border-radius: 2px;
  left: 15px;
  background-color: #737d82;
}
</style>
