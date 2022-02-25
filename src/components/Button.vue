<template>
<div>
<svg xmlns="http://www.w3.org/2000/svg" version="1.1" class="goo">
  <defs>
    <filter id="goo">
      <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur" />
      <feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 19 -9" result="goo" />
      <feComposite in="SourceGraphic" in2="goo"/>
    </filter>
  </defs>
</svg>

<span class="button--bubble__container">
  <a href="https://br.puma.com/chuteira-future-z-1-2-campo-masculina-106476-01.html?utm_source=GGL&utm_medium=PLA&utm_campaign=PLA_GGL_SSH_Smart-Shopping_BR&gclid=CjwKCAiA5t-OBhByEiwAhR-hmwELtGxrgtZUeshvV7T9kCsBX-sJo2RDovcQSj5qiHt3Q2d7s3wD9BoCNfoQAvD_BwE" class="button button--bubble" target="_blank">
    Confira
  </a>
  <span class="button--bubble__effect-container">
    <span class="circle top-left"></span>
    <span class="circle top-left"></span>
    <span class="circle top-left"></span>

    <span class="button effect-button"></span>

    <span class="circle bottom-right"></span>
    <span class="circle bottom-right"></span>
    <span class="circle bottom-right"></span>
  </span>
</span>
</div>  
</template>

<script>

</script>

<style lang="scss" scoped>
$dark-blue: #0093FA;
$green: #90feb5;
$action-color: $green;

* {
  box-sizing: border-box;
}

div {
  margin-left: 47%;
  margin-top: 5%;
  display: block;
  height: 100%;
  animation: hue-rotate 10s linear infinite;
}

.button {
  -webkit-font-smoothing: antialiased;
  background-color: $dark-blue;
  border: none;
  color: #fff;
  display: inline-block;
  font-family: "Montserrat", sans-serif;
  font-size: 14px;
  font-weight: 100;
  text-decoration: none;
  user-select: none;
  letter-spacing: 1px;
  color: white;
  padding: 20px 40px;
  text-transform: uppercase;
  transition: all 0.1s ease-out;

  &:hover {
    background-color: $action-color;
    color: #fff;
  }

  &:active {
    transform: scale(0.95);
  }

  &--bubble {
    position: relative;
    z-index: 2;
    color: white;
    background: none;

    &:hover {
      background: none;
    }

    &:hover + .button--bubble__effect-container .circle {
      background: darken($action-color, 15%);
    }

    &:hover + .button--bubble__effect-container .button {
      background: darken($action-color, 15%);
    }

    &:active + .button--bubble__effect-container {
      transform: scale(0.95);
    }

    &__container {
      position: relative;
      display: inline-block;

      .effect-button {
        position: absolute;
        width: 50%;
        height: 25%;
        top: 50%;
        left: 25%;
        z-index: 1;
        transform: translateY(-50%);
        background: $dark-blue;
        transition: background 0.1s ease-out;
      }
    }
  }
}

.button--bubble__effect-container {
  position: absolute;
  display: block;
  width: 200%;
  height: 400%;
  top: -150%;
  left: -50%;
  -webkit-filter: url("#goo");
  filter: url("#goo");
  transition: all 0.1s ease-out;
  pointer-events: none;

  .circle {
    position: absolute;
    width: 25px;
    height: 25px;
    border-radius: 15px;
    background: $dark-blue;
    transition: background 0.1s ease-out;

    &.top-left {
      top: 40%;
      left: 27%;
    }

    &.bottom-right {
      bottom: 40%;
      right: 27%;
    }
  }
}

.goo {
  position: absolute;
  visibility: hidden;
  width: 1px;
  height: 1px;
}

html,
body {
  width: 100%;
  height: 100%;
  text-align: center;
}

.button--bubble__container {
  top: 50%;
  margin-top: -25px;
}

@keyframes hue-rotate {
  from {
    -webkit-filter: hue-rotate(0);
    -moz-filter: hue-rotate(0);
    -ms-filter: hue-rotate(0);
    filter: hue-rotate(0);
  }
  to {
    -webkit-filter: hue-rotate(360deg);
    -moz-filter: hue-rotate(360deg);
    -ms-filter: hue-rotate(360deg);
    filter: hue-rotate(360deg);
  }
}

@media screen and (max-width:700px){
  div{
    padding-top: 4rem;
    margin-left: 7rem;
    margin-right: auto;
  }
}
</style>