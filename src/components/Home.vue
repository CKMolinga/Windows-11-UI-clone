<template>
  <div class="main-container">
    <div class="flex">
      <div class="apps-container computer">
        <img class="icon" src="../assets/computer.0fa868a6.png" alt="pc">
        <h3 class="apps">This PC</h3>
      </div>
      <div class="apps-container computer">
        <img class="icon" src="../assets/trash-empty.ffc7f0e7.png" alt="pc">
        <h3 class="apps">Recycle Bin</h3>
      </div>
      <div class="apps-container computer">
        <img class="icon" src="../assets/explorer.1d241c47.png" alt="pc">
        <h3 class="apps">File Explorer</h3>
      </div>
      <div class="apps-container computer">
        <img class="icon" src="../assets/store-dark.b75a8bd7.png" alt="pc">
        <h3 class="apps">Microsoft Store</h3>
      </div>
      <div class="apps-container computer">
        <img class="icon" src="../assets/edge.bd39ae5b.png" alt="pc">
        <h3 class="apps">Microsoft Edge</h3>
      </div>
    </div>

    <div class="dialogue-box relative">
      <div class="header m-3">
        <h4 class="pinned-title">Pinned</h4>
        <h4 class="all-apps bg-gray-50 px-3 cursor-pointer">All apps</h4>
      </div>
      <div class="pinned-apps flex flex-wrap m-3 pt-4">
        <div class="">
        <img class="pinnedApp-icon" src="../assets/edge.bd39ae5b.png" alt="pc">
        <h3 class="pinnedApp-title">Edge</h3>
      </div>
      <div class="">
        <img class="pinnedApp-icon" src="../assets/edge.bd39ae5b.png" alt="pc">
        <h3 class="pinnedApp-title">Edge</h3>
      </div>
      <div class="">
        <img class="pinnedApp-icon" src="../assets/edge.bd39ae5b.png" alt="pc">
        <h3 class="pinnedApp-title">Edge</h3>
      </div>
      <div class="">
        <img class="pinnedApp-icon" src="../assets/edge.bd39ae5b.png" alt="pc">
        <h3 class="pinnedApp-title">Edge</h3>
      </div>

      </div>

      <div class="bottom bg-gray-400 h-12"></div>
    </div>


    <div class="footer">
      <div class="footer-items">
         <img class="icon pr-5" src="../assets/start.66f17ddc.png" alt="pc">
         <img class="icon pr-5" src="../assets/search.png" alt="pc">
          <img class="icon" src="../assets/vsCode.png" alt="pc">
           <img class="icon" src="../assets/github.png" alt="pc">
            <img class="icon" src="../assets/edge.bd39ae5b.png" alt="pc">
            <img class="icon" src="../assets/spotify.png" alt="pc">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main-container {
  height: 100vh;
  width: 100vw;
  background: url("../assets/light.ee0a71d6.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}

.flex {
  flex-direction: column;
  justify-content: space-between;
}

.apps-container{
  display: flex;
  flex-direction: column;
  width: 10vw;
  align-items: center;  
  margin-left: 5px;
  margin-top: 5px;
  padding: 25px 5px;
}

.apps-container:hover {
  background: #b5cbe0;
}

.icon {
  height: 45px;
  width: 45px;
}

.apps {
  color: #fff;
  font-size: 14px; 
}

.dialogue-box {
  height: 75vh;
  width: 75vw;
  background: #b5cbe0de;
  position: absolute;
  bottom: 7%;
  left: 10%;
  border-radius: 6px;
}

.header {
  display: flex;
  justify-content: space-between;
}

.pinnedApp-icon {
  height: 25px;
  width: 25px;
  flex-wrap: wrap;
}

.pinnedApp-title {
  font-size: 12px;
}

.pinned-apps {
  flex-direction: row;
}

.bottom { 
  position: absolute; 
  bottom: 0;
  left: 0;
}
.footer {
  background: #b5cbe0;
  height: 5.5vh;
  width: 100vw;
  position: absolute;
  bottom: 0;
}
.footer-items {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.footer-items img {
  height: 35px;
  width: 30px;
  padding: 8px 5px 6px 5px;
  margin: 0 2px;
}

.footer-items img:hover {
  background: #fff;
}

@media (min-width: 992px) {
  .dialogue-box {
  height: 65vh;
  width: 45vw;
  background: #b5cbe0de;
  position: absolute;
  bottom: 7%;
  left: 30%;
  border-radius: 6px;
}
}



</style>
