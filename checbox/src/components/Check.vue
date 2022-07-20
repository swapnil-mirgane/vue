<template>
  <div>
    <input type="checkbox" name="check" v-model="sle" value="edit" id="edit" />
    <label for="edit">Edit</label>
    <input type="checkbox" name="check" v-model="sle" value="delete" id="delete" />
    <label for="edit">Edit</label>
    <input type="checkbox" name="check" v-model="sle" value="update" id="edit" />
    <label for="edit">Edit</label>
    <input type="checkbox" name="check" v-model="sle" value="remove" id="edit" />
    <label for="edit">Edit</label>
    <input type="checkbox" name="check" v-model="sle" value="select" id="edit" />
    <label for="edit">all</label>
  </div>
  <h1 v-for="item in sle" :key="item">{{item}} </h1>
</template>
<script>
export default {
    name:'selecT',
data() {
    return {
        sle:[],
    }
},
}
</script>
