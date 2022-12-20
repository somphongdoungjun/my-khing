<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1>{{firstname}}  {{ lastname}} </h1>
  <h1>{{nickname}}</h1>
  <h1>{{Age}}</h1>
  <h1>{{tel}}</h1>
  <h1>{{room}}</h1>
  <h1>{{major}}</h1>
  <h1>{{school}}</h1>

</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      firstname:"ชื่อ - สกุล : สมพงศ์",
      lastname:"ดวงจันทร์",
      nickname:"ชื่อเล่น : khing",
      Age:"อายุ 20 ปี",
      tel:"เบอร์โทรศัพท์ : 0973782270",
      room: "ห้อง : it5102",
      major:"สาขา : Informationtecnology",
      school:"Lannapoly"
  }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
