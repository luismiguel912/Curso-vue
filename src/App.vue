<template>
  <div>
  <Car :poder="poder"/>
    <hr>
  <CarData/>
  </div>
</template>

<script>
import Car from "./components/Car"
import CarData from "./components/CarData.vue"
export default {
  components: {
    Car,
    CarData,
  },
  data() {
      return {
          poder: 20,
      };
  },
}
</script>

<style>

</style>