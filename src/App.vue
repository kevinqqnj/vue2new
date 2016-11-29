<template>
    <div id="app">
        <mu-flexbox>
            <mu-flexbox-item gutter="0">
                <firstcomponent></firstcomponent>
            </mu-flexbox-item>
        </mu-flexbox>
            <mu-flexbox>
            <mu-flexbox-item style="width:70%;">
                <cardcomp></cardcomp>
            </mu-flexbox-item>
            <mu-flexbox-item class="flex-demo">

                <li><router-link to="/first">跳转到第一页</router-link></li>
                <li><router-link to="/second">跳转到第二页</router-link></li>

            </mu-flexbox-item>

        </mu-flexbox>
        <mu-flexbox justify="center">
            <footercomponent></footercomponent>
        </mu-flexbox>

        <!--<img src="./assets/logo.png">-->
        <!--<h1>{{ msg }}</h1>-->
        <!--<input type="text" v-model="msg">-->

        <!--&lt;!&ndash;<secondcomponent></secondcomponent>&ndash;&gt;-->


        <div id="rightcontent">
        <router-view class="view"></router-view>
    </div>
        <div id="bottom">

        </div>
    </div>
</template>

<script>
    import firstcomponent from './components/firstcomponent.vue'
    import secondcomponent from './components/secondcomponent.vue'
    import footercomponent from './components/footercomponent.vue'
    import cardcomp from './components/cardcomp.vue'
        export default {
        name: 'app',
        data () {
            return {
                msg: 'Welcome to Vue.js 2.0 quickstart'
            }
        },
        components: {
            firstcomponent, footercomponent, secondcomponent, cardcomp
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
  /*margin-top: 60px;*/
}

#leftmenu {
    position: absolute;
    left: 0;
    width: 20%;

}
#rightcontent {
    position: absolute;
    left: 20%;
    width: 78%;
}
#bottom {
    left: 5%;
    position: absolute;
    width: 90%;
    top:95%;
}
h1, h2 {
  font-weight: normal;
}

a {
  color: #42b983;
}
</style>
