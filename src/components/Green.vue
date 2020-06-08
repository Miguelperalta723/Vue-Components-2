<template>
    <div>
        <h1>Green</h1>
        <button @click="counter++">Add</button>
        <p>{{ counter }}</p>
    </div>
</template>

<script>
export default {
   data: function(){
       return {
           counter: 0
       }
   },
   destroyed(){
       console.log("destroyed")
   }
}
</script>

<style scoped>
    div {
        border: 1px solid #ccc;
        box-shadow: 1px 1px 1px black;
        padding: 30px;
        margin: 30px auto;
        text-align: center;
    }

  
</style>