<template>
  <div>
    <div class="card">
      <div class="card-body shadow">
        <div class="d-flex align-items-center justify-content-between">
          <div>
            <h6>Conversion</h6>
            <div class="d-flex align-items-center">
              <p class="m-0">60%</p>
              <i class="feather-trending-up ms-1" style="color: #6ce5a9"></i>
            </div>
          </div>

          <div>
            <h3>89K</h3>
          </div>
        </div>
        <div class="mt-3">
          <chart4></chart4>
        </div>


      </div>
    </div>
  </div>
</template>

<script>
import Chart4 from "@/components/Chart4";
export default {
  name: "Card4",
  components: {Chart4}
}
</script>

<style scoped>

</style>