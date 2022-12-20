<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1>{{firstname}}  {{ lastname}} </h1>
  <h1>{{nickname}}</h1>
  <h1>{{Age}}</h1>
  <h1>{{tel}}</h1>
  <h1>{{room}}</h1>
  <h1>{{major}}</h1>
  <h1>{{school}}</h1>
  
  <h2>{{getFullname()}}</h2>
  <h3>{{hobby}}</h3>
   <h4>{{profile}}</h4>


<!-- เรียกอาร์เรย์-->
   <ul>
      <li> {{hobby[0]}}</li>
      <li> {{hobby[1] }}</li>
      <li> {{hobby[2] }}</li>
      <li> {{hobby[3] }}</li>
      <li> {{hobby[4] }}</li>
    </ul>
<!-- เรียกอาร์เรย์-->

</template>

<script>


export default {
  name: 'App',
  data(){ //เรียกเฉพาะข้อมูล
    return{
      firstname:"ชื่อ - สกุล : สมพงศ์",
      lastname:"ดวงจันทร์",
      nickname:"ชื่อเล่น : khing",
      Age:"อายุ 20 ปี",
      tel:"เบอร์โทรศัพท์ : 0973782270",
      room: "ห้อง : it5102",
      major:"สาขา : นักพัฒนาซอฟต์แวร์คอมพิวเตอร์",
      school:"วิทยาลัย : วิทยาลัยเทคโนโลยีโปลิเทคนิคลานนา เชียงใหม่",

      hobby : ["เล่นเกมส์","นอน","กินข้าว","ดูหนัง","เล่นกีฬา"],
      profile : {gender: "male", weiht:50 , hight:170, status: false}
  }
  },
  methods :{ //เรียกฟังก์ชั่น
    getFullname(){
      return this.firstname + this.lastname //เรียกมาจาก data ด้านบน
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
