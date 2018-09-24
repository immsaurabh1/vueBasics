<template>
  <div id="app">
    <navbar-component></navbar-component>
    <div class="content">
    <body-component></body-component>
    </div>
  </div>
</template>

<script>
import NavbarComponent from './components/navbar-component';
import BodyComponent from './components/body-component';
export default {
  name: 'app',
  components: { NavbarComponent, BodyComponent },
  data () {
    return {
      msg: 'Welcome to My Vue.js App',
      selected: null,
      options: ['list', 'of', 'options']
    }
  }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
  margin:0;

}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: #FEFFEA
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}
.content{
  height:calc(100vh - 73px);
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
