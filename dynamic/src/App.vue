<template>
  <div>
    <h2>Welcome To Dynamic Components</h2>
    <!-- <login />
    <about></about>
    <home></home>
    <contact></contact> -->
    <div class="btn">
    <button @click="tab='about'" >About</button>
    <button @click="tab='home'" > Home </button>
    <button @click="tab='contact'" >Contact</button>
    <button @click="tab='login'" >Login</button>
    </div>
    <component :is="tab"/>

  </div>
</template>
<script>
import login from "./components/Login.vue";
import about from "./components/About.vue";
import home from "./components/home.vue";
import contact from "./components/Contact.vue";
export default {
  components: {
    login,
    about,
    home,
    contact,
  },
  data() {
    return {
      tab:'home'
    }
  },
};
</script>
<style scoped>
.btn{

  width: 100%;
  display:flex;
  justify-content:center;
}
button{
  width: 15%;
  margin: 10px;
  padding: 10px;
}
h2{
  text-align: center;
  font-size: xx-large;
}
</style>
