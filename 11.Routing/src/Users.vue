<template>
    <div>
        <h1>User Page</h1>
        <p>User Id id:{{$route.params.userId}}</p>
        <button @click="goHome">Go home</button>
    </div>
</template>
<script>
    export default{
        watch: {
            '$route' (to, from){
                alert(to.params.userId);
            }
        },
        created(){
            alert(this.$route.params.userId);
        },
        methods: {
            goHome(){
                this.$router.push("/");
            }
        }
    }
</script>