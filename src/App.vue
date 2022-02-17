<template>
  <div class="app">
    <div class="clicker">
      <h1>社會信用點擊器</h1>
    </div>
    <div>
      <div class="clicker">
        <h2>社會信用: {{ count }}</h2>
      </div>
      <div class="clicker">
        <button class="button" @click="count += 1">愛派對</button>
      </div>
      <div class="xina-block">
        <img class="xina" src="https://i.imgur.com/cUin9RC.jpeg">
        <img class="xina" src="https://i.scdn.co/image/ab67616d0000b273fcc1a74f5e0ae9649ab2a104">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
      song:[ {
        src: require('./assets/sound.mp3')
      }],
      player: new Audio()
    }
  },
  methods: {
    play(song) {

    }
  }
}
</script>

<style scoped>
* {
  padding: 0;
  margin: 0;
  background-color: #902e2f;

}

.app{
  padding-top: 5%;
  padding-bottom: 5%;
}
.clicker {
  display: flex;
  align-items: center;
  justify-content: center;
}
.button{
  background-color: #ffd800;
  width: 10%;
  border: 0;
  padding: 10px 0;
  margin: 15px 0;
  text-align: center;
  color: #000;
  font-weight: bold;

}
.xina-block {
  margin-top: 5%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.xina {
  height: 50vh;
  padding: 20px;
}
</style>