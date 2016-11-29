<template>
    <div id="firstcomponent">
        <mu-appbar title="Vue2new">
            <mu-icon-button icon="menu" slot="left"/>
            <mu-icon-menu icon="more_vert" slot="right">
                <mu-menu-item title="菜单 1"/>
                <mu-menu-item title="菜单 2"/>
                <mu-menu-item title="菜单 3"/>
                <mu-menu-item title="菜单 4"/>
                <mu-menu-item title="菜单 5"/>
            </mu-icon-menu>
        </mu-appbar>
            <!--<mu-appbar title="I'm first component">-->
                <!--<mu-icon-button icon='menu' slot="left"/>-->
                <!--<mu-text-field icon="search" class="appbar-search-field"  slot="right" hintText="请输入搜索内容"/>-->
                <!--<mu-flat-button color="white" :label="author" slot="right"/>-->
                <!--<mu-icon-menu icon="more_vert" slot="right" />-->
            <!--</mu-appbar>-->

    </div>
</template>
<style lang="less">

    .appbar-search-field{
        color: #FFF;
        margin-bottom: 0;
    &.focus-state {
         color: #FFF;
     }
    .mu-text-field-hint {
        color: fade(#FFF, 54%);
    }
    .mu-text-field-input {
        color: #FFF;
    }
    .mu-text-field-focus-line {
        background-color: #FFF;
    }
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
