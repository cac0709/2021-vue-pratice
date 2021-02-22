<template>
  <div class="pratice">

   <h3>練習4567890</h3>
   <h3>
     單價:{{ price }}元,
     數量:{{ qulity }}個,
     總價:{{ price*qulity }}元
   </h3>
  </div>
</template>
<script>
export default {
  name: 'Praticetext',
  props: {
    price: String,
    qulity:String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
