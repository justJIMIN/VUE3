<template>
  <div>
    <Menu msg="Welcome to Your Vue.js App"/>
    <router-view></router-view>
  </div>
  
</template>
<script>
import Menu from '@/components/nav2.vue';

export default {
  name: 'App',
  components: {
    Menu,
  },
  methods:{
    fnSubPage() {
      this.$router.push('/view1')
    }
  }
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
