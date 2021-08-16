<template>
  <div>
    <canvas id="my-chart3" class="my-3" style="height: 175px" ></canvas>
  </div>
</template>

<script>
import Chart from "chart.js";

export default {
  name: "Chart3",
  data(){

    return{

      chartData: {

        type: 'doughnut',
        data: {
          labels: ['Social', 'Email', 'Search'],
          datasets: [{
            label: '# of Votes',
            data: [80, 30, 60],
            backgroundColor: [
              'rgba(90,141,238,0.81)',
              'rgba(109,219,13,0.93)',
              '#fdac41',


            ],
            borderColor: [
              'rgba(90,141,238,0.81)',
              'rgba(109,219,13,0.93)',
              'rgba(255, 206, 86, 1)',

            ],
            borderWidth: 1,

          }]
        },
        options: {

          maintainAspectRatio: false,


          cutoutPercentage:90,

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
        },


      }

    }
  },
  mounted() {
    const ctx = document.getElementById('my-chart3');
    new Chart(ctx,this.chartData)
  }
}
</script>

<style scoped>

</style>