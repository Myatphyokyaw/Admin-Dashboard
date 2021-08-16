<template>
  <div>
    <div class="d-flex flex-column justify-content-between h-100">
      <div>
        <div class="card mt-3 mt-lg-0">
          <div class="card-body shadow">


            <div class="p-1">
              <div class="d-flex align-items-center justify-content-between">


                <div>

                  <h6 class="">Profit Report</h6>
                  <div class="d-flex justify-content-center">
                    <div class="d-flex justify-content-center align-items-center">
                      <SmallChart></SmallChart>
                      <div>
                        <h5 class="m-0">$12k</h5>
                        <small class="text-muted">2020</small>
                      </div>

                    </div>
                    <div class="d-flex justify-content-center align-items-center">
                      <SmallChart></SmallChart>
                      <div>
                        <h5 class="m-0">$12k</h5>
                        <small class="text-muted">2020</small>
                      </div>

                    </div>
                  </div>


                </div>
                <div class="">


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


              <div>

                <h6>Registrations</h6>
                <div>
                  <div>
                    <h4 class="text-muted">56.3k</h4>
                    <font-awesome-icon :icon="['fas','chart-pie']"/>
                  </div>

                </div>

              </div>


            </div>


          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>

import SmallChart from "@/components/Small-Chart";

export default {
  name: "Card7",
  components: {SmallChart},
}
</script>

<style scoped>

</style>