<template>
  <div>
    <nav-bar class="nav-bar">
      <div slot='left'><img src="~assets/img/logo.png" alt="" style="height:44px;"></div>
      <div slot="center">
        <el-input size="small" v-model="searchItem" placeholder="材料名，料理名" prefix-icon="el-icon-search"></el-input>
      </div>
    </nav-bar>
  </div>
</template>

<script>
import NavBar from 'common/navbar/NavBar'
export default {
  name: "Home",
  components: {
    NavBar,

  },
  data() {
     return {
      searchItem: '',
     }

    }

}
</script>

<style scoped>

</style>
