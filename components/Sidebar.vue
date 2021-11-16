<template>
  <div class="sidebar">
    <img src="../static/Logo.png" alt="logo" />
    <ul>
      <li>
        <span><img src="../static/Combined Shape.svg" />Cockpit</span>
      </li>
      <li class="active">
        <img class="active-icon" src="../static/Combined Shape.svg" />Investment
        Opportunities
      </li>
      <li><img src="../static/Combined Shape.svg" />My Investments</li>
      <hr class="border-solid" />
      <li><img src="../static/Combined Shape.svg" />Knowledge Center</li>
      <li><img src="../static/Combined Shape.svg" />Venture Pool</li>
      <li><img src="../static/Combined Shape.svg" />Fee Model</li>
    </ul>
  </div>
</template>
<style>
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
  padding-left: 65px;
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
hr {
  position: relative;
  left: 8.33%;
  right: 8.33%;
  top: 28.27%;
  bottom: 71.63%;
  width: 250px;
  border: 1px solid #dfe9ec;
}
</style>