<template>
    <div id="footer">
        <a href="http://github.com/kevinqqnj">Github</a>
        <a>Copyright 2016, {{ author }}</a>
    </div>
</template>
<style>
    body{
        /*background-color:#ff0000;*/
    }
</style>
<script>
//    import HeaderComponent from './components/header.vue'
//    import OtherComponent from './components/other.vue'
    export default{
        data(){
            return{
                author: "Kevin ZQ"
            }
        }
//        components:{
//            'other-component':OtherComponent,
//            HeaderComponent,
//        }
    }
</script>
