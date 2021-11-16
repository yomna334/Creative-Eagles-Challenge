<template>
  <div class="container mx-auto">
    <div class="flex">
      <div class="w-75">
        <Sidebar />
      </div>
      <div class="flex-1">
        <Navbar/>
        <DealsList />
      </div>
    </div>
  </div>
</template>

<script>
import DealsList from "~/components/DealsList.vue";
import Sidebar from "~/components/Sidebar.vue";
import Navbar from "~/components/Navbar.vue";
export default { components: { DealsList, Sidebar, Navbar } };
</script>
<style>
*{
  overflow: hidden;
}
</style>
