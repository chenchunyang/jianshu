<template>
    <div>
        <form class="new-comment" method="post">
            <slot-scope></slot-scope>
            <textarea name="comment-content" placeholder="写下你的评论" v-model="value"></textarea>
            <div class="write-function-block">
                <div class="emoji-modal-wrap">
                    <a href="javascript:void(0)" class="emoji" @click="showEmoji = !showEmoji">
                        <i class="fa fa-smile-o"></i>
                    </a>
                    <!-- <div class="emoji-modal"></div> -->
                </div>
                <div class="hint">Ctrl+Enter发送</div>
                 <a href="#" class="btn-cancel">取消</a>
                <a href="#" class="btn-send" @click="submit" >发送</a>

                      <transition name="fade" mode="">
        <div class="emoji-box" v-if="showEmoji" >
          <el-button 
            class="pop-close" 
            :plain="true" 
            type="danger" 
            size="mini" 
            icon="close"
            @click="showEmoji = false"></el-button>
            <vue-emoji
              @select="selectEmoji">
            </vue-emoji>
          <span class="pop-arrow arrow"></span>
        </div>       
      </transition>

          <transition-group tag="div" name="list" class="comment">
      <p v-for="(item,index) in data" :key="index" class="item">
        <span v-html="emoji(item)"></span>
      </p>
    </transition-group>


                <!-- <a href="#" class="btn-cancel">取消</a> -->
            </div>
        </form>
    </div>
</template>
<script>
    import vueEmoji from './emoji.vue'
    export default {
        name:"myForm",
        data () {
            return {
                 value: '',
                showEmoji: false,
                data: []
            }
        },
          methods: {
            selectEmoji (code) {
            this.showEmoji = false
            this.value += code
        },
            submit () {
            this.data.push(this.value)
            this.value = ''
            }
        },
        components: {
                vueEmoji
        }
    }
</script>

<style lang="scss">
.clearfix {
  &:after {
    content: '';
    display: block;
    height: 0;
    clear: both;
    visibility: hidden;
  }
}



.fade-enter-active, .fade-leave-active { transition: opacity .5s; }
.fade-enter, .fade-leave-active { opacity: 0; }
.fade-move { transition: transform .4s; }

.list-enter-active, .list-leave-active { transition: all .5s; }
.list-enter, .list-leave-active { opacity: 0; transform: translateX(30px); }
.list-leave-active { position: absolute !important; }
.list-move { transition: all .5s;}
</style>