<template>
  <div>
    <el-row class="search">
      <el-col :span="24">
        <div class="search-line">
          <el-input
            v-model="searchtext"
            placeholder="搜索商家或地点"
            class="search-input"
            clearable
            @focus="searchfocus"
            @blur="lostfocus"/>
          <el-button 
            type="primary" 
            icon="el-icon-search"
            class="search-icon"/>
          <dl 
            v-show="showhotlist"
            class="hotlist">
            <dt>热门搜索</dt>
            <dd>DFC影城</dd>
            <dd>乌镇西栅景区</dd>
            <dd>SFC上影影城</dd>
          </dl>
          <div 
            v-show="showhostlistsearch"
            class="hostlist-search">
            <ul>
              <li>乌镇西栅景区</li>
              <li>乌镇西栅景区</li>
              <li>乌镇西栅景区</li>
            </ul>
          </div>
        </div>
        <div class="fast-search">
          <span>乌镇西栅景区</span>
          <span>乌镇西栅景区</span>
          <span>乌镇西栅景区</span>
          <span>乌镇西栅景区</span>
        </div>
      </el-col>
    </el-row>
    <el-row class="search-list">
      <el-col :span="24">
        <ul>
          <li>美团外卖</li>
          <li>猫眼电影</li>
          <li>美团酒店</li>
          <li>民宿／公寓</li>
          <li>商家入驻</li>
          <li>美团公益</li>
        </ul>
      </el-col>
    </el-row>
  </div>
</template>
<script>
export default {
  data() {
    return {
      searchtext: '',
      isFocus: false
    }
  },
  computed: {
    showhotlist: function() {
      return !this.searchtext && this.isFocus
    },
    showhostlistsearch() {
      return this.searchtext && this.isFocus
    }
  },
  methods: {
    searchfocus() {
      this.isFocus = true
    },
    lostfocus() {
      let self = this
      setTimeout(function() {
        self.isFocus = false
      }, 500)
    }
  }
}
</script>
<style scoped>
.search {
  width: 600px;
  margin-left: 80px;
  margin-top: 30px;
}
.search-line {
  width: 550px;
  height: 50px;
  position: relative;
}
.search-input {
  float: left;
  width: 550px;
}
.search-line >>> .el-input__inner {
  border-color: #13d1be;
}
.search-line >>> .el-input__inner:focus {
  border-color: #13d1be;
}
.search-icon {
  position: absolute;
  top: 0px;
  left: 470px;
  width: 81px;
  height: 41px;
  float: left;
  background-color: #13d1be;
  border: 1px solid #13d1be;
}
.hotlist {
  width: 470px;
  height: 60px;
  background-color: #fff;
  color: #999;
  border: 1px solid #e5e5e5;
  box-shadow: 0 3px 5px 1px rgba(0, 0, 0, 0.1);
  position: absolute;
  top: 40px;
  box-sizing: border-box;
  padding: 10px;
  z-index: 40;
}
.hotlist dt {
  text-align: left;
  font-weight: bold;
  margin-bottom: 5px;
}
.hotlist dd {
  float: left;
  margin-right: 5px;
  height: 20px;
  line-height: 20px;
}
.hostlist-search {
  width: 470px;
  background-color: #fff;
  color: #333;
  border: 1px solid #e5e5e5;
  box-shadow: 0 3px 5px 1px rgba(0, 0, 0, 0.1);
  position: absolute;
  top: 40px;
  box-sizing: border-box;
  padding: 5px;
  padding-left: 10px;
  z-index: 50;
}
.hostlist-search ul li {
  height: 25px;
  line-height: 25px;
  text-align: left;
}
.fast-search {
  text-align: left;
  color: #999;
}
.fast-search span {
  margin-left: 10px;
}
.search-list {
  margin-left: 60px;
  margin-top: 20px;
}
.search-list ul li {
  float: left;
  width: 100px;
  font-size: 16px;
}
</style>
