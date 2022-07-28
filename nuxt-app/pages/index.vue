<template>
<div>
<table border="2"> 
<tr> <td><label for="userName">UserName</label></td><td><input type="text"  id='userName' v-model.lazys="loginDetails.userName" placeholder="UserName"></td></tr>
<tr><td><label for="pass">Password</label></td><td><input type="passowrd" v-model="loginDetails.pass" id="pass" placeholder="Enter the password"></td></tr>
</table>
<button @click="login">Login</button>
</div>
</template>
<script setup lang="ts">
const loginDetails=reactive({
    userName:'',
    pass:''
})
function login(){
 if (loginDetails.userName=='swapnil'&&loginDetails.pass=='swapnil'){
    alert("Login Successfull");
 location.href="http://localhost:3000/crud2";
    
 }else{
  alert("plz Enter User= swapnil  pass= swapnil");
 }  
}
</script>
