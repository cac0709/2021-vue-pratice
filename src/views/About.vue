<template>
  <div class="about">
    <h1>This is an about page</h1>
     <img alt="aboutimage" src="../assets/hotpot.jpg">
     <Traing/>
     
  </div>
</template>

<script>
// @ is an alias to /src
import Traing from '../components/Traing.vue'

export default {
  name: 'About',
  components: {
    Traing
    
  }
}
</script>