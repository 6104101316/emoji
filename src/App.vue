<template>
  <div id="app">
    <div class="container">
      <h1>Kurama</h1>
      <div id="myCarousel" class="carousel slide" data-ride="carousel">
        <ol class="carousel-indicators">
          <li data-target="#myCarousel" data-slide-to="0" class></li>
          <li data-target="#myCarousel" data-slide-to="1" class="active"></li>
          <li data-target="#myCarousel" data-slide-to="2" class></li>
        </ol>
        <div class="carousel-inner">
          <div class="carousel-item">
            <img :src="img[0].src" class="img-fluid" />
          </div>
          <div class="carousel-item active">
            <img :src="img[1].src" class="img-fluid" />
          </div>
          <div class="carousel-item">
            <img :src="img[2].src" class="img-fluid" />
          </div>
          <a class="carousel-control-prev" href="#myCarousel" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
          </a>
          <a class="carousel-control-next" href="#myCarousel" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
          </a>
        </div>
      </div>
    </div>
    <div class="container">
      <hr class="featurette-divider" />
      <div class="row featurette alert alert-warning" style="opacity: 0.9; ">
        <div class="row align-items-center">
          
          <div class="col-6">
            <img :src="img[0].src" class="img-fluid" />
          </div>
          <div class="col-6">
            <!-- 2.รับค่าจาก emit @cc แล้วส่งไปทำงานใน function "sum"-->
            <emj label @cc="sum" />
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <hr class="featurette-divider" />
      <div class="row featurette alert alert-warning" style="opacity: 0.9; ">
        <div class="row align-items-center">
          <div class="col-6">
            <img :src="img[1].src" class="img-fluid" />
          </div>
          <div class="col-6">
            <!-- 2.รับค่าจาก emit @cc แล้วส่งไปทำงานใน function "sum"-->
            <emj label @cc="sum" />
          </div>
        </div>
      </div>
    </div>
    <div class="container">
      <hr class="featurette-divider" />
      <div class="row featurette alert alert-warning" style="opacity: 0.9; ">
        <div class="row align-items-center">
          
          <div class="col-6">
            <img :src="img[2].src" class="img-fluid" />
          </div>
          <div class="col-6">
            <!-- 2.รับค่าจาก emit @cc แล้วส่งไปทำงานใน function "sum"-->
            <emj label @cc="sum" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

import emj from "./components/emj.vue";

export default {
  name: "App",
  components: {
    emj,
  },

  data: function () {
    return {
      img: [
        {
          src:
            "https://i.pinimg.com/originals/9a/44/16/9a4416988b6e99e0692f5d5391528626.png",
        },
        {
          src:
            "https://vignette.wikia.nocookie.net/naruto/images/8/86/Kurama_ep.png/revision/latest?cb=20130830000612",
        },
        {
          src:
            "https://vignette.wikia.nocookie.net/naruto/images/0/08/Kurama_teams_up.png/revision/latest?cb=20130905155937",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  margin-top: 60px;
}
body{
  background-image: url(https://image.winudf.com/v2/image/Y29tLmFuZHJvbW8uZGV2NzE3NDMwLmFwcDgwOTYzNV9zY3JlZW5fMF8xNTMwMTUzNDg4XzA3OQ/screen-0.jpg?fakeurl=1&type=.jpg);
}
</style>
