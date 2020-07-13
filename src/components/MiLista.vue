<template>

<div id="central">
    <h3>{{ title }}</h3>
    <ul>
        <li v-for="(item, i) in items" v-bind:key="i"><a href="item.url"> {{item.texto}} </a> </li>
    </ul>

</div>
    
</template>

<script>
export default {
    name: "MiLista",
    el: "#central" ,
    props:  {
        title: String,
        items: Array
        },
    data:function(){
        return {
            Nombre:'Verona',
            msg: 'Bienvenid@s usuari@s'
        }   
    }
}
</script>

<style scoped>

    #central{
        background-color: #1b0522;
        color:white;
        padding:2%;
    }

    h3 {
        color:goldenrod;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li{
        list-style: none;
        display: inline-block;
        margin: 5px 10px;
    }

    a {
    color: #42b983;
    }

</style>