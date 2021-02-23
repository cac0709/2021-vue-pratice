<template>
  <div class="praticetext">

   <h3>練習4567890</h3>
   <h3>
     單價:{{ price }}元,
     數量:{{ qulity }}個,
     總價:{{ price*qulity }}元 
   </h3>
   <!-----V-MODEL綁定-------->
   <p>假設 1 日幣 = 0.278 台幣</p>
  <div>台幣 <input type="text" v-model="twd" v-on:input="twd2jpy"></div>
  <div>日幣 <input type="text" v-model="jpy" v-on:input="jpy2twd"></div>
  </div>
  
  <div>
     鉛筆: 
    <input type="text" v-model.trim="pen" >根
    <p>鉛筆共{{ pen }} 根</p> 
  </div>

</template>
<script>
 export default {
 name:'praticetex',
  data() {
      return {
        twd:'1',
        jpy:'0.278',
        pen:''
      }
  },
    methods: {
    twd2jpy(){
    this.jpy = Number.parseFloat(Number(this.twd) / 0.278).toFixed(3);
    },
    jpy2twd(){
    this.twd = Number.parseFloat(Number(this.jpy) * 0.278).toFixed(3);
    },
  },
   
   props: {
    price: String,
    qulity:String,
  }
  
 }
</script>


<style scoped lang="scss">
h3 {
  margin: 60px 0 0;
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
p{
  color: red;
  margin-right: 4;
  position: right;
}
</style>
