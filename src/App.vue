<template>
  <div id="app">
    <login v-show="isLogin"></login>
    <Layout v-show="!isLogin"></Layout>
  </div>
</template>

<script>
import Layout from 'components/Layout'
import Login from 'components/Login'
export default {
  name: 'app',
  components: {
    Layout,
    Login
  },
  data () {
    return {
      isLogin: false
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
