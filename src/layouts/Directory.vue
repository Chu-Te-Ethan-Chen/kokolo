<template>
<div class="kkl-directory">
  <div class="container">
    <div class="row dt-layout">
      <div class="col-md-3 col-sm-6 dt-socials">
        <!--Column1-->
        <div class="footer-pad">
          <div>kokolo</div>
          <div class="dt-social-links">
              <a href="#" target="_blank" class="dt-social-link"><i class="dt-icon dt-icon--facebook"></i>Facebook</a>
              <a href="#" target="_blank" class="dt-social-link"><i class="dt-icon dt-icon--youtube"></i>Youtube</a>
              <a href="#" target="_blank" class="dt-social-link"><i class="dt-icon dt-icon--twitter"></i>Twitter</a>
              <a href="#" target="_blank" class="dt-social-link"><i class="dt-icon dt-icon--instagram"></i>Instagram</a>
              <a href="#" target="_blank" class="dt-social-link"><i class="dt-icon dt-icon--linkedin"></i>Linkedin</a>
          </div>
        </div>
      </div>
      <div class="col-md-3 col-sm-6">
        <!--Column1-->
        <div class="footer-pad">
          <div class="dt-section-name">Smartscooter</div>
          <ul class="list-unstyled">
            <li><a class="dt-section-link" href="#">S Performance</a></li>
            <li><a class="dt-section-link" href="#">Gogoro 1 Series</a></li>
            <li><a class="dt-section-link" href="#">Gogoro 1 Series</a></li>
            <li><a class="dt-section-link" href="#">Gogoro 1 Series</a></li>
            <li><a class="dt-section-link" href="#">Gogoro VIVA</a></li>
            <li><a class="dt-section-link" href="#">Gogoro VIVA MIX</a></li>
            <li><a class="dt-section-link" href="#">iQ System®</a></li>
            <li><a class="dt-section-link" href="#">Compare Specs</a></li>
          </ul>
        </div>
      </div>
      <div class="col-md-3 col-sm-6">
        <!--Column1-->
        <div class="footer-pad">
          <div class="dt-section-name">Smart Power</div>
          <ul class="list-unstyled">
            <li><a class="dt-section-link" href="#">Gogoro Network®</a></li>
          </ul>
        </div>
      </div>
      <div class="col-md-3 col-sm-6">
        <!--Column1-->
        <div class="footer-pad">
          <div class="dt-section-name">News</div>
          <ul class="list-unstyled">
            <li><a class="dt-section-link" href="#">Latest</a></li>
            <li><a class="dt-section-link" href="#">About Us</a></li>
            <li><a class="dt-section-link" href="#">Media Center</a></li>
            <li><a class="dt-section-link" href="#">Media Assets</a></li>
            <li><a class="dt-section-link" href="#">Inquires</a></li>
            <li>
              <a class="dt-section-link" href="#"></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
  export default {
    name: 'DefaultDirectory',
  }
</script>

<style lang="scss" scoped>
.kkl-directory{
    background-color: #323237;
}
.dt-layout {
    padding: 60px 0;
    border-bottom: 1px solid hsla(0,0%,100%,.08);
}
.dt-section-name {
    position: relative;
    cursor: pointer;
    color: #737d82;
}
.dt-section-link {
    display: block;
    font-size: 14px;
    line-height: 1.4;
    color: #f6f6f6;
    text-decoration: none;
}
.dt-social-links {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    -ms-flex-flow: row wrap;
    flex-flow: row wrap;
    max-width: 380px;
    margin: 40px 0 0;
}
.dt-social-link {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    color: #b9bcbf;
    line-height: 1.14;
    font-size: 14px;
    text-decoration: none;
    -webkit-box-flex: 0;
    -ms-flex: 0 0 50%;
    flex: 0 0 50%;
    margin: 0 0 20px;
}
</style>