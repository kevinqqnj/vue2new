<template>
    <div id="secondcomponent">
        <h1>I'm 2nd page</h1>
        <ul>
            <span v-for="article in articles">
            <img :src="article.images.medium"><span v-text="article.title"></span>
        </span>
        </ul>
    </div>
</template>
<style>
    #secondcomponent {
        /*border-style: dashed;*/
        /*border-width: 1.5px;*/
        /*border-color: darkgreen;*/
        background-color: bisque;
        /*left: 20%;*/
        /*position: absolute;*/
    }

</style>
<script>
//    import HeaderComponent from './components/header.vue'
//    import OtherComponent from './components/other.vue'
    export default{
        data(){
            return{
                author: "Kevin",
                articles: []
            }
        },
        mounted: function () {
            this.$http.jsonp('https://api.douban.com/v2/movie/top250?count=10', {}, {
                headers: {

                },
                emulateJSON: true
            }).then(function(response) {
                // 这里是处理正确的回调

                this.articles = response.data.subjects
                // this.articles = response.data["subjects"] 也可以

            }, function(response) {
                // 这里是处理错误的回调
                console.log(response)
            });

        }
//        components:{
//            'other-component':OtherComponent,
//            HeaderComponent,
//        }
    }
</script>
