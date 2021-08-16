<template>
  <div>
    <canvas id="small" class="my-3" style="height: 40px"></canvas>
  </div>
</template>

<script>
import Chart from "chart.js";
export default {
  name: "small-chart",
  data() {

    return {

      chartData: {

        type: 'doughnut',
        data: {
          datasets: [{
            label: '# of Votes',
            data: [50, 50],
            backgroundColor: [
              'rgba(90,141,238,0.81)',
              '#f2f4f4',


            ],
            borderColor: [
              'rgba(90,141,238,0.81)',
              '#f2f4f4',


            ],
            borderWidth: 1,

          }]
        },
        options: {



          cutoutPercentage: 80,
          legend: {

            fontsize: 40,
            labels: {

              usePointStyle: true,

            },

            position: 'bottom',


          },

          scales: {
            y: {
              beginAtZero: true,
              display: false
            }
          }
        }

      }
    }
  },
  mounted() {
    const ctx = document.getElementById('small-chart');
    new Chart(ctx, this.chartData)
  }
}
</script>

<style scoped>

</style>