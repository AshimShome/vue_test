<template>
    <h1>{{msgss}}</h1>
    <ChildPage name="Sadam ali dfdfdsfsdsddsf"/>

</template>
<script>
import ChildPage from './Child.vue'

export default {
  name: 'HomePage',
  components: {
    ChildPage
   
  },
  props: {
    msgss : String
  },
  data(){

  }
}

</script>
<style scoped>
h1{
    color: green;
}
</style>