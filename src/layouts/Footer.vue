<template lang='pug'>
footer.ggr-footer
  .gc-container.gc-clear
    .locale
      select.locale-select
        option(disabled value) Region
        option(value='en-US') Global
        option(value='zh-TW') Taiwan
    .legal
      .legal-copyright.
        
        Copyright © 2014-2021 Gogoro Inc. All rights reserved.
        
      .legal-links
        a.legal-link(href='/privacy-policy/').
          
          Privacy Policy 
        a.legal-link(href='/terms-of-use/').
          
          Terms of Use
          
</template>

<script>
export default {
  name: "DefaultFooter",
};
</script>

<style lang="scss" scoped>
.ggr-footer {
    position: relative;
    font-size: 12px;
    padding: 30px 0;
    background-color: #323237;
}
.locale {
    text-align: center;
    margin-bottom: 30px;
}
.locale-select {
    padding-right: 15px;
    background: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pgo8c3ZnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHZlcnNpb249IjEuMSIgaWQ9IkNhcGFfMSIgeD0iMHB4IiB5PSIwcHgiIHdpZHRoPSI1MTJweCIgaGVpZ2h0PSI1MTJweCIgdmlld0JveD0iMCAwIDQ0NC44MTkgNDQ0LjgxOSIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgNDQ0LjgxOSA0NDQuODE5OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+CjxnPgoJPHBhdGggZD0iTTQzNC4yNTIsMTE0LjIwM2wtMjEuNDA5LTIxLjQxNmMtNy40MTktNy4wNC0xNi4wODQtMTAuNTYxLTI1Ljk3NS0xMC41NjFjLTEwLjA5NSwwLTE4LjY1NywzLjUyMS0yNS43LDEwLjU2MSAgIEwyMjIuNDEsMjMxLjU0OUw4My42NTMsOTIuNzkxYy03LjA0Mi03LjA0LTE1LjYwNi0xMC41NjEtMjUuNjk3LTEwLjU2MWMtOS44OTYsMC0xOC41NTksMy41MjEtMjUuOTc5LDEwLjU2MWwtMjEuMTI4LDIxLjQxNiAgIEMzLjYxNSwxMjEuNDM2LDAsMTMwLjA5OSwwLDE0MC4xODhjMCwxMC4yNzcsMy42MTksMTguODQyLDEwLjg0OCwyNS42OTNsMTg1Ljg2NCwxODUuODY1YzYuODU1LDcuMjMsMTUuNDE2LDEwLjg0OCwyNS42OTcsMTAuODQ4ICAgYzEwLjA4OCwwLDE4Ljc1LTMuNjE3LDI1Ljk3Ny0xMC44NDhsMTg1Ljg2NS0xODUuODY1YzcuMDQzLTcuMDQ0LDEwLjU2Ny0xNS42MDgsMTAuNTY3LTI1LjY5MyAgIEM0NDQuODE5LDEzMC4yODcsNDQxLjI5NSwxMjEuNjI5LDQzNC4yNTIsMTE0LjIwM3oiIGZpbGw9IiM3MzdkODIiLz4KPC9nPgo8L3N2Zz4K) 100%/10px no-repeat;
}
.locale-select, .locale-select:active, .locale-select:focus {
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    outline: none;
    background-color: #323237;
    border: none;
    color: #fff;
}
.legal-copyright {
    margin-bottom: 10px;
    color: #888;
}
.locale-select option {
    background: #323237;
    color: #fff;
}
.legal {
    text-align: center;
}
.legal-link {
    font-size: 11px;
    color: #737d82;
    text-decoration: none;
}
.legal-link+.legal-link {
    margin-left: 20px;
}
@include media-breakpoint-up(lg){
.ggr-footer {
    padding: 0;
    line-height: 64px;
}
.locale {
    float: right;
    text-align: right;
    margin-bottom: 0;
}
.legal-copyright {
    float: left;
    margin-bottom: 0;
}
.legal-copyright {
    margin-right: 25px;
}
.legal {
    float: left;
}
.legal-links {
    float: left;
}
}

</style>
