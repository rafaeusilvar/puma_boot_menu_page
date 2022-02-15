<template>
  <div id=container>
  puma 
  <div id=flip>
    <div><div>lifeStyle</div></div>
    <div><div>Sprint</div></div>
    <div><div>New Levels</div></div>
  </div>
  Future 2.1
</div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css?family=Roboto:700');

body {
  font-family:'Roboto';
  text-align:center;
}

#container {
  color:#999;
  text-transform: uppercase;
  font-size:36px;
  font-weight:bold;  
  width:100%;
  bottom:45%;
  display:block;
  text-align: center;
  margin-top: 75px;
}

#flip {
  height:50px;
  overflow:hidden;
}

#flip > div > div {
  color:#fff;
  padding:4px 12px;
  height:45px;
  margin-bottom:45px;
  display:inline-block;
}

#flip div:first-child {
  animation: show 5s linear infinite;
}

#flip div div {
  background:#5BC2A7;
}
#flip div:first-child div {
  background: black;
}
#flip div:last-child div {
  background:#F92A83;
}

@keyframes show {
  0% {margin-top:-270px;}
  5% {margin-top:-180px;}
  33% {margin-top:-180px;}
  38% {margin-top:-90px;}
  66% {margin-top:-90px;}
  71% {margin-top:0px;}
  99.99% {margin-top:0px;}
  100% {margin-top:-270px;}
}

p {
  /* position:fixed; */
  width:100%;
  bottom:30px;
  font-size:12px;
  color:#999;
  /* margin-top:200px; */
}
</style>