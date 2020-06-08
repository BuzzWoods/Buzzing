<template>
  <div>
    <editor :init="init"></editor>
  </div>
</template>

<script>
import tinymce from "tinymce/tinymce";
import Editor from "@tinymce/tinymce-vue";
import "tinymce/themes/silver";
import 'tinymce/icons/default/icons'

import 'tinymce/plugins/link' //链接插件
import 'tinymce/plugins/image' //图片插件
import 'tinymce/plugins/media' //媒体插件
import 'tinymce/plugins/table' //表格插件
import 'tinymce/plugins/lists' //列表插件
import 'tinymce/plugins/quickbars' //快速栏插件
import 'tinymce/plugins/fullscreen' //全屏插件
import "tinymce/plugins/axupimgs"

export default {
  data() {
    return {
      init: {
        language_url: "/tinymce/zh_CN.js", //public目录下
        language: "zh_CN",
        skin_url: '/tinymce/skins/ui/oxide',
        height: 300,
        branding: false,//是否禁用“Powered by TinyMCE”
        menubar: false,//顶部菜单栏显示,
        plugins: 'paste link quickbars table media lists image',
        toolbar: "undo redo | fullscreen | formatselect alignleft aligncenter alignright alignjustify | link unlink | numlist bullist | image media table | fontselect fontsizeselect forecolor backcolor | bold italic underline strikethrough | indent outdent imageupload",
      }
    };
  },
  components: {
    editor: Editor
  },
  mounted() {
    tinymce.init({});
  },
  created() { }
};
</script>

<style scoped lang="less">
</style>
