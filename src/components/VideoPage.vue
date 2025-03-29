<template>
  <main>
    <div id="preview" class="panel">
      <label><span>Preview</span></label>
    </div>
    <div id="program" class="panel">
      <img src="./../assets/img.png">
      <img src="./../assets/levels.png">
      <label><span>Program</span></label>
    </div>
    <div id="controls" class="panel">

    </div>
    <aside>Sidebar</aside>
  </main>
</template>

<script>
export default {
  name: 'VideoPage',
  props: {
    msg: String
  }
}
</script>

<style scoped>
main {
  display: grid;
  grid-template-columns: repeat(2, 1fr) 300px;
  grid-template-rows: repeat(2, 1fr);
  grid-column-gap: 20px;
  grid-row-gap: 20px;
  margin-left: 20px;
}

#preview {
  grid-area: 1 / 1 / 2 / 2;
}

#program {
  grid-area: 1 / 2 / 2 / 3;
}

#preview, #program {
  padding: 10px;
  margin-top: 20px;
  position: relative;
}

#controls {
  margin-bottom: 20px;
}

img {
  max-width: 100%;
  height: auto;
}

label {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 24px;
  text-align: center;
}
label span {
  background: rgba(0,0,0,0.5);
  border-radius: 3px;
  display: inline-block;
  padding: 2px 10px;
  height: 24px;
  line-height: 24px;
  font-weight: bold;
}

#controls {
  grid-area: 2 / 1 / 3 / 3;
}

aside {
  grid-area: 1 / 3 / 3 / 4;
}
</style>
