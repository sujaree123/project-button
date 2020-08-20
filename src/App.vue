<template>
  <div id="app">
    <div class="main-wrapper-first">
      <section class="service-area">
        <div class="container">
          <HelloWorld msg="Dogs on the beach" />
          <div class="row">
            <div class="col-md-6">
              <div class="single-service" style="background: url(img/1.jpg);">
                <div class="overlay overlay-content justify-content-center">
                  <h1>
                    <i class="fas fa-hand-point-right text-secondary"></i>
                    {{total1}}
                    <i class="fas fa-hand-point-left text-secondary"></i>
                  </h1>
                  <CsButton @cc="sum" />
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="single-service" style="background: url(img/2.jpg);">
                <div class="overlay overlay-content justify-content-center">
                  <h1>
                    <i class="fas fa-hand-point-right text-secondary"></i>
                    {{total2}}
                    <i class="fas fa-hand-point-left text-secondary"></i>
                  </h1>
                  <CsButton @cc="sum1" />
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="single-service" style="background: url(img/3.jpg);">
                <div class="overlay overlay-content justify-content-center">
                  <h1>
                    <i class="fas fa-hand-point-right text-secondary"></i>
                    {{total3}}
                    <i class="fas fa-hand-point-left text-secondary"></i>
                  </h1>
                  <CsButton @cc="sum2" />
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="single-service" style="background: url(img/4.jpg);">
                <div class="overlay overlay-content justify-content-center">
                  <h1>
                    <i class="fas fa-hand-point-right text-secondary"></i>
                    {{total4}}
                    <i class="fas fa-hand-point-left text-secondary"></i>
                  </h1>
                  <CsButton @cc="sum3" />
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="single-service" style="background: url(img/5.jpg);">
                <div class="overlay overlay-content justify-content-center">
                  <h1>
                    <i class="fas fa-hand-point-right text-secondary"></i>
                    {{total5}}
                    <i class="fas fa-hand-point-left text-secondary"></i>
                  </h1>
                  <CsButton @cc="sum4" />
                </div>
              </div>
            </div>

            <div class="col-md-6">
              <div class="single-service" style="background: url(img/6.jpg);">
                <div class="overlay overlay-content justify-content-center">
                  <h1>
                    <i class="fas fa-hand-point-right text-secondary"></i>
                    {{total6}}
                    <i class="fas fa-hand-point-left text-secondary"></i>
                  </h1>
                  <CsButton @cc="sum5" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import CsButton from "./components/CsButton.vue";

export default {
  name: "App",

  components: {
    HelloWorld,
    CsButton,
  },
  data: function () {
    return {
      total1: 0,
      total2: 0,
      total3: 0,
      total4: 0,
      total5: 0,
      total6: 0,
    };
  },

  methods: {
    sum(counterValue) {
      this.total1 = counterValue;
    },
    sum1(counterValue) {
      this.total2 = counterValue;
    },
    sum2(counterValue) {
      this.total3 = counterValue;
    },
    sum3(counterValue) {
      this.total4 = counterValue;
    },
    sum4(counterValue) {
      this.total5 = counterValue;
    },
    sum5(counterValue) {
      this.total6 = counterValue;
    },
  },
};
</script>

<style>
#app {
  font-family: "Itim", cursive;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
body {
  background-image: url("/img/111.jpg");
}
</style>
