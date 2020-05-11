<template>

  <div id="Search">
  <marquee>
    <h1>Type the number for finding out the cube:</h1>
</marquee>
	<input v-model="query">
	  <button v-on:click="handleSubmit">Enter</button>
    
	<p> </p>
</div>
</template>
<script>
export default {
  name: 'Search',
  data () {
    return {
      query:''
  }
 },
 methods:{
 handleSubmit: 
 
 function(){
 if(isNaN(this.query)){
 alert("not a valid number");
 }
 else
 alert("the cube of the number is   " +this.query*this.query*this.query);
 
 }
 }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight:  very large;
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
  color: green;
}
</style>
