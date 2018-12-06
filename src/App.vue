<template>
  <div id="app">
    <h1>SVG</h1>
    <div class="svg-item">
      <h2>
        <el-tag>Github</el-tag>
      </h2>
      <svg width="676" height="84">
        <g v-for="(item, index) in 52" :key="index" :id="item">
          <a xlink:href="">
            <rect v-for="(sub, num) in 7" @mouseenter="enter" @mouseleave="leave" :key="num" :x="`${13*index}`" :y="`${12*num}`" style="width:10px;height:10px;fill:#ebedf0;"></rect>
          </a>
        </g>
      </svg>
    </div>
    <div class="svg-item">
      <h2>
        <el-tag>animat</el-tag>
      </h2>
      <svg width="100" height="100">
        <!--  -->
        <circle cx="50" cy="50" r="45" fill="#fff" stroke="#000" stroke-width="5"></circle>
        <!--  -->
        <path d="M30 35 A 5 5,0 0 1,40 35" stroke="#000" fill="#fff" stroke-width="5" fill-opacity="0.5" />
        <path d="M60 35 A 5 5,0 0 1,70 35" stroke="#000" fill="#fff" stroke-width="5" fill-opacity="0.5" />
        <!--  -->
        <path d="M65 65 A 15 15,0 0 1,35 65" stroke="#000" fill="#fff" stroke-width="5" fill-opacity="0.5" />
        <!--  -->
        <circle cx="15" cy="85" r="10" fill="#fff" stroke="#000" stroke-width="5"></circle>
        <circle cx="85" cy="85" r="10" fill="#fff" stroke="#000" stroke-width="5"></circle>
      </svg>
    </div>
    <div class="svg-item">
      <h2>
        <el-tag>太极</el-tag>
      </h2>
      <svg viewBox="0 0 100 100" preseveAspectRatio="xMidyMid slice" width="100" height="100">
        <g id="taiji">
          <circle r="50" cx="50" cy="50" fill="#fff" stroke="#999" stroke-width="1" />
          <path d="M0 50 a25 25 0 1 0 50 0 a25 25 0 1 1 50 0 a50 50 0 1 0 -100 0" stroke-width="" stroke="" fill="#000" />
          <circle r="6.25" cx="25" cy="50" fill="#fff" />
          <circle r="6.25" cx="75" cy="50" fill="#000" />
        </g>
      </svg>
    </div>
    <div class="svg-item">

    </div>
    <div class="svg-item">

    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {
    /* Comment */
    enter(e) {
      e.target.style.fill = "#bdbebf";
    },
    leave(e) {
      e.target.style.fill = "#ebedf0";
    }
  }
};
</script>


<style lang="less">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
