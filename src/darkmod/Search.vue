<template>
  <div id="app">
<!--    搜索功能实现文件-->
<!--    暂未实现-->
    <br/>
    <br/>
    <input class="search-input" v-model="searchInput" placeholder="搜索您想要的应用" />
    <button class="search-button" @click="search">搜索</button>




  </div>
</template>

<script>


  export default {
    name: "darkSearch",
    data() {
      return {
        list: [],
        searchInput: "",
        downloadContent: "DOWNLOAD"
      };
    },
    methods: {
      search:function() {

      }
    },
    mounted() {
    },
  };
</script>



<style scoped>

  .search-input{
    height: 40px;
    width: 40%;
    text-align: center;
    font-size: 20px;
    transition: all 0.3s;
    border: solid 2px darkgray;
    border-radius: 10px 0 0 10px;
    position: relative;
    top:-2px;
  }
  .search-input:hover{
    border: solid 2px black;
  }
  .search-button{
    border-radius: 0 10px 10px 0;
    height: 46px;
    width: 100px;
    margin:0;
    border: solid 2px darkgray;
    padding: 0;
    position: relative;
    /*top:2px;*/
    left:-7px;
    transition: all 0.3s;
    font-size: 20px;
  }
  .search-button:hover{
    border: solid 2px black;
  }

</style>

