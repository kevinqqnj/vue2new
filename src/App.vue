<template>
    <div id="app">
        <img src="./assets/logo.png">
        <h1>{{ msg }}</h1>
        <input type="text" v-model="msg">
        <firstcomponent></firstcomponent>
        <!--<secondcomponent></secondcomponent>-->
        <ul>
            <li><router-link to="/first">跳转到第一页</router-link></li>
            <li><router-link to="/second">跳转到第二页</router-link></li>
        </ul>
        <router-view class="view"></router-view>
        <hr>
        <footer></footer>
</template>

<script>
    import firstcomponent from './components/firstcomponent.vue'
    import secondcomponent from './components/secondcomponent.vue'
    import footer from './components/footer.vue'
    export default {
        name: 'app',
        data () {
            return {
                msg: 'Welcome to Vue.js 2.0 quickstart'
            }
        },
        components: {
            firstcomponent, secondcomponent, footer
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

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
