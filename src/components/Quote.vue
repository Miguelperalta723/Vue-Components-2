<template>
    <div>
        <div>
            <slot></slot>
        </div>
        
    </div>
</template>

<script>
export default {
    props: ['quote']
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