<template>
    <div id="firstcomponent">
        <h1>I'm 1st component</h1>
        <a>written by {{ author }}</a>
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
