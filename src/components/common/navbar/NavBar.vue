<template>
  <div id="nav-bar">
    <el-row :gutter="0">
      <el-col :span="10" align="center"><div><slot name="left"></slot></div></el-col>
      <el-col :span="12" align="center"><div><slot name="center"></slot></div></el-col>
    </el-row>
  </div>
</template>

<script>
	export default {
		name: "NavBar"
	}
</script>

<style scoped>
  #nav-bar {
    position: relative;
    z-index: 10;

    /* display: flex; */

    height: 44px;
    line-height: 44px;
    text-align: center;
    background-color: #74B243;
  }


</style>
