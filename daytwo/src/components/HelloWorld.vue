<template>
  <div class="hello">
    <p v-for="(item,index) in list" @click="fun">{{item}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      list:[1,2,3,4,5]
    }
  },
  methods:{
    fun(){
      for(let i=0;i<this.list.length;i++){
console.log(this.list[i])
    }
    
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
