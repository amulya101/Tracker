<template>
    <button @click="add()" class="enterBtn">{{text}}</button>
</template>

<script>
export default {
    name: "Buttons",
    props:  {
        "text": String
    },

    methods : {
        add() {
            console.log("clicked add");
        }
    }
}
</script>

<style scoped>

.enterBtn {
    background: red;
    border-block-color: black;  
    font-size: 24px;
}

button:hover {
    background: white;
    border: solid;  
    border-block-color: black;
}


</style>>