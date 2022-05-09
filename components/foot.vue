<template>
  <div class="container">
    <div class="foot">
      <div class="footer-bottom">
        <div class="left"><img src="../assets/images/footer-logo.svg" /></div>

        <div class="bottom-right">
          <div class="reference">
            <div class="resources">
              <p class="text">About us</p>
              <ul class="">
                <nuxt-link to="/" class="item">
                  <p class="links">Company</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Security</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Address</p>
                </nuxt-link>
              </ul>
            </div>
            <div class="company">
              <p class="text">Contact Us</p>
              <ul class="">
                <nuxt-link to="/" class="item">
                  <p class="links">Email</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Whatsapp</p>
                </nuxt-link>
                <nuxt-link to="/" class="item">
                  <p class="links">Slack</p>
                </nuxt-link>
              </ul>
            </div>
            <div class="company">
              <p class="text">Support</p>
              <ul class="">
                <nuxt-link to="/" class="item">
                  <p class="links">Email</p>
                </nuxt-link>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="lastFooter-bottom">
        <div class="left"><p class="copyrightyear">All rights reserved ajo cc 2022</p></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'foot',
}
</script>

<style scoped>
.container {
  /* background: #0c1f55; */
  width: 100%;
  max-width: 1440px;
  margin: 0px auto;
  /* margin-right: 0px !important; */
}
.foot {
  width: 90%;
  margin: 0 auto;
}
.footer-bottom {
  padding-top: 40px;
  display: flex;
  justify-content: space-between;
  margin: 40px auto 90px auto;
}
.lastFooter-bottom {
  width: 100%;
  padding-top: 20px;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
}

.bottom-right {
  width: 35%;
}
.reference {
  display: flex;
  justify-content: space-around;
}
.resources .text,
.company .text {
  font-weight: 700;
  font-size: 18px;
  line-height: 36px;
  color: #000;
}
.links {
  font-weight: 300;
  font-size: 15px;
  line-height: 36px;
  color: #000;
  padding-top: 20px;
}

.copyrightyear {
  font-weight: 300;
  font-size: 14px;
  line-height: 36px;
  color: #000;
  text-align: center;
}
@media screen and (max-width: 1200px) {
  .footer-bottom {
    display: block;
  }
  .bottom-right {
    width: 100%;
  }
  .reference {
    width: 100%;
    margin-top: 30px;
  }
  
}
</style>
