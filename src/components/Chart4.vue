<template>
  <div style="max-height: 82px;">
    <canvas id="my-chart4" ></canvas>
  </div>
</template>

<script>
import Chart from "chart.js";

export default {
  name: "Chart4",
  data(){

    return{

      chartData: {


        type: 'bar',

        data: {
          labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep'],
          datasets: [{
            label: 'User',
            barThickness: 5,
            borderRadius: 50,
            barPercentage: 0.5,
            data: [120, 95, 210, 220, 290, 280, 110, 200, 140, 180],
            backgroundColor: [
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',
              'rgb(90,141,238)',

            ],
            borderColor: [
              '#fff',
              '#fff',
              '#fff',
              '#fff',
              '#fff',
              '#fff',
              '#fff',
              '#fff',
              '#fff',

            ],
            borderWidth: 0.5
          },
            {

              label: 'Viewer',
              borderRadius: 50,
              barThickness: 5,

              data: [100, 70, 180, 200, 250, 120, 150, 70, 45, 90, 120],
              backgroundColor: [
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',
                'rgb(245,194,9)',

              ],
              borderColor: [
                '#fff',
                '#fff',
                '#fff',
                '#fff',
                '#fff',
                '#fff',
                '#fff',
                '#fff',
                '#fff',

              ],
              borderWidth: 0.5
            }

          ]
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

            label: {
              display: false
            },

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
    const ctx = document.getElementById('my-chart4');
    new Chart(ctx,this.chartData)
  }
}
</script>

<style scoped>

</style>