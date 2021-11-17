<template>
  <div class="sidebar">
    <img src="../static/Logo.png" alt="logo" />
    <ul>
      <li>
        <span
          ><img class="icon" src="../static/Combined Shape.svg" />Cockpit</span
        >
      </li>
      <li class="active">
        <img class="active-icon icon" src="../static/starPath.png" />Investment
        Opportunities
      </li>
      <li><img class="icon" src="../static/Shape.png" />My Investments</li>
      <hr class="border-solid" />
      <li>
        <img class="icon" src="../static/KnowledgeCenter.png" />Knowledge Center
      </li>
      <li>
        <img class="icon" src="../static/Combined Shape.png" />Venture Pool
      </li>
      <li><img class="icon" src="../static/Fee Model.png" />Fee Model</li>
    </ul>
    <div class="recommendation">
      <img class="ico" src="../static/Vector.png" />
      <p>Recommend primeCrowed</p>
      <button class="invite">Invite Friends</button>
    </div>
    <div class="help">
      <p>Need help?</p>
      <p>+436641909445</p>
      <p>support@prime-crowd.com</p>
    </div>
  </div>
</template>
<style >
img {
  display: inline-block;
}
.active-icon {
  color: #ffffff;
}
li {
  width: 300px;
  height: 50px;
  padding-top: 14px;
  padding-bottom: 14px;
  padding-right: 41px;
  padding-left: 41px;
  font-family: Manrope;
  font-weight: 500;
  font-style: normal;
  font-size: 16px;
  line-height: 21.86px;
}
.active {
  color: #ffffff;
  background-color: #063847;
}
.icon {
  margin-right: 10px;
}
hr {
  position: relative;
  left: 8.33%;
  right: 8.33%;
  top: 28.27%;
  bottom: 71.63%;
  width: 250px;
  border: 1px solid #dfe9ec;
}
.recommendation,
.help {
  text-align: center;
}
.recommendation {
  width: 90%;
  height: 120px;
  margin-left: 10px;
  background: #00516c;
  color: #ffffff;
  padding: 15px;
  border-radius: 5px;
}
.invite {
  background-color: #ffffff;
  color: #25515e;
  text-align: center;
  font-size: 14px;
  width: 130px;
  border-radius: 5px;
}
.help {
  margin-top: 10px;
  width: 90%;
  margin-left: 10px;
  background: #dfe9ec;
  color: #76a1b0;
  border-radius: 5px;
}
</style>