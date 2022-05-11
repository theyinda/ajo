<template>
  <div class="all">
    <div class="navigation">
      <navbar />
    </div>

    <div class="over-all">
      <div class="hero">
        <div class="hero-container">
          <div class="map"><img src="../assets/images/cloud.svg" /></div>
          <div>
            <h2>Ajo</h2>
            <p>The travel guide</p>
          </div>
          <div class="phone">
            <img src="../assets/images/phone.svg" />
          </div>
          <div class="sky"><img src="../assets/images/sky.svg" /></div>
        </div>
      </div>

      <div class="store-container">
        <div class="store">
          <img src="../assets/images/google.svg" />
          <img src="../assets/images/apple.svg" />
        </div>
      </div>
      <div class="understand-container">
        <div class="leftBorder"></div>
        <div class="text">
          <h3>We understand, exploring cities can be hard</h3>
        </div>
        <div class="rightBorder"></div>
      </div>
      <div class="cities-container">
        <div class="city">
          <img src="../assets/images/road.svg" />
          <p>You run the risk of getting lost.</p>
        </div>
        <div class="city">
          <img src="../assets/images/online.svg" />
          <p>Not a lot of options for you to explore.</p>
        </div>
        <div class="city">
          <img src="../assets/images/update.svg" />
          <p>Missing out a lot of fun activities and attractions.</p>
        </div>
      </div>

      <div class="explore-container">
        <div class="exploreOne">
          <div class="imageCon">
            <img src="../assets/images/exploreOne.svg" />
          </div>

          <div class="explore">
            <h3>Explore cities with ease</h3>
            <p>
              Find local attractions and hot spots easily without the stress of
              asking the locals.
            </p>
          </div>
        </div>
        <div class="exploreOne">
          <div class="explore">
            <h3>Never get lost</h3>
            <p>
              Get directions directly from the app and also book rides with
              local car hires directly.
            </p>
          </div>
          <div class="imageCon">
            <img src="../assets/images/exploreTwo.svg" />
          </div>
        </div>
        <div class="exploreOne">
          <div class="imageCon">
            <img src="../assets/images/third.svg" />
          </div>

          <div class="explore">
            <h3>International suggestions</h3>
            <p>
              Get trip ideas for other countries and cities for you to explore
              when in doubt.
            </p>
          </div>
        </div>
      </div>
      <div class="review-container">
        <div class="review-slides">
          <img src="../assets/images/left.svg" class="left" />
          <img src="../assets/images/box.svg" />
          <img src="../assets/images/right.svg" class="left" />
        </div>
        <div class="more">
          <span>See more reviews</span>
          <img src="../assets/images/arrow.svg" />
        </div>
      </div>

      <div class="footerb">
        <foot />
      </div>
    </div>
  </div>
</template>

<script>
import Foot from '../components/foot.vue'
import navbar from '../components/navbar.vue'
export default {
  name: 'IndexPage',
  components: { navbar, Foot },
  data() {
    return {}
  },
}
</script>

<style scoped>
.all {
  background: #fff;
  width: 100%;
  margin: 0 auto;
}
.navigation {
  background: #041a7a;
  width: 100%;
}
.over-all {
  margin: 0 auto 0 auto;
}
.hero {
  width: 100%;
  background: #041a7a;
}
.hero-container {
  margin: 0 auto 346px auto;
  text-align: center;
  max-width: 1440px;
  padding-top: 60px;
  position: relative;
  height: 794px;
}
.map {
  position: absolute;
  left: 0px;
}
.sky {
  position: absolute;
  right: 195px;
  bottom: 185px;
  z-index: 1;
}
.hero-container h2 {
  font-weight: 900;
  font-size: 96px;
  line-height: 125px;
  color: #fff;
  text-align: center;
  padding-bottom: 20px;
}
.hero-container p {
  font-weight: 500;
  font-size: 35px;
  line-height: 46px;
  color: #fff;
}
.phone {
  width: 100%;
  margin-top: 100px;
  position: absolute;
  z-index: 3;
}
.phone img {
}

