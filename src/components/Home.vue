<template>
    <h1>{{msgss}}</h1>
</template>
<script>
export default {
  name: 'HomePage',
  props: {
    msgss: String
  }
}

</script>
<style scoped>
h1{
    color: green;
}
</style>