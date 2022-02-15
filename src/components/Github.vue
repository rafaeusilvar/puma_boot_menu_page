<template>
   <div class="user" >
     <div>PERFIL Github</div>
     <div class="image">
       <a href="https://github.com/rafaeusilvar" target="_blank"> 
       <img :src="user.avatar_url"/>
       </a>
     </div>
     <div class="name">
       {{ user.login }}
     </div>
   </div>
  </template>
  <script>
  import axios from "axios";

  export default {
   name: "User",
   data() {
     return {
       user: {},
     };
   },
   created() {
     this.getUser();
   },
   methods: {
     getUser() {
       axios
         .get("https://api.github.com/users/rafaeusilvar")
         .then((res) => {
           this.user = res.data;
         })
         .catch((error) => {
           console.log(error);
         });
     },
   },
  };
  </script>

<style>
.user {
  text-align: center;  
  color: white;
}
.image{
  size: 10px;
}
</style>