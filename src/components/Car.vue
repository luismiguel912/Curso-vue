<template>
<div>
    <p>Marca: {{ brand }}</p>
    <!-- <p>
      <span v-for="color in color"  :key="color"> {{ color }}</span>
    </p> -->
    <ul v-for="color in color"  :key="color">
      <li>{{ color }}</li>
    </ul>
    <ul v-for="powers in powers" :key="powers">
      <li v-if="powers > 50">{{ powers }}</li>
    </ul>
    <p>mensaje: {{ mensaje.text }}</p> 
</div>
</template>

<script>
export default {
    data() {
        return {
            brand: "nissan",
            color: ['red','blue','green','yellow'],
            mensaje: {
                title: "hola mundo",
                text: "gg"
            },
            powers: [10,120,30,40,50,60],
        };
    },

    // setup() {
    //      const d = "hsola";
    //      const g = 1;
        
    //     return {
    //         d,g,
    //     }
    // },
};
</script>

<style>

</style>