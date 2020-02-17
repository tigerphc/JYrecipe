<template>
  <div>
    <div>
      <nav-bar class="nav-bar">
        <div slot='left' style="height:44px;"><img src="~assets/img/logo.png" alt="" style="height:44px;"></div>
        <div slot="center">
          <el-input size="small" v-model="searchItem" placeholder="材料名，料理名" prefix-icon="el-icon-search"></el-input>
        </div>
      </nav-bar>
    </div>
    <div id="resent-search-view3"> 
      <el-row>  
        <ul id="resent-search3">
            <li class="resent-search-tag3"><i>6500S</i></li>
            <li class="resent-search-tag3"><i>SM-</i></li>
            <li class="resent-search-tag3"><i>X26</i></li>
            <li class="resent-search-tag3"><i>CS201</i></li>
            <li class="resent-search-tag3"><i>BP8904</i></li>
            <li class="resent-search-tag3"><i>101</i></li>
            <li class="resent-search-tag3"><i>fi-61</i></li>
            <li class="resent-search-tag3"><i>MT990</i></li>
            <li class="resent-search-tag3"><i>惠普</i></li>
            <li class="resent-search-tag3"><i>CDD8766</i></li>
            <li class="resent-search-tag3"><i>南天</i></li>
        </ul>  
      </el-row>                   
    </div>


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
ul{
  list-style: none;
  margin-top: 10px;
}
#resent-search3 { 
    margin-left: 15px;
    overflow-x: auto; 
    white-space:nowrap;
    width: auto;
}
::-webkit-scrollbar {
    display: none;
}

.resent-search-tag3 { 
    display: inline-block; 
    font-size: 10pt;
    border-radius: 3px;
    background-color: #f0f2f5;
    color: #686868;
    padding: 2px 10px;
    margin-right: 10px;
}
</style>
