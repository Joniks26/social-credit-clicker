<template>
  <div class="app">
    <div class="flex">
      <h1>社會信用點擊器</h1>
    </div>
    <div>
      <div class="flex">
        <h2>社會信用: {{ count }}</h2>
      </div>
      <div class="flex">
        <button class="button" @click="count += 1">愛派對</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    }
  }
}
</script>

<style scoped>
.app{
  padding-top: 20%;
  padding-bottom: 20%;
  background-color: red;
}
.flex {
  display: flex;
  align-items: center;
  justify-content: center;
}
.button{
  background-color: yellow;
  width: 10%;
  border: 0;
  padding: 10px 0;
  margin: 5px 0;
  text-align: center;
  color: #000;
  font-weight: bold;

}
</style>