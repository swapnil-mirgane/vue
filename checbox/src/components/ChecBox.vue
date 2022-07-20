<template>
<div>
<input type="radio" v-model="gender" name="gen" value="Male" id="male"> <label for="male">Male</label>
<input type="radio" v-model="gender" name="female" value="Female" id="female"><label for="female">Female</label>
<h1>selected Gender is {{gender}}</h1>
</div>
</template>
<script>
export default {
    name:'geN',
    data(){
        return{
            gender:null,
        }
    }

}
</script>