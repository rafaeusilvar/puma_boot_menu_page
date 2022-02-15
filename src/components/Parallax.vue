<template>
<div class="parallax"></div>
<!--  

  <v-parallax
    dark
    class="d-flex"
     height="800"
    src="https://mir-s3-cdn-cf.behance.net/project_modules/max_1200/cd0f55124619575.610822c59c496.png"
  >
    <v-row
      align="center"
      justify="center"
    >
      <v-col
        class="text-center"
        cols="12"
      >
      </v-col>
    </v-row>
  </v-parallax>
-->
</template>

<style scoped>
.parallax {
background-image: url("https://mir-s3-cdn-cf.behance.net/project_modules/1400_opt_1/dc967d67591063.5b3ec885d4194.jpg");
/* margin-top: -10px; */
min-height: 670px;
background-attachment: fixed;
background-position: center;
background-repeat: no-repeat;
background-size: cover;
}

@media screen and (max-width:700px){
  .parallax{
    min-height: 30px;
  }
}
</style>