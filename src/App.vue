<template>
<div id="container">
  <div class="title">
      <h1>
        {{ msg }}
      </h1>
    </div>
  <div class="ascene" v-html="ascene">
  </div>
</div>
</template>

<script>
require('aframe');

export default {
    data() {
        return {
            msg: 'Basic A-frame scene rendered in Vue.js',
            ascene:
            '<a-scene>\
                <a-sphere color="#999" radius="2" position="0 4 -15"></a-sphere>\
            </a-scene>'
        }
    }
}
</script>

<style>
.title {
    color: #333;
    text-align: center;
    font-family: sans-serif;
}
</style>
