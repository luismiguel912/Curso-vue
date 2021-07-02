<template>
<div>
    <!-- <p>Marca: {{ brand }}</p> -->
    <!-- <p>
      <span v-for="color in color"  :key="color"> {{ color }}</span>
    </p> -->
    <!-- <ul v-for="color in color"  :key="color"> -->
      <!-- <li>{{ color }}</li>
    </ul>
    <ul v-for="powers in powers" :key="powers">
      <li v-if="powers > 50">{{ powers }}</li>
    </ul>
    <p>mensaje: {{ mensaje.text }}</p>  -->
    <hr>
    <h1>Tema Props</h1>
    <h1> Valor del props desde el padre: {{poder}}</h1>
</div>
</template>

<script>
export default {
  props: {
    poder: {
      type: Number,
      default: 60,
    },
  },
    // data() {
    //     return {
    //         brand: "nissan",
    //         color: ['red','blue','green','yellow'],
    //         mensaje: {
    //             title: "hola mundo",
    //             text: "gg"
    //         },
    //         powers: [10,120,30,40,50,60],
    //     };
    // },
    setup(props) {
      const hola = 1;
      console.log(props)
        
      return {
          hola,
      }
    },
};
</script>

<style>

</style>