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
                   <div class="list-container">
                       <ul class="note-list">
                           <li class="have-img">
                               <nuxt-link to="/p/123" class="wrap-img">
                                    <img src="~~/assets/img/b.jpg" >
                               </nuxt-link>
                               <div class="content">
                                   <div class="author">
                                       <nuxt-link to="/p/123" class="avatar">
                                            <img src="~~/assets/img/default-avatar.jpg" >
                                        </nuxt-link>
                                         <div class="info">
                                        <nuxt-link to="/u/123" class="nickname">
                                                测试用户
                                        </nuxt-link>
                                        <span class="time ">04.12 10:18</span>
                                    </div>
                                     </div>
                                   
                                  
                                   
                                    <nuxt-link class="title" to="/p/123">我乖了，你就会永远睡我吗</nuxt-link>
                                    <div class="abstract">一个月前，七七还骑在大刘的腿上，可怜楚楚的说：“我乖了，你就会永远睡我吗？”大刘一边把剥开的情人节巧克力，塞进七七嘴里，一边将信将疑的回答：“是啊！”大刘的眼睛里全是迷雾，七...</div>
                                    <div class="meta">
                                         <nuxt-link to="/pc/123"  class="collection-tag">社会与法</nuxt-link>
                                        <nuxt-link to="/p/123" >
                                                <i class="fa fa-eye"></i>
                                                1500
                               </nuxt-link>
                                <nuxt-link to="/p/123" >
                                                <i class="fa fa-comment"></i>
                                                100
                               </nuxt-link>
                                    <span>
                                        <i class="fa fa-heart"></i>
                                        20
                                    </span>
                                    
                                    </div>
                               </div>
                               
                           </li>
                       </ul>
                       <ul class="note-list">
                           <li class="have-img">
                               <!-- <nuxt-link to="/p/123" class="wrap-img">
                                    <img src="~~/assets/img/b.jpg" >
                               </nuxt-link> -->
                               <div class="content">
                                   <div class="author">
                                       <nuxt-link to="/p/123" class="avatar">
                                            <img src="~~/assets/img/default-avatar.jpg" >
                                        </nuxt-link>
                                           <div class="info">
                                        <nuxt-link to="/u/123" class="nickname">
                                                测试用户
                                        </nuxt-link>
                                        <span class="time ">04.12 10:18</span>
                                    </div>
                                     </div>
                                 
                                  
                                   
                                    <div class="title">我乖了，你就会永远睡我吗</div>
                                    <div class="abstruct">一个月前，七七还骑在大刘的腿上，可怜楚楚的说：“我乖了，你就会永远睡我吗？”大刘一边把剥开的情人节巧克力，塞进七七嘴里，一边将信将疑的回答：“是啊！”大刘的眼睛里全是迷雾，七...</div>
                                    <div class="meta">
                                        <nuxt-link to="/p/123" >
                                                <i class="fa fa-eye"></i>
                                                1500
                               </nuxt-link>
                                <nuxt-link to="/p/123" >
                                                <i class="fa fa-comment"></i>
                                                100
                               </nuxt-link>
                                    <span>
                                        <i class="fa fa-heart"></i>
                                        20
                                    </span>
                                    
                                    </div>
                               </div>
                               
                           </li>
                       </ul>
                       <a href="#" class="load-more">阅读更多</a>
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
import myHeader from "../components/myHeader";
export default {
  head: {
    title: "简书-创作你的创作",
    meta: [
      { charset: "utf-8" },
      { name: "keywords", content: "简书首页" },
      { name: "description", content: "简书首页" },
      { name: "author", content: "李志远" }
    ]
  },
  components: {
    myHeader
  },
  data() {
    return {
      name: "首页"
    };
  }
};
</script>
<style>

</style>