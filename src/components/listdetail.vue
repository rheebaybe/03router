<template>
  <div class="container">
      {{$route.params.id}}
      <router-link to="/product">뒤로가기</router-link>
      <h2>list detail</h2>
      <div>
          <h3>{{listData[$route.params.id].title}}</h3>
          <p>{{listData[$route.params.id].content}}</p>
      </div>
  </div>
</template>

<script>
export default {
    name:'detail',
    props:['listData']
}
</script>

<style>
    .container{
        padding: 10px;
    }
</style>