.explore-container {
  border-top: 1px solid rgba(0, 0, 0, 0.3);
  width: 90%;
  margin: 40px auto;
  max-width: 1440px;
}
.exploreOne {
  display: flex;
  align-items: center;
  margin-top: 200px;
  justify-content: space-evenly;
}
.exploreOne h3 {
  font-weight: 500;
  font-size: 35px;
  line-height: 44px;
  width: 451px;
  height: 23px;
  padding-bottom: 25px;
  margin-bottom: 28px;
  border-bottom: 20px solid #fcf300;
}
.exploreOne p {
  font-weight: 400;
  font-size: 24px;
  line-height: 36px;
  width: 383px;
}
.review-container {
  width: 90%;
  margin: 200px auto 70px auto;
  max-width: 1440px;
}
.review-slides {
  display: flex;
  justify-content: center;
  align-items: center;
}
.left {
  padding: 20px;
  background: #fdf86b;
  border-radius: 50%;
  cursor: pointer;
}
.more {
  display: flex;
  justify-content: center;
  align-items: center;
}
.more span {
  font-weight: 300;
  font-size: 24px;
  line-height: 36px;
  color: #041a7a;
}
.more img {
  margin-left: 10px;
  cursor: pointer;
}
.store-container {
  width: 90%;
  margin: 90px auto;
  max-width: 1440px;
  display: flex;
  /* height: 100px; */
  justify-content: center;
  align-items: center;
}

.store-container img {
  margin-left: 26px;
}
.understand-container {
  width: 90%;
  margin: 60px auto 80px auto;
  max-width: 1440px;
  display: flex;
  height: 100px;
  justify-content: space-between;
  align-items: center;
}
.leftBorder {
  height: 1px;
  width: 397px;
  border: 1px solid rgba(0, 0, 0, 0.3);
}
.text h3 {
  font-weight: 500;
  font-size: 35px;
  line-height: 44px;
  width: 452px;
  text-align: center;
  height: 23px;
  padding-bottom: 67px;
  margin-bottom: 28px;
  border-bottom: 20px solid #fcf300;
}
.rightBorder {
  height: 1px;
  width: 397px;
  border: 1px solid rgba(0, 0, 0, 0.3);
}
.cities-container {
  width: 90%;
  margin: 60px auto;
  max-width: 1440px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.city {
  margin-left: 130px;
}
.cities-container p {
  font-weight: 400;
  font-size: 24px;
  width: 216.85px;
  line-height: 36px;
}

.footerb {
  background: #fefa96;
  width: 100%;
}
@media only screen and (max-width: 1200px) {
  .sky,
  .map {
    display: none;
  }
  .cities-container {
    display: block;
    justify-content: center;
    align-items: center;
    margin: 20px auto;
    width: 90%;
  }
  .city {
    width: 70%;
    justify-content: center;
    text-align: center;

    margin-left: 0;
    margin: 20px auto;
  }
  .cities-container p {
    width: 100%;
    padding: 30px 0;
  }
  .explore-container {
    border-top: 1px solid rgba(0, 0, 0, 0.3);
    width: 90%;
    margin: 40px auto;
    max-width: 1440px;

  }
  .exploreOne {
    display: block;
    align-items: center;
    margin-bottom: 50px;
    justify-content: center;
  }
  .exploreOne h3 {
    font-weight: 500;
    font-size: 35px;
    line-height: 44px;
    /* width: 400px; */
    padding-bottom: 25px;
    margin-bottom: 28px;
    border-bottom: 20px solid #fcf300;
  }
  .exploreOne p {
    font-weight: 400;
    font-size: 24px;
    line-height: 36px;
    /* width: 383px; */
  }
  .explore {
    width: 100%;
    margin: 20px auto;
  }
  .exploreOne h3 {
    text-align: center;
    width: 100%;
  }
  .exploreOne p {
    text-align: center;
    width: 100%;
  }
  .imageCon img {
    display: block;
    width: 50%;
    margin: 10px auto;
  }
}
@media only screen and (max-width: 900px) {
  .review-container {
    display: none;
  }
}
@media only screen and (max-width: 600px) {
  .hero-container {
    height: 300px;
    margin: 0 auto 46px auto;
  }
  .phone {
    display: none;
    margin-top: 0px;
  }
  .store{
   width: 100%;
}
  .store-container img {
    display: block;
     width: 50%;
    justify-content: center;
    margin-bottom: 20px;
     margin: 30px auto;
     cursor: pointer;
    /* margin-left: 0px; */
  }
  .text h3 {
    width: 100%;
    text-align: center;
    height: 23px;
    padding-bottom: 67px;
    margin-bottom: 28px;
    border-bottom: 70px solid #fcf300;
  }
  .cities-container {
    margin-top: 180px;
  }
  .exploreOne p {
    padding-bottom: 25px;
    padding-top: 30px;
  }
}
</style>