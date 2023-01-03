<template>
<h1 v-if="show">if condition</h1>
<h1 v-else>else condition</h1>
<button v-on:click="show=!show">ck</button>
<h1>{{tech}}</h1>
<label for="Java">Java</label>
<input type="checkbox" id="Java" value="Java" v-model="tech">
<label for="C++">C++</label>
<input type="checkbox" id="C++" value="C++" v-model="tech">
<label for="node">Java</label>
<input type="checkbox" id="node" value="node" v-model="tech">
<br/><br/><br/>
<h1>{{gender}}</h1>
<label for="Man">Man</label>
<input type="radio" id="Man" value="Man" name="gender" v-model="gender">
<label for="Female">Female</label>
<input type="radio" id="Female" value="Female" name="gender" v-model="gender">


<br/><br/><br/>

<h1>Contact</h1>
<h1>Contact-{{email}}</h1>
<h1>Contact-{{mobile}}</h1>
<h1>Contact-{{getname(10)}}</h1>
<h1>Contact-{{10+10}}</h1>
<h1>Contact-{{getval("saddam")}}</h1>
<h1>Contact-{{getval("champuk")}}</h1>
<button v-on:click="test()">click me </button>
<h2>{{count}}</h2>
<input type="test" v-model="count2">
<h2>{{count2}}</h2>


<input type="test" v-model="email2" placeholder="email">
<input type="password" v-model="password" placeholder="password">
<button v-on:click="getdada()">click me for details </button>

</template>

<script>
export default {
    name: 'ContactPage',
    data() {
        return {
            email: "ashim@gmail.com",
            mobile: "01613101011",
            count: 0,
            getname: function (a) {
                return a
            },
            count2: 0,
            email2: null,
            password: null,
             tech:[],
             gender:null,
             show:true
        }
        
    },
    methods: {
        getval(a) {
            return a
        },
        test() {
            this.count = this.count + 1
        },
        getdada() {
        //  alert(this.password,this.email2);
        console.warn(this.password,this.email2);
        }
    }

}
</script>



<style scoped>
h1 {
    color: orange;
}
</style>
