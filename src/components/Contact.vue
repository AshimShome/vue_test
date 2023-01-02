<template>
    <h1>Contact</h1>
    <h1>Contact-{{email}}</h1>
    <h1>Contact-{{mobile}}</h1>
    <h1>Contact-{{getname(10)}}</h1>
    <h1>Contact-{{10+10}}</h1>



</template>

<script>
export default {
  name: 'ContactPage',
  data(){
    return{
    email: "ashim@gmail.com",
    mobile: "01613101011",
    getname:function(a){
      return a
    }

    }
  }
 
}
</script>
<style >
h1{
    color: orange;
}
</style>