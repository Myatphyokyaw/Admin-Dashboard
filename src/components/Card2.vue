<template>
  <div class="">
    <div class="card ">
      <div class="card-body shadow">

        <h3 class="text-center">$32,690</h3>
        <p class="text-center text-muted">Referral 40%</p>
        <div class="px-4">
         <chart2></chart2>
        </div>


      </div>
    </div>
  </div>
</template>

<script>
import Chart2 from "@/components/Chart2";
export default {
  name: "Card2",
  components: {Chart2}
}
</script>

<style scoped>

</style>