<template>
  <div class="about">
    <h1>This is an about page</h1>

    <router-link to="/about/child1">child1</router-link>
    <router-link to="/about/child2">child2</router-link>
    <router-view></router-view>
    <artical></artical>
    <tinEditor></tinEditor>
  </div>
</template>
<script>
import artical from "@/components/text";

import tinEditor from '@/components/tiny-editor'

export default {
  name: "about",
  components: {
    artical,
    tinEditor
  },
  data() {
    return {
      
    };
  }
};
</script>
