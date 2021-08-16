<template>
  <div>
    <div class="card mt-4 mt-lg-0">
      <div class="card-body shadow  p-4">

        <h6>Activity</h6>
        <ActivityProgress class="my-4" progress-color="var(--bs-primary)" rate="$8,125" progress-width='42' title="Total Sales" circle-color="rgba(90,141,238,.2)"></ActivityProgress>
        <ActivityProgress class="my-4" progress-color="#39da8a" rate="$18,963" progress-width="80" title="Income Amount" circle-color="rgba(57,218,138,.2)"></ActivityProgress>
        <ActivityProgress class="my-4" progress-color="#fdac41" rate="$14,150" progress-width="50" title="Total Budget" circle-color="rgba(253,172,65,.2)"></ActivityProgress>
        <ActivityProgress class="my-4" progress-color="#ff5b5c" rate="106" progress-width="90" title="Completed Tasks" circle-color="rgba(255,91,92,.2)"></ActivityProgress>
      </div>
    </div>
  </div>
</template>

<script>


import ActivityProgress from "@/components/Activity-progress";

export default {
  name: "Card6",
  components: {ActivityProgress},
}
</script>

<style scoped>

</style>