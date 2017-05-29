<template>
  <div class="nav">
    <ul class="flex flex-top flex-main-justify">
      <li v-for="item in navList" class="flex-box-1" :style="{'backgroundColor':item.bgColor}">{{item.title}}</li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'page-left-nav',
    data() {
      return {
        navList: [{
          title: '111',
          isFocus: true,
          bgColor: '#111'
        }, {
          title: '222',
          isFocus: false,
          bgColor: '#222'
        }, {
          title: '333',
          isFocus: false,
          bgColor: '#333'
        }, {
          title: '444',
          isFocus: false,
          bgColor: '#444'
        }]
      }
    }
  }

</script>

<style scoped lang="scss">
  $pageLeftWidth: 300px;
  .nav {
    width: $pageLeftWidth;
    height: 100%;

    ul {
      height: 100%;
      width: 100%;
    }

    li {
      width: $pageLeftWidth - 20px;
      cursor: pointer;
      &:hover {
        transition: all ease 0.5s;
        width: 100%;
        background-color: red!important;
      }
    }
  }

</style>
