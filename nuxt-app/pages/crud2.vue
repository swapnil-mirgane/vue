<template>
  <div class="ml-44">
  
      <table border="2" class="place-content-center border-2">
        <tr>
          <td>
            <label for="firstName"
              >First Name <input type="text" id="firstName" v-model="mydata.firstName" class="border-2" />
            </label>
          </td>
        </tr>
        <tr>
          <td>
            <label for="lasttName"
              >Last Name <input type="text" id="lastName" v-model="mydata.lastName" class="border-2" />
            </label>
          </td>
        </tr>
        <tr>
          <td>
            <label for="gender"
              >Gender :
              <input
                type="radio"
                id="gender"
                name="gender"
                class="border-2"
                value="Male"
              />Male
              <input
                type="radio"
                id="gender"
                name="gender"
                class="border-2"
                value="Female"
              />Female</label
            >
          </td>
        </tr>
        <tr>
          <td>
            <label for="address"
              >Address <input type="text"  id="address" v-model="mydata.address" class="border-2" />
            </label>
          </td>
        </tr>
        <tr>
          <td>
            <label for="city">City <input type="text" id="city" v-model="mydata.city" class="border-2" /> </label>
          </td>
        </tr>
        <tr>
          <td>
            <label for="hobby">Hobby <input type="checkbox" value="Cricket"/> </label>
          </td>
        </tr>
        <tr>
          <td>
            <label for="decription"
              >Description:
              <textarea id="decription" v-model="mydata.description" class="border-2"  cols="" rows=""></textarea>
            </label>
          </td>
        </tr>
      </table>
      <div><button @click="add">Save</button></div>
  </div>
</template>
<script setup lang="ts">
let firstName=''
let lastName=''
let address=''
let city=''

let mydata=reactive({
  firstName:'',lastName:'',address:'',city:'',gender:'',description:''
})
let add=()=>{
console.log(mydata);

}

</script>