<template>
<h1>{{msgss}}</h1>
<ChildPage data="Sadam ali dfdfdsfsdsddsf"  />
<ul>
    <li v-for="item in users" :key="item.name" >
        <!-- {{item.name}}
        {{item.email}} -->
        <ReuseComponent :data="item" />

    </li>
</ul>
</template>

<script>
import ChildPage from './Child.vue'
import ReuseComponent from './ReuseComponent.vue'

export default {
    name: 'HomePage',
    props: {

    },
    components: {
        ChildPage,
        ReuseComponent
    },
    // props: {
    //   data : String
    // },
    data() {
        return {
            users: [{
                    name: "ashim",
                    email: "ashim@gmail"
                },
                {
                    name: "saddam",
                    email: "saddam@gmail"
                },
                {
                    name: "pobon",
                    email: "pobon@gmail"
                },
            ]
        }
    },
    methods: {
        getname: function (name) {
            alert(name);
        },
        getnamet: function () {
            alert("name");
        }

    }
}
</script>

<style scoped>
h1 {
    color: green;
}
</style>
