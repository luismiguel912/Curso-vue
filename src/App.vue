<template>
  <div>
  <Car/>
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
}
</script>

<style>

</style>