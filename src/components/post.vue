<template>
  <div>
    <div>{{post.title}}</div>
    <div>{{post.content}}</div>
    <button v-on:click="$emit('enlarge-text',2)">Enlarge text</button>
  </div>
</template>

<script>
export default {
    name:'post',
    props: ['post'],
    data() {
        return {
            //postFontSize:20,
        };
    },
    computed: {

    },
    created() {

    },
    methods: {

    },
};
</script>

<style scoped lang="less">
</style>
