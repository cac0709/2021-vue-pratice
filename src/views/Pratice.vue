<template>
  <div class="pratice">
    <h1>Pratice</h1>   
     <Praticetext price="100" qulity="10" />
     

     
  </div>
</template>
<script>
// @ is an alias to /src
import Praticetext from '@/components/Praticetext.vue'

export default {
  name: 'Pratice',
  components: {
    Praticetext
  },



}
</script>
