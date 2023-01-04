<template>
    <h1>Child</h1>
    <p>{{name}}</p>
    <p>{{getname}}</p>
</template>
<script>

export default{
    name:'ChildPage',
  props: {
    name : String,
    getname :Function
  },
  components:{
    
  },
  data(){
    return{
      info:{
          name:'ashim',
          phone:'01613101011',
          age:29,
      }
    }

  }
}
</script>
