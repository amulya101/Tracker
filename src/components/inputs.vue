<template>
    <div class="funtions">
        <h1 > {{intro}} </h1>
        <p> This is a new component </p>
        <label> Inputs </label>
        <div class="txtBox" >
            <input type="text"> 
            
        </div>   
    </div>
    <div class="btn">
        <Buttons text="Add"/>
        <Buttons text="Edit"/>
        <Buttons text="Delete"/>
    </div>
</template>

<script>
import Buttons from './buttons.vue'

export default {
  components: { Buttons },
    name: "Inputs",
    props : {
        intro: String

    }    
}
</script>

<style scoped>
.funtions{
    font-family: 'Courier New', Courier, monospace;
    border: 3px solid red;
    width: 100%;
    text-align: center;   
    display: flex;
    flex-direction: column;
    margin: 10px 2px 10px 2px;
    
}

.txtBox{
    width: 100%;
    display: flex;
    justify-content: center;
    flex-direction: row;
    padding: 10px 10px 10px 10px
}



.btn {
    justify-content: center;
    display: flex;
    flex-direction: row;
    background-color: dodgerblue;

}

</style>>