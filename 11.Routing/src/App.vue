<template>
    <div id="app">
        <h1>{{ msg }}</h1>
        <hr/>
        <router-link to="/">Home</router-link>
        <router-link to="/users/13">Users 13</router-link>
        <router-link to="/users/10">Users 10</router-link>
        <hr/>
        <router-view></router-view>
    </div>
</template>

<script>
    export default {
        name: 'app',
        data () {
            return {
                msg: 'Welcome to Your Vue.js App'
            }
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
