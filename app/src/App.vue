<template>
  <div id="app">
    <font-awesome-icon class="face-logo" :icon="['far', 'grimace']" />
    <PhotoUploader msg="Welcome to Age Estimator!" />
  </div>
</template>

<script>
import PhotoUploader from './components/PhotoUploader.vue'

export default {
  name: 'App',
  components: {
    PhotoUploader
  }
}
</script>

<style lang="scss">
:root {
  --bg-color: #eef0f2;
  --theme1: #42b983;
  --theme1-light: #64c89b;
  --theme3: #f56c6c;
  --theme2: #106fb2;
  --danger: #ed1c24;
  --title: #2c3e50;
  --desc: #6a8bad;
}

body {
  margin: 0;
  background: var(--bg-color);
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}

.center {
  display: flex;
  align-items: center;
  justify-content: center;
}

.face-logo {
  font-size: 6rem;
  color: var(--theme1);
  transition: color 0.2s;
  &:hover {
    color: var(--theme1-light);
  }
  cursor: pointer;
}
</style>
