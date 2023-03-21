<template>
    <img alt="Vue logo" src="../assets/logo.png">
    <h1>Name : {{firstName+" "+lastName}}</h1>
    <h2>Email :{{email}}</h2>
    <h2>Email :{{email=="razahmed163101@gmail.com"}}</h2>
    <h3>Age :{{getAge(21)}}</h3>
    <h4>Points {{points}}</h4>
    <button v-on:click="pluspoints()">Plus</button>
</template>

<script>
export default {
    name:"BasicComponenets",
    data(){
        return {
            firstName: "Raza",
            lastName: "Ahmed",
            email: "razahmed163101@gmail.com",
            
            points: 0
        }
    },
    methods:{
        getAge:function(age){
            return age
        },
        pluspoints:function(){
            this.points+=this.getAge(20);
        }
    }
}
</script>

<style>
#app{
    font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>