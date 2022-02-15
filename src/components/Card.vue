<template>
  <div class="container">
  <div class="card card0">
    <div class="border">
      <h2></h2>
      <div class="icons">
        <i class="fa fa-codepen" aria-hidden="true"></i>
        <i class="fa fa-instagram" aria-hidden="true"></i>
        <i class="fa fa-dribbble" aria-hidden="true"></i>
        <i class="fa fa-twitter" aria-hidden="true"></i>
        <i class="fa fa-facebook" aria-hidden="true"></i>
      </div>
    </div>
  </div>
  <div class="card card1">
    <div class="border">
      <h2></h2>
      <div class="icons">
        <i class="fa fa-codepen" aria-hidden="true"></i>
        <i class="fa fa-instagram" aria-hidden="true"></i>
        <i class="fa fa-dribbble" aria-hidden="true"></i>
        <i class="fa fa-twitter" aria-hidden="true"></i>
        <i class="fa fa-facebook" aria-hidden="true"></i>
      </div>
    </div>
  </div>
  <div class="card card2">
    <div class="border">
      <h2></h2>
      <div class="icons">
        <i class="fa fa-codepen" aria-hidden="true"></i>
        <i class="fa fa-instagram" aria-hidden="true"></i>
        <i class="fa fa-dribbble" aria-hidden="true"></i>
        <i class="fa fa-twitter" aria-hidden="true"></i>
        <i class="fa fa-facebook" aria-hidden="true"></i>
      </div>
    </div>
  </div>
</div>
</template>
<style scoped>
.container {
  height: 100vh;
  width: 100vw;
  max-height: 800px;
  max-width: 1280px;
  min-height: 600px;
  min-width: 1000px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: 0 auto;
}
.border {
  height: 369px;
  width: 290px;
  background: transparent;
  border-radius: 10px;
  transition: border 1s;
  position: relative;
}
.border:hover {
  border: 1px solid #fff;
}
.card {
  height: 379px;
  width: 300px;
  background: #808080;
  border-radius: 10px;
  transition: background 0.8s;
  overflow: hidden;
  background: #000;
  box-shadow: 0 70px 63px -60px #000;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
.card0 {
  background: url("https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/df978967591063.5b3ec885d1053.jpg") center center no-repeat;
  background-size: 300px;
  cursor: pointer;
}
.card0:hover {
  background: url("https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/df978967591063.5b3ec885d1053.jpg") center center no-repeat;
  background-size: 600px;
}
.card0:hover h2 {
  opacity: 1;
}
.card0:hover .fa {
  opacity: 1;
}
.card1 {
  background: url("https://static.netshoes.com.br/produtos/chuteira-campo-puma-future-21-netfit-fg/91/D14-5116-191/D14-5116-191_zoom1.jpg?ts=1611238131&") center center no-repeat;
  background-size: 300px;
  cursor: pointer;
}
.card1:hover {
  background: url("https://static.netshoes.com.br/produtos/chuteira-campo-puma-future-21-netfit-fg/91/D14-5116-191/D14-5116-191_zoom1.jpg?ts=1611238131&") center center no-repeat;
  background-size: 600px;
}
.card1:hover h2 {
  opacity: 1;
}
.card1:hover .fa {
  opacity: 1;
}
.card2 {
  background: url("https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/573ba167591063.5b3ec885d493c.jpg") center center no-repeat;
  background-size: 300px;
  cursor: pointer;
}
.card2:hover {
  background: url("https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/573ba167591063.5b3ec885d493c.jpg") center center no-repeat;
  background-size: 600px;
}
.card2:hover h2 {
  opacity: 1;
}
.card2:hover .fa {
  opacity: 1;
}
h2 {
  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  color:#00A5E1;
  margin: 20px;
  opacity: 0;
  transition: opacity 1s;
}
.fa {
  opacity: 0;
  transition: opacity 1s;
}
.icons {
  position: absolute;
  fill: #fff;
  color: #fff;
  height: 130px;
  top: 226px;
  width: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}

</style>