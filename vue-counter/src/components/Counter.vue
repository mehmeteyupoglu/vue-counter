<template>
  <b-container class="bv-example-row">
  <b-row>
    <b-col>
      <h1> {{ counterValue }}</h1>
      <b-button @click="decrement" variant="danger">Decrement</b-button>
      <b-button @click="increment" variant="success">Increment</b-button>
      
    </b-col>
  </b-row>
</b-container>
</template>

<script>
export default {
  name: 'Counter', 
  data(){
    return {
      counterValue : 0
    }
  }, 
  methods: {
    increment(){
      this.counterValue++
    }, 
    decrement(){
    if(this.counterValue >= 1){
      this.counterValue--
    } else {
      this.counterValue
    }
    
    } 
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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

button {
  margin: 0 10px; 
}
</style>
