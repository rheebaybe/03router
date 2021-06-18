<template>
  <h2>product</h2>
  <ul>
    <li v-for="(itme,i) in listData" :key="i">
      <router-link :to='`/detail/${listData[i].number}`'>{{listData[i].title}}</router-link>
    </li>
  </ul>
</template>

<script>


export default {
  name:'product',
  props:['listData']
}
</script>

<style>

</style>