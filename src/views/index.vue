<template>
  <div class="container">
    <nav-header :type="type"></nav-header>
    <div class="content">主体内容</div>
    <router-view/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import NavHeader from '@/components/public/nav-header.vue'

export default Vue.extend({
  name: 'Home',
  components: {
    NavHeader
  },
  data () {
    return {
      type: 'index'
    }
  }
})
</script>
