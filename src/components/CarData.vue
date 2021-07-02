<template>
<div>
  <h1>hola mundo data</h1>
    <p>Marca : {{ marca}}</p>
    <p>Modelo: {{ modelo}}</p>
    <p>Fuerza: {{ caballos}}</p>
    <button @click="subir">Aumentar</button>
    <button @click="disminuir">Disminuir</button>
</div>
</template>

<script>
export default {
    data() {
        return {
            marca: 'nisan',
            modelo: 'mx',
            caballos: 9,        
            };
    },
    methods: {
        subir() {
            if(this.caballos <=10){

                this.caballos = this.caballos + 1;
            }
        },
        disminuir() {
            if(this.caballos > 0){

                this.caballos = this.caballos - 1;
            }
        },
    }
}
</script>

<style>

</style>