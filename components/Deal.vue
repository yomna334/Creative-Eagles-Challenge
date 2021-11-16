<template>
  <div class="col">
    <img v-bind:src="deal.banner" />
    <p>2 days left</p>
    <p>{{ deal.title }}</p>
    <p>{{ deal.teaser }}</p>
    <button class="bg-hex-b2a8bb">{{ deal.status }}</button>
    <button class="bg-hex-b2a8bb">{{ deal.type }}</button>
  </div>
</template>
<script>
export default {
  props: ["deal"],
};
</script>
