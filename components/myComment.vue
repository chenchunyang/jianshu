<template>
    <div class="comment-list">
        <form method="post" class="new-comment">
            <nuxt-link to="/u/123" class="avatar">
                <img src="~/assets/img/default-avatar.jpg" alt="">
            </nuxt-link>
            <textarea name="commment-content" placeholder="写下你的评论"></textarea>

            <div class="write-function-block">
                <div class="emoji-modal-wrap">
                    <a href="#" class="">
                        <i class="fa fa-smile-o"></i>
                    </a>
                    <div class="emoji-modal"></div>
                </div>
                <div class="hint">Ctrl+Enter发送</div>
                <a href="#" class="btn-send">发送</a>
                <a href="#" class="btn-cancel">取消</a>
            </div>
        </form>

    </div>
</template>
<script>
    export  default {
        name:'myComment',
        data:function () {
            return{
                comments:[{
                    "page": 1,
                    "total_pages": 2,
                    "comment_exist": true,
                    "comments": [
                        {
                            "id": 23204412,
                            "compiled_content": "还不错呦~",
                            "floor": 2,
                            "note_id": 27198662,
                            "user_id": 11696335,
                            "created_at": "2018-04-25T16:37:47.000+08:00",
                            "user": {
                                "id": 11696335,
                                "slug": "ce37c858e871",
                                "nickname": "皮卡林",
                                "avatar": "http://upload.jianshu.io/users/upload_avatars/11696335/84ea8639-f3f1-480a-93d4-e1425762b1c6",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 13,
                            "children_count": 4,
                            "children": [
                                {
                                    "id": 23204440,
                                    "compiled_content": "是还不错",
                                    "user_id": 11696407,
                                    "parent_id": 23204412,
                                    "created_at": "2018-04-25T16:38:31.000+08:00",
                                    "user": {
                                        "id": 11696407,
                                        "slug": "f22f9ffb9bc6",
                                        "nickname": "f22f9ffb9bc6"
                                    }
                                },
                                {
                                    "id": 23204445,
                                    "compiled_content": "约吗？",
                                    "user_id": 11696297,
                                    "parent_id": 23204412,
                                    "created_at": "2018-04-25T16:38:41.000+08:00",
                                    "user": {
                                        "id": 11696297,
                                        "slug": "7c3479ef05d2",
                                        "nickname": "0缄默0"
                                    }
                                },
                                {
                                    "id": 23204464,
                                    "compiled_content": "\u003ca href=\"/users/7c3479ef05d2\" class=\"maleskine-author\" target=\"_blank\" data-user-slug=\"7c3479ef05d2\"\u003e@0缄默0\u003c/a\u003e 再见",
                                    "user_id": 11696335,
                                    "parent_id": 23204412,
                                    "created_at": "2018-04-25T16:39:06.000+08:00",
                                    "user": {
                                        "id": 11696335,
                                        "slug": "ce37c858e871",
                                        "nickname": "皮卡林"
                                    }
                                }
                            ]
                        },
                        {
                            "id": 23204424,
                            "compiled_content": "报警找我110",
                            "floor": 5,
                            "note_id": 27198662,
                            "user_id": 11726469,
                            "created_at": "2018-04-25T16:38:04.000+08:00",
                            "user": {
                                "id": 11726469,
                                "slug": "7466c63a08ac",
                                "nickname": "远方无远方",
                                "avatar": "http://upload.jianshu.io/users/upload_avatars/11726469/2fa7e041-5918-4e17-b3e2-8b252a5a6a32",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 8,
                            "children_count": 1,
                            "children": [
                                {
                                    "id": 23204454,
                                    "compiled_content": "你是个傻子吧",
                                    "user_id": 11726654,
                                    "parent_id": 23204424,
                                    "created_at": "2018-04-25T16:38:58.000+08:00",
                                    "user": {
                                        "id": 11726654,
                                        "slug": "9751bf239b07",
                                        "nickname": "Ace_e60d"
                                    }
                                }
                            ]
                        },
                        {
                            "id": 23204418,
                            "compiled_content": "支持一下 ，消灭0回复",
                            "floor": 4,
                            "note_id": 27198662,
                            "user_id": 11726245,
                            "created_at": "2018-04-25T16:37:51.000+08:00",
                            "user": {
                                "id": 11726245,
                                "slug": "b847b7d49625",
                                "nickname": "就是cc",
                                "avatar": "http://cdn2.jianshu.io/assets/default_avatar/8-a356878e44b45ab268a3b0bbaaadeeb7.jpg",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 6,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204427,
                            "compiled_content": "呦呦呦~\u003cimg src=\"//static.jianshu.io/assets/emojis/blush.png\" alt=\":blush:\" title=\":blush:\" class=\"emoji\" width=\"20\" height=\"20\"\u003e",
                            "floor": 6,
                            "note_id": 27198662,
                            "user_id": 11726215,
                            "created_at": "2018-04-25T16:38:11.000+08:00",
                            "user": {
                                "id": 11726215,
                                "slug": "0f8e999deb37",
                                "nickname": "丿我心忧玲丶",
                                "avatar": "http://upload.jianshu.io/users/upload_avatars/11726215/c14e6fa6-ecee-4193-ad4d-eb8e3c661adb",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 4,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204451,
                            "compiled_content": "你是真的皮。。。",
                            "floor": 11,
                            "note_id": 27198662,
                            "user_id": 10300732,
                            "created_at": "2018-04-25T16:38:54.000+08:00",
                            "user": {
                                "id": 10300732,
                                "slug": "8ac4893532c4",
                                "nickname": "啦啦啦啦啦_0418",
                                "avatar": "http://upload.jianshu.io/users/upload_avatars/10300732/38fc7895-ad5c-4fa3-96cc-065de6319253",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 3,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204435,
                            "compiled_content": "乌拉拉拉拉啊啊啊",
                            "floor": 7,
                            "note_id": 27198662,
                            "user_id": 6616680,
                            "created_at": "2018-04-25T16:38:25.000+08:00",
                            "user": {
                                "id": 6616680,
                                "slug": "940274e4900b",
                                "nickname": "风的归途",
                                "avatar": "http://cdn2.jianshu.io/assets/default_avatar/11-4d7c6ca89f439111aff57b23be1c73ba.jpg",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 2,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204437,
                            "compiled_content": "老夫夜观天象，方只明天晴转多云",
                            "floor": 8,
                            "note_id": 27198662,
                            "user_id": 11728286,
                            "created_at": "2018-04-25T16:38:28.000+08:00",
                            "user": {
                                "id": 11728286,
                                "slug": "a106764cb017",
                                "nickname": "無悔_0581",
                                "avatar": "http://upload.jianshu.io/users/upload_avatars/11728286/9942f894-e2ae-492f-b225-6a9b4433c164",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 2,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204447,
                            "compiled_content": "看昵称",
                            "floor": 9,
                            "note_id": 27198662,
                            "user_id": 11726229,
                            "created_at": "2018-04-25T16:38:50.000+08:00",
                            "user": {
                                "id": 11726229,
                                "slug": "c7e3e97b12e7",
                                "nickname": "我是水军啊",
                                "avatar": "http://cdn2.jianshu.io/assets/default_avatar/5-33d2da32c552b8be9a0548c7a4576607.jpg",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 2,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204448,
                            "compiled_content": "为大佬打尻！",
                            "floor": 10,
                            "note_id": 27198662,
                            "user_id": 11825620,
                            "created_at": "2018-04-25T16:38:51.000+08:00",
                            "user": {
                                "id": 11825620,
                                "slug": "7c30570b1c4f",
                                "nickname": "paradian",
                                "avatar": "http://cdn2.jianshu.io/assets/default_avatar/9-cceda3cf5072bcdd77e8ca4f21c40998.jpg",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 1,
                            "children_count": 0,
                            "children": []
                        },
                        {
                            "id": 23204456,
                            "compiled_content": "小礼物走一波~\u003cimg src=\"//static.jianshu.io/assets/emojis/unamused.png\" alt=\":unamused:\" title=\":unamused:\" class=\"emoji\" width=\"20\" height=\"20\"\u003e",
                            "floor": 12,
                            "note_id": 27198662,
                            "user_id": 11731124,
                            "created_at": "2018-04-25T16:38:58.000+08:00",
                            "user": {
                                "id": 11731124,
                                "slug": "668a875e127e",
                                "nickname": "暮冬Gentle已认证",
                                "avatar": "http://upload.jianshu.io/users/upload_avatars/11731124/ee3acab2-150e-4ac4-ace6-fa60b6c0660b",
                                "is_author": false,
                                "badge": null
                            },
                            "liked": true,
                            "likes_count": 1,
                            "children_count": 0,
                            "children": []
                        }
                    ]
                }]
            }
        },
        methods:{

        }

    }
</script>

<style scoped>
    .comment-list{
        padding-top: 20px;
    }
    .comment-list .new-comment{
        margin: 0 0 20px 56px;
    }
    .comment-list .new-comment .avatar {
        width: 38px;
        height: 38px;
        position: absolute;
        left: -38px;
        display: inline-block;
        margin-right: 10px;
    }
    .comment-list .new-comment textarea{
        padding: 10px 15px;
        width: 100%;
        height: 80px;
        outline: none;
        resize: none;
        display: inline-block;
        font-size: 13px;
        border: 1px solid #dcdcdc;
        background: #f7f7f7;
        border-radius: 4px;
        vertical-align: top;

    }
    .comment-list .new-comment .write-function-block{
        height: 50px;
    }
    .comment-list .new-comment .write-function-block .emoji{
        float: left;
        margin-top: 14px;
    }
    .comment-list .new-comment .write-function-block .emoji i{
        font-size: 30px;
    }
    .comment-list .new-comment .write-function-block .emoji i:hover{
        color: #2f2f2f;
    }
    .comment-list .new-comment .write-function-block .hint{
        float: left;
        margin: 20px 0 0  20px;
        font-size: 13px;
        color: #969696;
    }
    .comment-list .new-comment .write-function-block .btn-send{
        float: right;
        width: 78px;
        padding: 8px 18px;
        margin: 10px 0;
        display: block;
        font-size: 16px;
        background: #42c02e;
        color: #fff;
        text-align: center;
        border-radius: 20px;
        outline: none;

    }
    .comment-list .new-comment .write-function-block .btn-cancel{
        float: right;
    }


</style>