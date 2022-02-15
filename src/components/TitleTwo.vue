<template>
  <div>
    <p id="title">FUTURE PUMA</p>
  </div>
</template>
<style scoped>
#title {
  text-align: center;
  margin-top: 5%;
  position: relative;
  font-family: sans-serif;
  text-transform: uppercase;
  font-size: 2em;
  letter-spacing: 4px;
  overflow: hidden;
  background: linear-gradient(90deg, #5BC2A7, #fff, #F92A83);
  background-repeat: no-repeat;
  background-size: 80%;
  animation: animate 3s linear infinite;
  -webkit-background-clip: text;
  -webkit-text-fill-color: rgba(255, 255, 255, 0);
}
#italy{
  text-align: center;
  padding-top: 5%;
  padding-left: 5%;
  padding-right: 5%;

}

@keyframes animate {
  0% {
    background-position: -500%;
  }
  100% {
    background-position: 500%;
  }
}
</style>