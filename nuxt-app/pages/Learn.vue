<template>
<h1>my name is  {{name}}
</h1>
<input type="text"  v-model="mydata.firstName" placeholder="first name"> 
<input type="text" v-model="mydata.lastname" placeholder="last name">
<input type="text" v-model="mydata.address" placeholder="enter the city">
<h2>my name is {{mydata.lastname +'     '+ mydata.firstName}} and i am from {{mydata.address}}</h2>
<button @click="change">change</button>
</template>
<script setup lang="ts" >
let name='mirgane';
// let firstName=ref("");

const mydata=reactive({
    firstName:'',
    lastname:'',
    address:''
});
function change(){

    
    
}
</script>