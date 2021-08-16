<template>
  <div>
    <div class="my-2" style="max-height: 60px;">
      <canvas id="my-chart2" ></canvas>
    </div>

  </div>
</template>

<script>
import Chart from "chart.js";

export default {
  name: "Chart2",
  data(){

    return{

      chartData: {

        type: 'line',
        data: {
          labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep','Oct'],
          datasets: [{


            data: [50, 20, 50, 40, 50, 20, 40, 25, 60, 45,40],
            backgroundColor: [
             '#fff8'
            ],
            borderColor: [
              '#6ce5a9',
            ],
            borderWidth: 3,
            tension: 0.25,
            pointRadius: 1,
          }]
        },
        options: {


          maintainAspectRatio: false,
            legend: {
              display: false,
            },


          scales: {
            xAxes: [{

                display:false

            }],
            yAxes: [{

                display:false,

            }]
          }
        }

      }
    }
  },
  mounted() {
    const ctx = document.getElementById('my-chart2');
    new Chart(ctx,this.chartData)
  }
}
</script>

<style scoped>
#my-chart2{

}
</style>