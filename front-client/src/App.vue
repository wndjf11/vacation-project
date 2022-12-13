<template>
  <div id="app">
    <body>
      <div class="bookcover">
        <div class="bookdot">
          <div class="page">
            <!-- 프로필 -->
            <profile-nav />
            <div class="column2">
              <div class="row3">
                <div class="column3">chan_chan_2222</div>
                <div class="column4">https://chan_chan_2222</div>
              </div>
              <div class="row4">
                <div class="updated">
                  <div class="cate">
                    Updated
                    <hr class="line" />
                  </div>
                  <div class="column6">
                    <div class="row5">
                      <span class="red">방명록</span> 스토리는 냠냠<br />
                      <span class="blue">개발일지</span> css어려웡
                      <br />
                      <span class="blue">개발일지</span> vue로 만들자<br />
                      <span class="red">방명록</span> 가보자가보자<br />
                    </div>
                    <div class="row6">
                      <hr />
                      개발일지: 0/25
                      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;방명록:0/25
                      <hr />
                    </div>
                  </div>
                </div>
                <div class="updated">
                  <div class="cate">
                    담벼락
                    <hr class="line" />
                  </div>
                </div>
              </div>
            </div>
            <div class="column5"></div>
          </div>
        </div>
      </div>
    </body>
  </div>
</template>
<script>
import ProfileNav from "@/components/common/ProfileNav.vue";
// import FooterNav from "@/components/common/FooterNav.vue";
export default {
  components: { ProfileNav },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  background-color: #888;
}

.bookcover {
  height: 720px;
  /* 1280x720 */
  width: 1280px;
  margin: 100px auto;
  /* 변두리 색 */
  background-color: rgb(169, 168, 186);
  border-radius: 9px;
  position: relative;
}

.bookdot {
  height: 696px;
  /* 24 */
  width: 1256px;
  border: dashed white 2px;
  border-radius: 9px;
  position: absolute;
  top: 12px;
  left: 12px;
}
.page {
  display: flex;
  /* 696-26 */
  height: 670px;
  width: 1230px;
  /* 내부색 */
  background-color: rgb(206, 203, 234);
  border-radius: 9px;
  position: absolute;
  top: 11px;
  left: 11px;
}

.column2 {
  display: flex;
  flex-direction: column;
  flex: 0.6;
  margin-top: 15px;
  margin-bottom: 15px;
  margin-left: 15px;
}
.row3 {
  display: flex;
  flex-direction: row;
  flex: 0.05;
}

.column3 {
  flex: 0.5;
  line-height: 20px;
  text-align: left;
}

.column4 {
  flex: 0.5;
  line-height: 20px;
  text-align: center;
}

.row4 {
  flex: 0.95;
  background-color: white;
  border-radius: 9px;
}
.column5 {
  flex: 0.14;
  /* background-color: rgb(230, 230, 230); */
  border: solid rgb(255, 255, 255);
  margin-top: 15px;
  margin-bottom: 15px;
  margin-left: 1px;
}

@font-face {
  font-family: "NeoDunggeunmo";
  src: url("https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2001@1.3/NeoDunggeunmo.woff")
    format("woff");
  font-weight: normal;
  font-style: normal;
}

.updated {
  display: flex;
  flex-direction: column;
  height: 30%;
  margin: 15px;
}
.column6 {
  display: flex;
  justify-content: space-between;
}
.red {
  background-color: rgb(242, 98, 94);
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  color: white;
}
.blue {
  background-color: rgb(102, 122, 193);
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  color: white;
}
.row5 {
  font-size: 13px;
  line-height: 20px;
  text-align: left;
  padding: 10px;
}
.row6 {
  font-size: 13px;
  padding: 10px;
}

.line {
  border: none;
  height: 1.5px;
  background-color: #bbb;
  margin-top: 0px;
  margin-bottom: 3px;
}
.dot {
  border: none;
  border: 1px dashed #bbb;
  margin-top: 1px;
  margin-bottom: 1px;
}
.cate {
  font-family: "KOTRA_BOLD-Bold";
  color: #6fadcf;
}
@font-face {
  font-family: "KOTRA_BOLD-Bold";
  src: url("https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-10-21@1.1/KOTRA_BOLD-Bold.woff")
    format("woff");
  font-weight: normal;
  font-style: normal;
}
@font-face {
  font-family: "KyoboHand";
  src: url("https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-04@1.0/KyoboHand.woff")
    format("woff");
  font-weight: normal;
  font-style: normal;
}
</style>
