<script setup>
import HOME from './components/Home.vue'
import FOOTER from './components/footer.vue'
import BUTTON from "./components/Button.vue"
</script>

<template>
  <div class="background">  
    <div class="container green"></div>
    <div class="container blue"></div>

</div>


  <div>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/uphasia_logo.png" class="logo" alt="Vue logo" />
    </a>
  </div>
  <HOME/>
  <BUTTON/>
  <FOOTER/>

</template>

<style scoped>
.background{
  
  position: absolute;
  z-index: 2;
  width: 100vw;
  height: 100;
  background-color: #f5f5f7;
  filter: blur(100px);

}
.container{
  z-index: 1;
  width: 300px;
  right: 0;
  top: -20px;
  height: 300px;
  position: absolute;
  border-radius: 100%;
  /* box-shadow: 0px 0px 1000px #17aa7b8d; */

}
.blue{
background-color: #0005AF;
animation-name: container_blue;
animation-duration: 12s;
  animation-iteration-count: infinite;

}
.green{
  background-color: #17aa7b9a;
  animation-name: container_green;
  animation-duration: 5s;
  animation-iteration-count: infinite;

}
.logo {
  margin-top: 20px;
  height: 7em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
@keyframes container_green {
  0% { 
    opacity: 0.3; 
    right: 10%;
  top: -20%;
  scale: 1.0;
}
  40% { 
    opacity: 0.8; 
    right: 0%;
  top: -10%;
  scale: 0.5;

}
  60% { 
    opacity: 0.5; 
    right: 5%;
   top: 20%;
   scale: 0.3;

}
  100% { 
    opacity: 0.3; 
    right: 10%;
    top: -20%;
    scale: 1.0;

}
}


@keyframes container_blue {
  0% { 
    opacity: 0.2; 
    left: 10%;
  bottom:  50%;
  scale: 1.0;
}
  40% { 
    opacity: 0.3; 
    left: 0%;
  top: -10%;
  scale: 0.5;

}
  60% { 
    opacity: 0.1; 
    left: 5%;
   top: 20%;
   scale: 0.3;

}
  100% { 
    opacity: 0.2; 
    left: 10%;
    top: -20%;
    scale: 1.0;

}
}
</style>
