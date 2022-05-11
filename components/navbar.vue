<template>
  <div class="">
    <div class="topnav" id="myTopnav" ref="myTopnav">
      <div class="logo">
        <nuxt-link to="#" class="" exact-active-class="">
          <img src="../assets/images/logo.svg" />
        </nuxt-link>
        <div class="line"></div>
      </div>

      <div class="doing">
        <nuxt-link to="/" class="navv" >
          <p class="nav-link">Home</p>
        </nuxt-link>
        <nuxt-link to="#Product" class="navv" exact>
          <p class="nav-link">Product</p>
        </nuxt-link>
        <nuxt-link to="#Contact" class="navv" exact>
          <p class="nav-link">Contact</p>
        </nuxt-link>
      </div>

      <div class="details">
        <nuxt-link to="#started" class="" exact-active-class="">
          <button class="started">Sign up</button>
        </nuxt-link>
        <nuxt-link to="#login" class="" exact-active-class="">
          <button class="login">Login</button>
        </nuxt-link>
      </div>
      <a href="javascript:void(0);" class="icon" @click="myFunction()">
        <img src="../assets/images/icon.png" />
      </a>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    myFunction() {
      const x = this.$refs.myTopnav
      if (x.className === 'topnav') {
        x.className += ' responsive'
      } else {
        x.className = 'topnav'
      }
    },
  },
}
</script>

<style scoped>
.topnav {
  overflow: hidden;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 0px auto;
  width: 90%;
  max-width: 1440px;
}

.topnav a {
  float: left;
  display: block;
  text-decoration: none;
  font-weight: 400;
  font-size: 20px;
  line-height: 26px;
  margin-top: 10px;
  margin: 10px 0px 10px 0px;
  color: #fff;
  text-align: center;
  align-items: center;
}
.navv{
  padding-right: 48px;
}
.logo {
 display: flex;
 justify-content: center;
 align-items: center;
}
.line{
 height: 20px;
 border-right: 1px solid #fffee6;
}

/* active */
.nuxt-link-exact-active{
  border-bottom: 2px solid #fcf300;
}

.doing {
  margin-left: 25%;
  width: 400px;
  display: flex;
  justify-content: center;
  /* background: pink; */
}

.topnav .icon {
  display: none;
}

.details {
  width: 450px;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px 0px 10px 0px;
}
.sign {
  font-size: 14px;
  line-height: 18px;
  text-align: center;
  color: #476bd2;
  padding-right: 25px;
}
.details button {
  font-weight: 500;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  border-radius: 56px;
  width: 171px;
  height: 56px;
}
.details .started {
  background: #fcf300;
  color: #9a9400;
  margin-right: 14px;
}
.login {
  border: 2px solid #fffee6;
  color: #fffee6;
  background: transparent;
}

@media screen and (max-width: 1200px) {
  .topnav a:not(:first-child),
  .details a,
  .doing a {
    display: none;
  }
  .topnav a.icon {
    float: right;
    display: block;
     position: absolute;
    right: 0;
    top: 0;
    padding: 14px 16px;
  }
  .topnav {
    display: block;
    padding: 0;
  }
  .logo{
    justify-content: flex-start;
  }
}

@media screen and (max-width: 1200px) {
  .topnav.responsive {
    position: relative;
  }
  .topnav.responsive .icon {
    position: absolute;
    right: 0;
    top: 0;
    padding: 14px 16px;
  }
  .topnav.responsive a {
    float: none;
    display: block;
    text-align: left;
  }
  .doing {
  margin-left: 0%;
  padding-left:4%;
  justify-content: flex-start;
 
}

}
@media screen and (max-width: 500px) {
  .details {
  display: block;
}
.details button {
  margin-top: 20px;
  margin-left: 5%;
}
 .doing {
  padding-left:8%;
}
}
</style>
