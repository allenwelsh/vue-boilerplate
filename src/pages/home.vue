<template>
  <div id="home">
    <img src="../assets/logo.png">
    <h1>{{ msg }}</h1>
    <el-button @click.native="startHacking">Let's do it</el-button>
  </div>
</template>

<script>
export default {
  name: 'home-view',
  data() {
    return {
      msg: 'Use Vue 2.0 Today!'
    };
  },

  methods: {
    startHacking() {
      this.$notify({
        title: 'It Works',
        message: 'We have laid the groundwork for you. Now it\'s your time to build something epic!',
        duration: 6000
      });
    }
  }
};
</script>

<style>
#home {
  padding: 15px;
}
</style>
