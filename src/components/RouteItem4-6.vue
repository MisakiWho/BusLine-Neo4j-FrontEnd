<template>
  <div class="item-container">
    <div class="table-element">
      <span>{{index+1}}</span>
    </div>
    <div class="table-element">
      <span>RouteName:</span>
    </div>
    <div class="table-element">
      <span>{{routeInfo.name}}</span>
    </div>
    <div class="table-element">
      <span>关联线路数量:</span>
    </div>
    <div class="table-element">
      <span>{{routeInfo.count}}</span>
    </div>

  </div>
</template>

<script>
export default {
name: "RouteItem2",

  props: {
    routeInfo: {
      type: Object
    },
    index: {
      type: Number
    },
  }
}
</script>

<style scoped>

.item-container{
  display: flex;
}
.table-element{
  padding:10px;
  width: 300px;
  height: 30px;
  border:solid;
}
</style>