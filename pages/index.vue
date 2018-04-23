<template>
    <div style="height:100%">
       <my-header></my-header>
       <div class="container index">
           <div class="row">
               <div class="col-xs-16 main" >
                   <div class="recommend-collection">
                       <nuxt-link to="/collection/123" class="collection">
                            <img src="~~/assets/img/c1.jpg" alt="">
                            <span>简书电影</span>
                       </nuxt-link>
                        <nuxt-link to="/collection/123" class="collection">
                            <img src="~~/assets/img/c2.jpg" alt="">
                            <span>手绘</span>
                       </nuxt-link>
                        <nuxt-link to="/collection/123" class="collection">
                            <img src="~~/assets/img/c3.jpg" alt="">
                            <span>人文社科</span>
                       </nuxt-link>
                        <nuxt-link to="/collection/123" class="collection">
                            <img src="~~/assets/img/c4.jpg" alt="">
                            <span>社会热点</span>
                       </nuxt-link>
                        <nuxt-link to="/collection/123" class="collection">
                            <img src="~~/assets/img/c5.jpg" alt="">
                            <span>故事</span>
                       </nuxt-link>
                       <nuxt-link to="/collection/123" class="collection">
                            <img src="~~/assets/img/c6.jpg" alt="">
                            <span>读书</span>
                       </nuxt-link>
                        <nuxt-link to="/collection/123" class="more-collection">
                            更多热门专题
                            <i class="fa fa-angle-right"></i>
                       </nuxt-link>
                       <div class="split-line"></div>
                   </div>
               </div>
               <div class="col-xs-offset-1 col-xs-7 aside" >
                   侧边栏
               </div>
           </div>
       </div>
    </div>
</template>
<script>
    import myHeader from  '../components/myHeader'
    export default {
        head:{
            title:'简书-创作你的创作',
            meta:[
                {charset:'utf-8'},
                {name:'keywords',content:'简书首页'},
                {name:'description',content:'简书首页'},
                {name:'author',content:'李志远'}
            ]
        },
        components:{
            myHeader
        },
        data () {
            return {
                name:'首页'
            }
        }
    }
</script>
<style>

</style>