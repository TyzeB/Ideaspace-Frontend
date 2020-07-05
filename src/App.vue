<template>
  <div id="app">
    <nav class="nav-bar">
      <div>
        <h3>IS</h3>
      </div>
      <div>
        <button class="auth">Log In</button>
        &nbsp;
        <button class="auth">Sign Up</button>
      </div>
    </nav>
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
};
</script>

<style lang="scss">
$cornflower: #6495ED;
$deepsky: #00BFFF;
$whiteish: #fbfbff;
$greyblue: #3B4252;
$greyblue1: #4C566A;

body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $whiteish;
  background: $greyblue;
  min-height: 100vh;
}

.nav-bar {
  background-color: $greyblue1;
  display: flex;
  justify-content: space-around;
  flex-direction: row;
  align-items: center;
  div {
    button {
      vertical-align: text-top;
    }
  }
}

.auth {
  width: 100px;
  height: 30px;
  border: none;
  outline: none;
  font-weight: bold;
  color: $whiteish;
  background-color: $cornflower;
  background: linear-gradient(90deg, $cornflower 0%, $deepsky 100%);
  &:hover {
    background: linear-gradient(90deg, $deepsky 0%, $cornflower 100%);
    border: 2px solid $deepsky;
  }
}
</style>
