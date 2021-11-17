<template>
  <div class="dealsList">
    <div class="btns">
      <button :class="'all ' + (tab == 'all' ? 'active-tab' : '')" v-on:click="tab = 'all'">All</button>
      <button :class="(tab == 'active' ? 'active-tab' : '')" v-on:click="tab = 'active'">Active</button>
      <button :class="(tab == 'comingSoon' ? 'active-tab' : '')" v-on:click="tab = 'comingSoon'">Coming Soon</button>
      <hr class="underLine" />
    </div>
    <div class="flex" v-if="tab == 'all'">
      <Deal
        class="w-80 deal"
        v-for="(deal, index) in deals"
        :key="index"
        :deal="deal"
      />
    </div>
    <div class="flex" v-if="tab == 'active'">
      <Deal
        class="w-80 deal"
        v-for="(deal, index) in activeDeals"
        :key="index"
        :deal="deal"
      />
    </div>
    <div class="flex" v-if="tab == 'comingSoon'">
      <Deal
        class="w-80 deal"
        v-for="(deal, index) in comingSoonDeals"
        :key="index"
        :deal="deal"
      />
    </div>
  </div>
</template>
<script>
import * as axios from "axios";

export default {
  data() {
    return {
      tab: "all",
      deals: [],
    };
  },
  mounted() {
    this.getDeals();
  },
  computed: {
    activeDeals() {
      return this.deals.filter((item) => item.status == "active");
    },

    comingSoonDeals() {
      return this.deals.filter((item) => item.status == "coming_soon");
    },
  },
  methods: {
    async getDeals() {
      let { data } = await axios.get("https://prime-crowd.com/api/mock/rounds");
      this.deals = data;
      console.log(this.deals);
    },
  },
};
</script>
<style >
.btns{
  padding-top:30px ;
}
button {
  border: none;
  margin-right: 30px;
}
.all{
  margin-left: 20px;
}
.underLine {
 margin-top:10px ;
width:95%;
  border: 1px solid #dfe9ec;
      left: 9px;

}
.dealsList {
  height: 1024px;
  background-color: #f4f7f9;
}
.deal {
  position: relative;
  left: 80px;
  background-color: #ffffff;
  margin: 20px;
  border-radius: 5px 5px 0px 0px;
}
.active-tab{
  border-bottom:2px solid #063847;
 ;
}
</style>