<template>
  <div id="app">
    <img src="./assets/logo.png">
    <el-dialog :visible.sync="openDiag">
    <div>
      <p>
        If Element is successfully added to this project, you'll see an
        <code v-text="'<el-button>'"></code>
        below
      </p>
    </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    </el-dialog>
     <el-button type="primary" >Welcome</el-button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  },
  data : function () {
    return  {
      visible: true
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
