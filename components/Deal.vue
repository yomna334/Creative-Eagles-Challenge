<template>
  <div class="col">
    <img v-bind:src="deal.banner" />
    <div class="content">
      <button class="days">2 days left</button>
      <p class="title">{{ deal.title }}</p>
      <p><span class="percent">35%</span>1.285.000 € left to fund</p>
      <div class="border">
        <div class="percent-line" style="height:3px;width:35%"></div>
      </div>
     
      <p class="para">{{ deal.teaser }}</p>
      <button class="card-footer">{{ deal.status }}</button>
      <button class="card-footer">{{ deal.type }}</button>
      <hr />
      <div class="footer">
        <div class="invest">
          <p>58</p>
          <p>Want to invest</p>
        </div>
        <div class="pipe"></div>
        <div class="invest">
          <p>58</p>
          <p>Funding Round</p>
        </div>
      </div>
    </div>
    <button class="learn">Learn More</button>
  </div>
</template>
<script>
export default {
  props: ["deal"],
};
</script>
<style >
.content {
  margin-left: 10px;
}
.days {
  width: 60px;
  background: #00516c;
  color: #ffffff;
  border-radius: 5px;
  font-size: 12px;
}
.title {
  font-size: 20px;
  font-weight: 700;
  font-style: normal;
  font-family: Manrope;
  line-height: 27.32px;
}
.para {
  font-family: Manrope;
  font-weight: 500;

  font-style: normal;
  font-size: 16px;
  line-height: 20px;
}
.percent {
  color: #67ae3d;
  font-family: Manrope;
  font-weight: 700;

  font-style: normal;
  font-size: 20px;
  line-height: 27.32px;
}
.percent-line{
  width: 100%;
    background: #67ae3d;

}
.card-footer {
  width: 65px;
  background: #f4f7f9;
  color: #063847;
  border-radius: 20px;
  font-family: Manrope;
  font-style: normal;
  font-weight: 600;
  font-size: 12px;
  line-height: 16px;
  text-align: center;
}
.invest {
  display: inline-block;
  text-align: center;
  margin-left: 30px;
}
.pipe {
  display: inline-block;
   border-left: 1px solid #DFE9EC;
  height: 40px;
  margin-left: 10px;
} 
.learn {
  width: 90%;
  margin-left: 5%;
  margin-right: 5%;
  text-align: center;
  background: #063847;
  color: #ffffff;
  height: 50px;
  border-radius: 5px;
}

</style>
