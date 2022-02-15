<template>
    <div>
      <Menu />
      <Parallax />
      <Title />
      <Main />
      <Button />
      <ParallaxMain/>
      <TitleTwo/>
      <Card />
      <!-- <Github /> -->
    </div>
</template>


<script>

// import Github from './components/Github.vue';
import Menu from './components/Menu.vue';
import Parallax from './components/Parallax.vue';
import Main from './components/Main.vue';
import Title from './components/Title.vue';
import Button from './components/Button.vue';
import ParallaxMain from './components/ParallaxMain.vue';
import Card from './components/Card';
import TitleTwo from './components/TitleTwo.vue';

export default {
  name: 'app',
  components: {
    Menu,
    Parallax,
    Main,
    Title,
    Button,
    ParallaxMain,
    Card,
    TitleTwo,
    // Github,
  }
};
</script>

<style >
  body { 
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  }
</style>