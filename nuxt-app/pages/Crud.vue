<template>
  <div class="ml-44">
    <table class="place-content-center border-2">
      <tr>
        <td>
          <label for="firstName"
            >First Name
            <input
              type="text"
              id="firstName"
              v-model="mydata.firstName"
              class="border-2"
            />
          </label>
        </td>
      </tr>
      <tr>
        <td>
          <label for="lasttName"
            >Last Name
            <input type="text" id="lastName" v-model="mydata.lastName" class="border-2" />
          </label>
        </td>
      </tr>
      <tr>
        <td>
          <label for="address"
            >Address
            <input type="text" id="address" v-model="mydata.address" class="border-2" />
          </label>
        </td>
      </tr>
      <tr>
        <td>
          <label for="city"
            >City <input type="text" id="city" v-model="mydata.city" class="border-2" />
          </label>
        </td>
      </tr>
      <tr>
        <td>
          <label for="hobby">Hobby <input type="checkbox" value="Cricket" /> </label>
        </td>
      </tr>
      <tr>
        <td>
          <label for="decription"
            >Description:
            <textarea
              v-mode="mydata.Discription"
              id="decription"
              class="border-2"
              cols=""
              rows=""
            ></textarea>
          </label>
        </td>
      </tr>
    </table>
    <button>submit</button>
  </div>
</template>
// <script setup lang="ts">
// let details = [];
let mydata = reactive({
  firstName: "",
  lastName: "",
  address: "",
  city: "",
  Discription: "",
});

// function save() {
//   console.log(details);
// }
</script>
