<template>
  <div>
    <div id="navbar">

      <div class="travel_condition">
        <p class="input_describtion">遊玩類型</p>
        <select v-model="cellphone">
          <!--有value傳value，沒有value就傳包含的文字-->
          <option disabled value="">請選擇</option>
          <option>山林</option>
          <option>海景</option>
          <option>美食</option>
        </select>
      </div>
      <div class="travel_condition">
        <p class="input_describtion">出發位置</p>
        <input v-model.trim="text" placeholder="Location">
      </div>
      <div class="travel_condition">
        <p class="input_describtion">景點之間通勤時間</p>
        <input v-model.trim="text" placeholder="Hours">
      </div>
      <div class="travel_condition">
        <p class="input_describtion">交通方式</p>
        <select v-model="cellphone">
          <!--有value傳value，沒有value就傳包含的文字-->
          <option disabled value="">請選擇</option>
          <option>鐵路</option>
          <option>汽車</option>
        </select>
      </div>

      <div class="account">
        <img src="../src/assets/user.png" alt="頭貼" width="45" height="45" >
      </div>
    </div>

    <div id="attractions">
      <div class="popular">
        <p class="title">熱門選擇</p>
        <div>
        <div class="menu"></div>
        </div>
        <div class="love"></div>
        <!--<button type="button">button</button>-->
       <!--<frameset cols=120,* frameborder="0" framespacing="0" border="0">
        </frameset>-->
      </div>
      <div class="secret">
        <p class="title">私房小眾</p>
      </div>
    
    </div>
  </div>

  


</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    
  }
}
</script>

<style>
body {
  margin:0;
  padding:0;
}

#navbar{
  background-color: rgb(70, 207, 200);
  display: flex;
  flex-direction: row;
  justify-content:start;
  position: relative;
  top: 0px;
  padding: 5px;
  height: 100px;
  width: 100%;
  padding-left: 30px;
  border-bottom: solid 2px #93827F;
}
.travel_condition{
  margin-left: 20px; 
}
.account{
  width: 60px;
  height: 60px;
  margin-left: 650px;
  margin-top: 15px;
  border: solid 1px black;
  border-radius: 99em; 
  display: inline-flex;
  justify-content: center; 
  align-items: center; 
  padding-bottom: 1px;
  padding-right: 1px;
}

#attractions{
  display: flex;
  justify-content: center; 
  background-color: #FEF9FF;
}
.popular{
  /*border: solid 1px black;*/
  border-right: solid 2px #93827F;
  height: 300px;
  width: 49.5%;
  height: 500px;
}
.secret{
  /*border: solid 1px yellow;*/
  height: 300px;
  width: 50.5%;
  height: 500px;
}
.title{
  font-size: 23px;
  margin-left: 15px;

}
.menu {
     height: 10vh;
     width: 700px;
     background-color: #30FFFF;
     float: left;
 }
 .love{
      height:10vh;
      width: 200px;
      background-color: #5134d4;
      float: right;
 }

</style>
