<template>

    <h2 style="font-size: 14px;">User Component</h2>
    <el-row>
        <el-button type="primary" v-on:click="getUser(userName)" round style=" padding: 10px 20px; border-radius: 100px; background: red; color: white; cursor: pointer;">Send User Name to Parent</el-button>
    </el-row>
    
</template>
<script>
export default {
    name: "user",
    data() {
        return {
            userName: "Kunal Pawar"
        }    
    },
    props:{
        getUser:Function
    }

}

</script>
