<template>
    <h1 style="font-style: italic; font-size: 23px; color: Green">User Name: {{name}}</h1>
    <User :getUser = "getUserName" />
</template>

<script>
import User from './user.vue'
export default {
    name: "home",
    data() {
        return {
            name: ''
        }
    },
    components:{
        User
    },
    methods: {
        getUserName(name) {
            this.name=name
        }
    }
}
</script>
