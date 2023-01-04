<template>
<div class="red">
<h1>ReuseComponent.vue</h1>    
<h2>{{data.name}}</h2>
<h2>{{data.email}}</h2>
<button v-on:click="getnamet()">Aleart Name</button>
</div>
</template>
<script>
export default {
   name:'ReuseComponent',
   props: {
     data:Object,
    }

}
</script>
