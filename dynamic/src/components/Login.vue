<template>
  <div>
    <form>
      <label for="user">
        UserName:
        <input
          type="text"
          id="user"
          autofocus
          name="user"
          v-model="user"
          ref="user" /></label
      ><br />
      <label for="pass"
        >Password: <input type="password" id="pass" v-model="pass" /></label
      ><br />
      <button type="button" v-on:click="submit">Login</button>
    </form>
  </div>
</template>
<script>
export default {
  name: "logiN",
  data() {
    return {
      user: "",
      pass: "",
    };
  },
  methods: {
    submit(){
        if(this.user==''){
             alert("plz fill the fildes");
        }else{
        if (this.user=='swapnil'&&this.pass=='swapnil') {
            alert("hi" +this.user +'you login successfully ');
            
        }else{
            alert("Invalid User And Password")
        }
    }
    }
  },
};
</script>
<style scoped>
div {
  background-color: aqua;
  width: 40%;
  margin: auto;
  display: flex;
  justify-content: center;
}

button {
  margin: 20px;
  width: 50%;
  background-color: rgb(12, 107, 107);
}

input {
  margin: 20px;
  border: none;
  background-color: aqua;
}
</style>
