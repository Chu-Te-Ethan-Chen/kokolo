<template lang='pug'>
nav.ggr-directory
  .gc-container
    .dt-layout
      .dt-socials
        a.dt-icon.dt-icon--logo(href)
        .dt-social-links
          a.dt-social-link(href='http://www.facebook.com/gogoro' target='_blank')
            i.dt-icon.dt-icon--facebook
            | Facebook 
          a.dt-social-link(href='http://www.youtube.com/GogoroChannel' target='_blank')
            i.dt-icon.dt-icon--youtube
            | Youtube 
          a.dt-social-link(href='http://twitter.com/WeAreGogoro' target='_blank')
            i.dt-icon.dt-icon--twitter
            | Twitter 
          a.dt-social-link(href='http://www.instagram.com/gogoro_taiwan/' target='_blank')
            i.dt-icon.dt-icon--instagram
            | Instagram 
          a.dt-social-link(href='http://www.linkedin.com/company/gogoro' target='_blank')
            i.dt-icon.dt-icon--linkedin
            | Linkedin

      .dt-sections
        .dt-section(data-v-3eb1cdaa)
          .dt-section-name(data-v-3eb1cdaa) Smartscooter
          .dt-section-links(data-v-3eb1cdaa)
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/s-performance/') S Performance
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/1-series/') Gogoro 1 Series
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/2-series/') Gogoro 2 Series
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/3-series/') Gogoro 3 Series
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/viva/') Gogoro VIVA
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/viva/mix/') Gogoro VIVA MIX
            a.dt-section-link(data-v-3eb1cdaa href='/software/') iQ System®
            a.dt-section-link(data-v-3eb1cdaa href='/smartscooter/specs/') Compare Specs
        .dt-section(data-v-3eb1cdaa)
          .dt-section-name(data-v-3eb1cdaa) Smart Power
          .dt-section-links(data-v-3eb1cdaa)
            a.dt-section-link(data-v-3eb1cdaa href='/gogoro-network/') Gogoro Network®
        .dt-section(data-v-3eb1cdaa)
          .dt-section-name(data-v-3eb1cdaa) News
          .dt-section-links(data-v-3eb1cdaa)
            a.dt-section-link(data-v-3eb1cdaa href='/news/') Latest
            a.dt-section-link(data-v-3eb1cdaa href='/about-us/') About Us
            a.dt-section-link(data-v-3eb1cdaa href='/media-center/') Media Center
            a.dt-section-link(data-v-3eb1cdaa href='/media-center/logos/') Media Assets
            a.dt-section-link(data-v-3eb1cdaa href='/media-center/#section-contact') Inquires
        .dt-section(data-v-3eb1cdaa)
          .dt-section-name(data-v-3eb1cdaa) Get Support
          .dt-section-links(data-v-3eb1cdaa)
            a.dt-section-link(data-v-3eb1cdaa href='https://support.gogoro.com/en/') Tech Support
            a.dt-section-link(data-v-3eb1cdaa href='https://support.gogoro.com/en') Mail Us
            a.dt-section-link(data-v-3eb1cdaa href='https://support.gogoro.com/en/faq/') FAQ
</template>

<script>
export default {
  name: "DefaultDirectory",
};
</script>

