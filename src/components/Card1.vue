<template>
  <div>
    <div class="card">
      <div class="card-body shadow">
        <h6>Website Analytics</h6>

        <div class="row pe-4 p-lg-2">
          <div class="col-4 col-lg-4">
            <div class="">
              <div class="d-flex align-items-center text-muted">


                <i class="far fa-user me-3"></i>
                <p class="m-0">Users</p>
              </div>
              <div class="mt-3 d-flex">
                <i class="feather-pie-chart fs-2 text-success me-3"></i>
                <h3 class="">61K</h3>
              </div>
            </div>
          </div>
          <div class="col-4 col-lg-4">
            <div class="">
              <div class="d-flex align-items-center text-muted">
                <i class="feather-trending-up me-3"></i>
                <p class="m-0">Sessions</p>
              </div>
              <div class="mt-3 d-flex">
                <i class="feather-pie-chart fs-2 text-warning me-3"></i>
                <h3>92K</h3>
              </div>
            </div>
          </div>
          <div class="col-4 col-lg-4">
            <div class="">
              <div class="d-flex align-items-center text-muted ">
                <i class="feather-clock me-3"></i>
                <p class="m-0 text-black-50">Bounce</p>
              </div>
              <div class="mt-3 d-flex">
                <i class="feather-pie-chart fs-2 text-danger me-3"></i>
                <h3>72.6%</h3>
              </div>
            </div>
          </div>

        </div>
        <div class="mt-3">
          <chart1></chart1>

        </div>


      </div>
    </div>
  </div>
</template>

<script>
import Chart1 from "@/components/Chart1";
export default {
  name: "Card1",
  components: {Chart1}
}
</script>

<style scoped>

</style>