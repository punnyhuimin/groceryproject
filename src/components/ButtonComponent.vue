<template>
    <div id = "app">
        <button v-on:click = "inc"> + </button> 
        <p>{{counter}}</p>
        <button v-on:click = "dec" > - </button>
    </div>
</template>

<script>
export default {
    data(){
        return{
            counter:0
        }
    },
    methods:{
        dec: function(){
            if(this.counter>0)
                return this.counter--; else
                return this.counter;
        },
        inc: function(){
            if(this.counter<10)
                return this.counter++; 
            else
                alert('You cannot buy more than 10 items')
        }
    }
} </script>

<style scoped> 
header{
    background:rgb(122, 63, 100); 
    padding:10px;
    border-style: solid; 
    border-color:black; 
    border-width: 2px;
} 
button{
    background-color:rgb(145, 158, 190);
    font-size:25px; 
    border-radius: 10px; 
    text-align: center; 
    text-decoration: none; 
    display:inline-block; 
    padding:10px 30px;
} 
img{
    width:100px;
    height:100px; 
}
label{ 
    width:100px; 
    font-size: 30px;
}
</style>