<style lang="scss" scoped>
.ggr-directory {
    position: relative;
    background-color: #323237;
}
.gc-container {
    margin-left: auto;
    margin-right: auto;
    padding-left: 15px;
    padding-right: 15px;
}
.dt-layout {
    padding: 60px 0 0;
    border-bottom: 1px solid hsla(0,0%,100%,.08);
}
.dt-icon {
    display: block;
    background: 50%/contain no-repeat;
    width: 20px;
    height: 20px;
}
.dt-icon--facebook {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHZpZXdCb3g9IjAgMCAyMCAyMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0wLjQwODcyNiAyLjA0NzU0QzAgMi44NDk3IDAgMy44OTk4IDAgNlYxNEMwIDE2LjEwMDIgMCAxNy4xNTAzIDAuNDA4NzI2IDE3Ljk1MjVDMC43NjgyNTEgMTguNjU4MSAxLjM0MTkzIDE5LjIzMTcgMi4wNDc1NCAxOS41OTEzQzIuODQ5NyAyMCAzLjg5OTggMjAgNiAyMEg4LjQ3ODQ1VjEyLjk5NDlINS44NzVWOS45NjcyOUg4LjQ3ODQ1VjcuNzM5NzFDOC40Nzg0NSA1LjE1Njk1IDEwLjA1NzggMy43NTAwNSAxMi4zNjEyIDMuNzUwMDVDMTMuMTM3NCAzLjc0ODM2IDEzLjkxMzIgMy43ODc0OSAxNC42ODUzIDMuODY3MjlWNi41NjcyOUgxMy4wOTkxQzExLjg0NCA2LjU2NzI5IDExLjU5OTEgNy4xNjA0IDExLjU5OTEgOC4wMzYyNlY5Ljk2Mzg1SDE0LjU5OTFMMTQuMjA5NSAxMi45OTE0SDExLjU4MTlWMjBIMTRDMTYuMTAwMiAyMCAxNy4xNTAzIDIwIDE3Ljk1MjUgMTkuNTkxM0MxOC42NTgxIDE5LjIzMTcgMTkuMjMxNyAxOC42NTgxIDE5LjU5MTMgMTcuOTUyNUMyMCAxNy4xNTAzIDIwIDE2LjEwMDIgMjAgMTRWNkMyMCAzLjg5OTggMjAgMi44NDk3IDE5LjU5MTMgMi4wNDc1NEMxOS4yMzE3IDEuMzQxOTMgMTguNjU4MSAwLjc2ODI1MSAxNy45NTI1IDAuNDA4NzI2QzE3LjE1MDMgMCAxNi4xMDAyIDAgMTQgMEg2QzMuODk5OCAwIDIuODQ5NyAwIDIuMDQ3NTQgMC40MDg3MjZDMS4zNDE5MyAwLjc2ODI1MSAwLjc2ODI1MSAxLjM0MTkzIDAuNDA4NzI2IDIuMDQ3NTRaIiBmaWxsPSIjQjlCQ0JGIi8+Cjwvc3ZnPgo=);
}
.dt-icon--youtube {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHZpZXdCb3g9IjAgMCAyMCAyMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTE5LjU4MTggNC43QzE5LjQ2ODcgNC4yNzQ1MSAxOS4yNDU5IDMuODg2MTggMTguOTM1NiAzLjU3Mzg4QzE4LjYyNTMgMy4yNjE1OCAxOC4yMzg0IDMuMDM2MjUgMTcuODEzNiAyLjkyMDQ1QzE2LjI1IDIuNSAxMCAyLjUgMTAgMi41QzEwIDIuNSAzLjc1IDIuNSAyLjE4NjM2IDIuOTIwNDVDMS43NjE2MSAzLjAzNjI1IDEuMzc0NzIgMy4yNjE1OCAxLjA2NDQxIDMuNTczODhDMC43NTQwOTcgMy44ODYxOCAwLjUzMTI1NSA0LjI3NDUxIDAuNDE4MTgyIDQuN0MwIDYuMjcwNDUgMCA5LjU0NTQ1IDAgOS41NDU0NUMwIDkuNTQ1NDUgMCAxMi44MjA1IDAuNDE4MTgyIDE0LjM5MDlDMC41MzEyNTUgMTQuODE2NCAwLjc1NDA5NyAxNS4yMDQ3IDEuMDY0NDEgMTUuNTE3QzEuMzc0NzIgMTUuODI5MyAxLjc2MTYxIDE2LjA1NDcgMi4xODYzNiAxNi4xNzA1QzMuNzUgMTYuNTkwOSAxMCAxNi41OTA5IDEwIDE2LjU5MDlDMTAgMTYuNTkwOSAxNi4yNSAxNi41OTA5IDE3LjgxMzYgMTYuMTcwNUMxOC4yMzg0IDE2LjA1NDcgMTguNjI1MyAxNS44MjkzIDE4LjkzNTYgMTUuNTE3QzE5LjI0NTkgMTUuMjA0NyAxOS40Njg3IDE0LjgxNjQgMTkuNTgxOCAxNC4zOTA5QzIwIDEyLjgyMDUgMjAgOS41NDU0NSAyMCA5LjU0NTQ1QzIwIDkuNTQ1NDUgMjAgNi4yNzA0NSAxOS41ODE4IDQuN1pNNy45NTQ1NSAxMi41MTkzVjYuNTcxNTlMMTMuMTgxOCA5LjU0NTQ1TDcuOTU0NTUgMTIuNTE5M1oiIGZpbGw9IiNCOUJDQkYiLz4KPC9zdmc+Cg==);
}
.dt-icon--twitter {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjEiIGhlaWdodD0iMjAiIHZpZXdCb3g9IjAgMCAyMSAyMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik02LjQ0NjQ1IDE4LjI2MjVDMTMuOTkzNSAxOC4yNjI1IDE4LjEyMzEgMTIuMDA0IDE4LjEyMzEgNi41ODU4NEMxOC4xMjMxIDYuNDA5NzcgMTguMTIzMSA2LjIzMzcgMTguMTE1MSA2LjA1NzYyQzE4LjkxNTQgNS40ODEzOSAxOS42MTE3IDQuNzUzMSAyMC4xNjM5IDMuOTI4NzdDMTkuNDI3NiA0LjI1NjkgMTguNjM1MyA0LjQ3Mjk5IDE3LjgwMyA0LjU3NzAzQzE4LjY1MTMgNC4wNzI4MyAxOS4yOTk2IDMuMjY0NTEgMTkuNjExNyAyLjMwNDEyQzE4LjgxOTQgMi43NzYzMSAxNy45MzkxIDMuMTEyNDUgMTcuMDAyNyAzLjI5NjUyQzE2LjI1MDQgMi40OTYyIDE1LjE4NTkgMiAxNC4wMDk1IDJDMTEuNzQ0NiAyIDkuOTAzODQgMy44NDA3NCA5LjkwMzg0IDYuMTA1NjRDOS45MDM4NCA2LjQyNTc3IDkuOTQzODUgNi43Mzc5IDEwLjAwNzkgNy4wNDIwMkM2LjU5ODUxIDYuODczOTUgMy41NzMzIDUuMjMzMjkgMS41NDg0OSAyLjc1MjNDMS4xOTYzNSAzLjM2MDU0IDAuOTk2MjczIDQuMDY0ODMgMC45OTYyNzMgNC44MTcxM0MwLjk5NjI3MyA2LjI0MTcgMS43MjQ1NiA3LjQ5ODIgMi44MjEgOC4yMzQ1QzIuMTQ4NzMgOC4yMTA0OSAxLjUxNjQ4IDguMDI2NDEgMC45NjQyNjEgNy43MjIyOUMwLjk2NDI2MSA3LjczODMgMC45NjQyNjEgNy43NTQzIDAuOTY0MjYxIDcuNzc4MzFDMC45NjQyNjEgOS43NjMxMSAyLjM4MDgzIDExLjQyNzggNC4yNTM1OCAxMS44MDM5QzMuOTA5NDQgMTEuOSAzLjU0OTI5IDExLjk0OCAzLjE3MzE0IDExLjk0OEMyLjkwOTA0IDExLjk0OCAyLjY1Mjk0IDExLjkyNCAyLjQwNDg0IDExLjg3NkMyLjkyNTA1IDEzLjUwODYgNC40NDU2NSAxNC42OTMxIDYuMjM4MzcgMTQuNzI1MUM0LjgyOTgxIDE1LjgyOTUgMy4wNjExIDE2LjQ4NTggMS4xNDAzMyAxNi40ODU4QzAuODEyMiAxNi40ODU4IDAuNDg0MDY4IDE2LjQ2OTggMC4xNjM5NCAxNi40Mjk4QzEuOTcyNjYgMTcuNTgyMiA0LjEzMzUzIDE4LjI2MjUgNi40NDY0NSAxOC4yNjI1WiIgZmlsbD0iI0I5QkNCRiIvPgo8L3N2Zz4K);
}
.dt-icon--instagram {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHZpZXdCb3g9IjAgMCAyMCAyMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik01Ljg3NzAxIDAuMDYwMTc3N0M2Ljk0MzYyIDAuMDExNTExNiA3LjI4NDE2IDAgMTAgMEMxMi43MTU4IDAgMTMuMDU2NCAwLjAxMTUxMTYgMTQuMTIzIDAuMDYwMTc3N0MxNS4xODc0IDAuMTA4NzI1IDE1LjkxNDMgMC4yNzc3ODYgMTYuNTUwNCAwLjUyNTAwN0MxNy4yMDggMC43ODA1MjQgMTcuNzY1NiAxLjEyMjQ2IDE4LjMyMTYgMS42NzgzOUMxOC44Nzc1IDIuMjM0MzYgMTkuMjE5NSAyLjc5MjAzIDE5LjQ3NSAzLjQ0OTYyQzE5LjcyMjIgNC4wODU2OSAxOS44OTEzIDQuODEyNjMgMTkuOTM5OCA1Ljg3NzAxQzE5Ljk4ODUgNi45NDM2MiAyMCA3LjI4NDE2IDIwIDEwQzIwIDEyLjcxNTggMTkuOTg4NSAxMy4wNTY0IDE5LjkzOTggMTQuMTIzQzE5Ljg5MTMgMTUuMTg3NCAxOS43MjIyIDE1LjkxNDMgMTkuNDc1IDE2LjU1MDRDMTkuMjE5NSAxNy4yMDggMTguODc3NSAxNy43NjU2IDE4LjMyMTYgMTguMzIxNkMxNy43NjU2IDE4Ljg3NzUgMTcuMjA4IDE5LjIxOTUgMTYuNTUwNCAxOS40NzVDMTUuOTE0MyAxOS43MjIyIDE1LjE4NzQgMTkuODkxMyAxNC4xMjMgMTkuOTM5OEMxMy4wNTY0IDE5Ljk4ODUgMTIuNzE1OCAyMCAxMCAyMEM3LjI4NDE2IDIwIDYuOTQzNjIgMTkuOTg4NSA1Ljg3NzAxIDE5LjkzOThDNC44MTI2MyAxOS44OTEzIDQuMDg1NjkgMTkuNzIyMiAzLjQ0OTYyIDE5LjQ3NUMyLjc5MjAzIDE5LjIxOTUgMi4yMzQzNiAxOC44Nzc1IDEuNjc4MzkgMTguMzIxNkMxLjEyMjQ2IDE3Ljc2NTYgMC43ODA1MjQgMTcuMjA4IDAuNTI1MDA3IDE2LjU1MDRDMC4yNzc3ODYgMTUuOTE0MyAwLjEwODcyNSAxNS4xODc0IDAuMDYwMTc3NyAxNC4xMjNDMC4wMTE1MTE2IDEzLjA1NjQgMCAxMi43MTU4IDAgMTBDMCA3LjI4NDE2IDAuMDExNTExNiA2Ljk0MzYyIDAuMDYwMTc3NyA1Ljg3NzAxQzAuMTA4NzI1IDQuODEyNjMgMC4yNzc3ODYgNC4wODU2OSAwLjUyNTAwNyAzLjQ0OTYyQzAuNzgwNTI0IDIuNzkyMDMgMS4xMjI0NiAyLjIzNDM2IDEuNjc4MzkgMS42NzgzOUMyLjIzNDM2IDEuMTIyNDYgMi43OTIwMyAwLjc4MDUyNCAzLjQ0OTYyIDAuNTI1MDA3QzQuMDg1NjkgMC4yNzc3ODYgNC44MTI2MyAwLjEwODcyNSA1Ljg3NzAxIDAuMDYwMTc3N1pNMTUuODk3NyAyLjIwNDM4QzE1LjU0NTQgMi4wNjc0NCAxNS4wMTU5IDEuOTA0NTMgMTQuMDQwOSAxLjg2MDA3QzEyLjk4NjQgMS44MTE5NiAxMi42NzAxIDEuODAxNzYgMTAgMS44MDE3NkM3LjMyOTkgMS44MDE3NiA3LjAxMzYxIDEuODExOTYgNS45NTkxNSAxLjg2MDA3QzQuOTg0MTYgMS45MDQ1MyA0LjQ1NDY3IDIuMDY3NDQgNC4xMDIzIDIuMjA0MzhDMy42MzU1MiAyLjM4NTc5IDMuMzAyNCAyLjYwMjQ5IDIuOTUyNDkgMi45NTI0NEMyLjYwMjU0IDMuMzAyMzUgMi4zODU4NCAzLjYzNTQ3IDIuMjA0NDQgNC4xMDIyNUMyLjA2NzQ5IDQuNDU0NjIgMS45MDQ1OCA0Ljk4NDExIDEuODYwMTIgNS45NTkxQzEuODEyMDEgNy4wMTM1NiAxLjgwMTgxIDcuMzI5ODUgMS44MDE4MSA5Ljk5OTk4QzEuODAxODEgMTIuNjcwMSAxLjgxMjAxIDEyLjk4NjQgMS44NjAxMiAxNC4wNDA4QzEuOTA0NTggMTUuMDE1OCAyLjA2NzQ5IDE1LjU0NTMgMi4yMDQ0NCAxNS44OTc3QzIuMzg1ODQgMTYuMzY0NCAyLjYwMjU4IDE2LjY5NzYgMi45NTI0OSAxNy4wNDc1QzMuMzAyNCAxNy4zOTc0IDMuNjM1NTIgMTcuNjE0MSA0LjEwMjMgMTcuNzk1NUM0LjQ1NDY3IDE3LjkzMjUgNC45ODQxNiAxOC4wOTU0IDUuOTU5MTUgMTguMTM5OEM3LjAxMzQ5IDE4LjE4OCA3LjMyOTcgMTguMTk4MiAxMCAxOC4xOTgyQzEyLjY3MDMgMTguMTk4MiAxMi45ODY2IDE4LjE4OCAxNC4wNDA5IDE4LjEzOThDMTUuMDE1OSAxOC4wOTU0IDE1LjU0NTQgMTcuOTMyNSAxNS44OTc3IDE3Ljc5NTVDMTYuMzY0NSAxNy42MTQxIDE2LjY5NzYgMTcuMzk3NCAxNy4wNDc1IDE3LjA0NzVDMTcuMzk3NSAxNi42OTc2IDE3LjYxNDIgMTYuMzY0NCAxNy43OTU2IDE1Ljg5NzdDMTcuOTMyNSAxNS41NDUzIDE4LjA5NTQgMTUuMDE1OCAxOC4xMzk5IDE0LjA0MDhDMTguMTg4IDEyLjk4NjQgMTguMTk4MiAxMi42NzAxIDE4LjE5ODIgOS45OTk5OEMxOC4xOTgyIDcuMzI5ODUgMTguMTg4IDcuMDEzNTYgMTguMTM5OSA1Ljk1OTFDMTguMDk1NCA0Ljk4NDExIDE3LjkzMjUgNC40NTQ2MiAxNy43OTU2IDQuMTAyMjVDMTcuNjE0MiAzLjYzNTQ3IDE3LjM5NzUgMy4zMDIzNSAxNy4wNDc1IDIuOTUyNDRDMTYuNjk3NiAyLjYwMjQ5IDE2LjM2NDUgMi4zODU3OSAxNS44OTc3IDIuMjA0MzhaTTEwIDQuODY0ODhDNy4xNjM5NCA0Ljg2NDg4IDQuODY0ODggNy4xNjM5NCA0Ljg2NDg4IDEwQzQuODY0ODggMTIuODM2MSA3LjE2Mzk0IDE1LjEzNTEgMTAgMTUuMTM1MUMxMi44MzYxIDE1LjEzNTEgMTUuMTM1MSAxMi44MzYxIDE1LjEzNTEgMTBDMTUuMTM1MSA3LjE2Mzk0IDEyLjgzNjEgNC44NjQ4OCAxMCA0Ljg2NDg4Wk02LjY2NjY1IDkuOTk5OTlDNi42NjY2NSAxMS44NDA5IDguMTU5MDMgMTMuMzMzMyAxMCAxMy4zMzMzQzExLjg0MDkgMTMuMzMzMyAxMy4zMzMzIDExLjg0MDkgMTMuMzMzMyA5Ljk5OTk5QzEzLjMzMzMgOC4xNTkwMiAxMS44NDA5IDYuNjY2NjQgMTAgNi42NjY2NEM4LjE1OTAzIDYuNjY2NjQgNi42NjY2NSA4LjE1OTAyIDYuNjY2NjUgOS45OTk5OVpNMTUuMzM4IDUuODYxOTlDMTYuMDAwOCA1Ljg2MTk5IDE2LjUzOCA1LjMyNDc2IDE2LjUzOCA0LjY2MjAxQzE2LjUzOCAzLjk5OTI2IDE2LjAwMDggMy40NjE5OSAxNS4zMzggMy40NjE5OUMxNC42NzUzIDMuNDYxOTkgMTQuMTM4IDMuOTk5MjYgMTQuMTM4IDQuNjYyMDFDMTQuMTM4IDUuMzI0NzYgMTQuNjc1MyA1Ljg2MTk5IDE1LjMzOCA1Ljg2MTk5WiIgZmlsbD0iI0I5QkNCRiIvPgo8L3N2Zz4K);
}
.dt-icon--linkedin {
    background-image: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHZpZXdCb3g9IjAgMCAyMCAyMCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0wLjQwODcyNiAyLjA0NzU0QzAgMi44NDk3IDAgMy44OTk4IDAgNlYxNEMwIDE2LjEwMDIgMCAxNy4xNTAzIDAuNDA4NzI2IDE3Ljk1MjVDMC43NjgyNTEgMTguNjU4MSAxLjM0MTkzIDE5LjIzMTcgMi4wNDc1NCAxOS41OTEzQzIuODQ5NyAyMCAzLjg5OTggMjAgNiAyMEgxNEMxNi4xMDAyIDIwIDE3LjE1MDMgMjAgMTcuOTUyNSAxOS41OTEzQzE4LjY1ODEgMTkuMjMxNyAxOS4yMzE3IDE4LjY1ODEgMTkuNTkxMyAxNy45NTI1QzIwIDE3LjE1MDMgMjAgMTYuMTAwMiAyMCAxNFY2QzIwIDMuODk5OCAyMCAyLjg0OTcgMTkuNTkxMyAyLjA0NzU0QzE5LjIzMTcgMS4zNDE5MyAxOC42NTgxIDAuNzY4MjUxIDE3Ljk1MjUgMC40MDg3MjZDMTcuMTUwMyAwIDE2LjEwMDIgMCAxNCAwSDZDMy44OTk4IDAgMi44NDk3IDAgMi4wNDc1NCAwLjQwODcyNkMxLjM0MTkzIDAuNzY4MjUxIDAuNzY4MjUxIDEuMzQxOTMgMC40MDg3MjYgMi4wNDc1NFpNMTUuNDk1MSA4LjUwNDk1QzE0Ljc0NSA3Ljc1NDggMTMuNzI3NSA3LjMzMzM3IDEyLjY2NjcgNy4zMzMzN0MxMS42MDU4IDcuMzMzMzcgMTAuNTg4NCA3Ljc1NDggOS44MzgyNCA4LjUwNDk1QzkuMDg4MSA5LjI1NTA5IDguNjY2NjcgMTAuMjcyNSA4LjY2NjY3IDExLjMzMzRWMTZIMTEuMzMzM1YxMS4zMzM0QzExLjMzMzMgMTAuOTc5OCAxMS40NzM4IDEwLjY0MDYgMTEuNzIzOSAxMC4zOTA2QzExLjk3MzkgMTAuMTQwNSAxMi4zMTMxIDEwIDEyLjY2NjcgMTBDMTMuMDIwMyAxMCAxMy4zNTk0IDEwLjE0MDUgMTMuNjA5NSAxMC4zOTA2QzEzLjg1OTUgMTAuNjQwNiAxNCAxMC45Nzk4IDE0IDExLjMzMzRWMTZIMTYuNjY2N1YxMS4zMzM0QzE2LjY2NjcgMTAuMjcyNSAxNi4yNDUyIDkuMjU1MDkgMTUuNDk1MSA4LjUwNDk1Wk01Ljk5OTk5IDE2VjhIMy4zMzMzM1YxNkg1Ljk5OTk5Wk01Ljk5OTk5IDQuNjY2NzFDNS45OTk5OSA1LjQwMzA5IDUuNDAzMDQgNi4wMDAwNCA0LjY2NjY2IDYuMDAwMDRDMy45MzAyOCA2LjAwMDA0IDMuMzMzMzMgNS40MDMwOSAzLjMzMzMzIDQuNjY2NzFDMy4zMzMzMyAzLjkzMDMzIDMuOTMwMjggMy4zMzMzNyA0LjY2NjY2IDMuMzMzMzdDNS40MDMwNCAzLjMzMzM3IDUuOTk5OTkgMy45MzAzMyA1Ljk5OTk5IDQuNjY2NzFaIiBmaWxsPSIjQjlCQ0JGIi8+Cjwvc3ZnPgo=);
}
.dt-social-link .dt-icon {
    margin: 0 8px 0 0;
}
.dt-icon--logo {
    width: 100px;
    height: 36px;
    background-image: url("~@/assets/logo.svg");
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
.dt-sections {
    margin: 4px 0 0;
}
.dt-section {
    font-size: 14px;
    border-top: 1px solid hsla(0,0%,100%,.08);
    padding: 14px 0;
}
.dt-section-name {
    position: relative;
    cursor: pointer;
    color: #737d82;
}
.dt-section-links {
    overflow: hidden;
    max-height: 0;
    -webkit-transition: max-height .3s,opacity .2s,-webkit-transform .3s .3s;
    transition: max-height .3s,opacity .2s,-webkit-transform .3s .3s;
    transition: max-height .3s,transform .3s .3s,opacity .2s;
    transition: max-height .3s,transform .3s .3s,opacity .2s,-webkit-transform .3s .3s;
    -webkit-transform: translateX(-30px);
    transform: translateX(-30px);
    opacity: 0;
}
.dt-section-links:before {
    content: "";
    display: block;
    height: 16px;
}
.dt-section-link {
    display: block;
    font-size: 14px;
    line-height: 1.4;
    color: #f6f6f6;
    text-decoration: none;
}
.dt-section-link+.dt-section-link {
    margin: 8px 0 0;
}
@include media-breakpoint-up(sm){
  .gc-container {
    max-width: 576px;
}
} 
@include media-breakpoint-up(md){
.gc-container {
    max-width: 720px;
}
}
@include media-breakpoint-up(lg){
.gc-container {
    max-width: 940px;
}
.dt-layout {
    padding: 60px 0;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
}
.dt-socials {
    -webkit-box-flex: 0;
    -ms-flex: 0 0 20%;
    flex: 0 0 20%;
}
.dt-social-links {
    margin: 60px 0 0;
    display: block;
}
.dt-sections {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
    -ms-flex-flow: row wrap;
    flex-flow: row wrap;
}
.dt-sections {
    -webkit-box-flex: 1;
    -ms-flex: 1;
    flex: 1;
    margin: 0 -5px;
}
.dt-section {
    -webkit-box-flex: 0;
    -ms-flex: 0 0 33.3%;
    flex: 0 0 33.3%;
    padding: 0 5px;
}
.dt-section {
    padding: 0;
    border: none;
    margin: 0 0 60px;
}
.dt-section-links {
    opacity: 1;
    -webkit-transform: none;
    transform: none;
    -webkit-transition: none;
    transition: none;
    max-height: none;
}
}
@include media-breakpoint-up(xl){
.gc-container {
    max-width: 1140px;
}
.dt-socials {
    -webkit-box-flex: 0;
    -ms-flex: 0 0 25%;
    flex: 0 0 25%;
}
.dt-section {
    -webkit-box-flex: 0;
    -ms-flex: 0 0 25%;
    flex: 0 0 25%;
}
}
</style>
