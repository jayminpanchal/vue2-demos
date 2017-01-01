<template>
    <div>
        <h1>User Page</h1>
        <p>User Id id:{{$route.params.userId}}</p>
        <button @click="goHome">Go home</button>
    </div>
</template>
<script>
    export default{
        methods: {
            goHome(){
                this.$router.push("/");
            }
        }
    }
</script>