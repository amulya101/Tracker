<template>
    <nav class="top">
       <button> {{first}} </button>
       <button> {{second}} </button>
    </nav>
</template>

<script>
export default {
    name: "Nav",
    props: {
        first: {
            type : String,
            default : "Hello"
        },
        second: String
    }    
}
</script>

<style scoped>
.top{
    display: flex;
    font-size: 10px;
    justify-content: center;
    padding-bottom: 10px;
}

</style>>