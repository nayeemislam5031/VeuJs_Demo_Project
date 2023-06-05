
<template>
  
  <h1>{{ title }} </h1>
  <input type="text" ref="name">
  <button @click="handleclick" >click me</button>
  <Model :header="header" :text="text" />
  
</template>

<script >
import Model from "./components/Model.vue"


export default {
  name:'App',
  components:{Model},
  data(){
    return{
      title:"This is the Vue :) ",
      header: " Sign Up for the GatWay!",
      text: "Grave your ninja swag for half price"
    }
  },
  methods: {
    handleclick() {
      console.log(this.$refs.name);
      this.$refs.name.classList.add('active');
      this.$refs.name.focus()
    }
  },

}

</script>

<style scoped >

h1{
  text-align: center;
  color: whitesmoke;
  display: inline-block;
  border-bottom: 1px solid #ddd;
  padding-bottom:10px; 
  font-size:large;
}
.active{
  background-color: rgb(218, 224, 218);
  /* color: white; */
}


</style>
