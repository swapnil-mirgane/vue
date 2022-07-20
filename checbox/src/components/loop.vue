<template>
<div>
<ul>
    <li v-for="item in arr" :key="item" >{{item}}</li>
</ul>
</div>
</template>
<script>
export default {
    name:'looP',
    data() {
        return {
            arr:['swapnil','kunal','rohit','ganesh'],
        }
    },
}
</script>
<style scoped>

</style>