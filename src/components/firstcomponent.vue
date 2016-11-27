<template>
    <div id="firstcomponent">
        <h1>I'm 1st component</h1>
        <a>written by {{ author }}</a>
    </div>
</template>
<style>
    #firstcomponent {
        /*border-style: dashed;*/
        /*border-width: 1.5px;*/
        /*border-color: lightsalmon;*/
        background-color: #ccc;
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
