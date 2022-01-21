<template>

<h1> Get input field value</h1>
<input type="text" placeholder ="email"  v-model="email"/>
<br/>
<br/>
<input type="password" placeholder ="password" v-model="password" />

<br/>
<br/>
<button v-on:click="getData()" type="button">Click me</button>
 </template>

<script> 

export default {
    name: "Home",
    data(){
      return{
        email:null,
        password:null,
      }
    },
    methods: {
    getData()
    {

      console.warn("function called values are", this.email, this.password)

    },
    }

   }


  </script>
  <style scoped> 
  h1{
  color: orange
  }
  
  
  </style>