<template>
  <div style="height: 40px;width: 70px">
    <canvas id="my-chart5" ></canvas>
  </div>
</template>

<script>
import Chart from "chart.js";

export default {
  name: "Chart5",
  data(){

    return{

      chartData: {

        type: 'line',
        data: {
          labels: ['Jan', 'Feb', 'Mar', 'Apr', 'Aug', 'Sep'],
          datasets: [{


            data: [50, 100, 0, 60, 20, 30],
            backgroundColor: [
              'rgba(255,255,255,0)',
            ],
            borderColor: [
              '#6ce5a9',
            ],
            borderWidth: 3,
            tension: 0.4,
            pointRadius: 1,
          }]
        },
        options: {

          maintainAspectRatio: false,

            legend: {

              display: false,
              labels: {
                color: 'rgb(255, 99, 132)'
              }
            },


          scales: {
            xAxes: [{

              display:false

            }],
            yAxes: [{

              display:false

            }]

          }
        }

      }
    }
  },
  mounted() {
    const ctx = document.getElementById('my-chart5');
    new Chart(ctx,this.chartData)
  }
}
</script>

<style scoped>

</style>