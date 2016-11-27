<template>
    <div id="footer">
        <hr>
        <p>This is footer</p>
        <a href="http://github.com/kevinqqnj">Github</a>
        <a>Copyright 2016, {{ author }}</a>
    </div>
</template>
<style>

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
