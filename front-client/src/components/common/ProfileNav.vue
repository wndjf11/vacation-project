<template>
  <!-- header box -->
  <div class="column1">
    <div class="row1">TODAY ??| TOTAL ?????</div>
    <div class="row2">
      <img src="@/assets/profile.jpg" alt="프로필" class="image" />
      <div class="text1">김진호 똥멍청이</div>
      <div class="text2">chan</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.column1 {
  display: flex;
  flex-direction: column;
  flex: 0.25;
  margin-left: 15px;
  margin-bottom: 15px;
  margin-top: 15px;
}
.row1 {
  font-family: "NeoDunggeunmo";
  text-align: center;
  line-height: 20px;
  flex: 0.05;
}
.row2 {
  display: flex;
  flex-direction: column;
  align-items: center;
  background-color: white;
  flex: 0.95;
  border-radius: 9px;
}

.image {
  width: 240px;
  height: 180px;
  margin: 15px;
  border-radius: 9px;
}

.text1 {
  font-family: "KyoboHand";
  text-align: center;
  height: 200px;
}

.text2 {
  font-family: "KyoboHand";
  text-align: center;
}
</style>
