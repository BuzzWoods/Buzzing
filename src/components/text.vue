<template>
  <div :style="{fontSize: postFontSize + 'px'}">
    <post :post='post' v-on:enlarge-text="postFontSize += $event"></post>
  </div>
</template>

<script>
import post from "@/components/post";
export default {
  name: "enlarge",
  props: {},
  components: {
    post
  },
  data() {
    return {
      post: {
        title: "happy day",
        content: "weather is nice!!!"
      },
      postFontSize: 20
    };     
  },
  computed: {},
  created() {},
  methods: {}
};
</script>

<style scoped lang="less">

</style>
