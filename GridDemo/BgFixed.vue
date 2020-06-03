<template>
    <div class="grids">
      <div class="grid-item bg1">
        <h2>16<span>|24</span></h2>
        <p>完成目标数</p>
      </div>
      <div class="grid-item bg1">
        <h2><i class="iconfont iconiconset0251"></i></h2>
        <p>呼吸</p>
      </div>
      <div class="grid-item bg2">
        <h2><i class="iconfont iconpaobu"></i></h2>
        <p>公里</p>
      </div>
      <div class="grid-item bg1">
        <h2>36℃</h2>
        <p>温度</p>
      </div>
      <div class="grid-item bg1">
        <h2><i class="iconfont iconbed"></i></h2>
        <p>睡眠质量</p>
      </div>
      <div class="grid-item bg2">
        <h2>98<span>bpm</span></h2>
        <p>心率</p>
      </div>
      <div class="grid-item bg1">
        <h2>50<span>kg</span></h2>
        <p>体重</p>
      </div>
      <div class="grid-item bg1">
        <h2>20<span>%</span></h2>
        <p>体脂率</p>
      </div>
      <div class="grid-item bg2">
        <h2>108<span>mgdl</span></h2>
        <p>血糖</p>
      </div>
      <div class="grid-item bg2">
        <h2>680<span>kcal</span></h2>
        <p>平均消耗</p>
      </div>
      <div class="grid-item bg2">
        <h2><i class="iconfont iconjianshen"></i></h2>
        <p>锻炼</p>
      </div>
      <div class="grid-item bg2">
        <h2>85<span>%</span></h2>
        <p>身体含水量</p>
      </div>
    </div>
</template>

<script>
    export default {
        name: "BgFixed"
    }
</script>

<style scoped>
.grids{
  width: 100vw;
  height:100vh;
  background-color: #333;
  color:#fff;
  display: grid;
  grid-template-columns:repeat(4,1fr);
  grid-gap: 8px;
}
.grids > div:nth-of-type(1){
  grid-column: 1/3;
}

.grids > div:nth-of-type(6){
  grid-column: 3/5;
}
.grids > div:nth-of-type(9){
  grid-column: 3/5;
}
.grids > div:nth-of-type(10){
  grid-column: 1/3;
}
  .grid-item{
    background-size: cover;
    background-attachment: fixed;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;

    transition: all 0.5s ease-in;
  }
  .grid-item.bg1{
    background-image: url("../../assets/images/grid/bg5.jpg");
    color:#2e2e2e;
  }
  .grid-item.bg2{
    background-image: url("../../assets/images/grid/bg4.jpg");
  }
  .grid-item i.iconfont{
    font-size: 34px;
  }
  .grid-item:hover{
    cursor:pointer;
    opacity: 0.8;
    transform: scale(0.98);
  }
</style>
