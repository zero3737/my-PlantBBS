<template>
  <div id="app">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="less">
* {

  list-style: none;
  user-select: none;

}
a {

  color: @gray;

  &:hover {

    cursor: pointer;
    color: @red;

  }

}
.badge {

  background-color: @green;
  margin-right: 15px;

}

</style>
