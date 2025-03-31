<template>
  <Header/>
  <VideoPage/>
</template>

<script>
import Header from './components/Header.vue'
import VideoPage from './components/VideoPage.vue'

export default {
  name: 'App',
  components: {
    Header,
    VideoPage,
  },
}
</script>

<style>
body, html {
  padding: 0;
  margin: 0;
  background: #353535;
  height: 100%;
  overflow: hidden;
}

.header {
  background: #282828;
  border-bottom: 1px solid #070707;
}

.panel {
  background: #2d2d2d;
  border: 1px solid #1d1d1d;
  border-radius: 6px;
}

* {
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
  height: 100%;
}

main {
  height: calc(100% - 48px);
}
</style>
