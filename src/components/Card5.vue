<template>
  <div class="d-flex flex-column justify-content-between mt-4 h-100">
    <div>
      <div class="card mt-3 mt-lg-0">
        <div class="card-body shadow">


          <div class="p-1">
            <div class="d-flex align-items-center justify-content-between">

              <RoundedCircle color="#dee8fc" width="40px" height="40px"></RoundedCircle>


              <div>

                <h5>$38,566</h5>
                <p class="m-0 text-muted">Conversion</p>
              </div>
              <div class="">

                <chart5></chart5>

              </div>
            </div>

          </div>


        </div>
      </div>
    </div>
    <div>
      <div class="card mt-3 mt-lg-0">
        <div class="card-body shadow">


          <div class="p-1">
            <div class="d-flex align-items-center justify-content-between">
              <div class="text-center rounded-circle"
                   style="width: 40px;height: 40px;line-height: 40px;background-color: #ffead3">
                <i class="feather-dollar-sign text-warning"></i>
              </div>
              <div>

                <h5>$53,659</h5>
                <p class="m-0 text-muted">Income</p>
              </div>
              <div class="">

                <chart6></chart6>

              </div>
            </div>

          </div>


        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Chart5 from "@/components/Chart5";
import Chart6 from "@/components/Chart6";
import RoundedCircle from "@/components/Rounded-Circle";

export default {
  name: "Card5",
  components: {RoundedCircle, Chart6, Chart5}
}
</script>

<style scoped>

</style>