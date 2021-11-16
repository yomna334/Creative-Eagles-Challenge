<template>
<div class="dealsList">
    <div class="flex">
    <Deal class="w-80 deal" v-for="(deal,index) in deals" :key="index"  :deal="deal"/>
    </div>
</div>
</template>
<script>
import * as axios from 'axios';

export default {
    data(){
        return {
            deals:[]
        }
    },
    mounted(){
        this.getDeals();
    }
,
methods:{
    async getDeals(){
        let {data} = await axios.get('https://prime-crowd.com/api/mock/rounds');
        this.deals=data;
    }
}
}
</script>
<style>
.dealsList{
    height: 1024px;
    background-color: #F4F7F9;
}.deal{
    background-color: #FFFFFF;
    margin: 20px;
border-radius: 5px 5px 0px 0px;
}
</style>