<template>
  <v-app  id="inspire">
    <v-card class="overflow-hidden" tile>
      <v-card-actions >
        <v-flex class="d-flex" style="align-items: center; justify-content: center">
          <p class="font-weight-medium" style="font-size: 26px">关于</p>
        </v-flex>
      </v-card-actions>
      <v-card-text>
        <markdown :mdValuesP="content" :fullPageStatusP="false" :editStatusP="false"
                  :previewStatusP="true"
                  :navStatusP="false" :icoStatusP="false">
        </markdown>
      </v-card-text>

    </v-card>


  </v-app>

</template>

<script>
    import markdown from '../../components/markdown';
    export default {
        name: "about",
        data() {
            return{
                content: "#### 简介\n" +
                    "\n" +
                    "Hello，我是凌霄。这是我的照片：\n" +
                    "![本人吴彦祖](http://omsaa4hdo.bkt.clouddn.com/wyz.jpeg)\n" +
                    "\n" +
                    "可以靠颜值吃饭的我，偏偏要靠才华。\n" +
                    "\n" +
                    "#### 谈谈人生\n" +
                    "\n" +
                    "爱梦想，爱生活。平时喜欢发发呆，胡思乱想。爱音乐，目前自学吉他，希望能学会。爱宠物，老家有一只狗。想养只猫，不过现在单身，合租，养活自己都是问题。总结：我是一只有趣的程序猿。\n" +
                    "\n" +
                    "这是我的个人博客，用来记录一些平时遇到的琐碎问题和一些笔记，不期待有多大的流量。如果刚好你能从我的博客找到解决问题的方法，那么我很高兴能帮到你。\n" +
                    "\n" +
                    "#### 个人链接\n" +
                    "\n" +
                    "[Github](https://github.com/lingxiaopua)\n" +
                    "\n" +
                    "[掘金](https://juejin.im/user/5a3097fbf265da430c11ccd8)\n" +
                    "\n" +
                    "[微博](https://weibo.com/p/1005053866839538/home?from=page_100505&mod=TAB&is_all=1#place)\n" +
                    "\n" +
                    "邮箱：lingxiaopua@gmail.com\n"
            }
        },
        components: {
            markdown, // 声明mardown组件
        },
    }
</script>

<style scoped>

</style>
