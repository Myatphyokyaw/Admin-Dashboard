<template>
  <div >
    <canvas id="my-chart" height="275px"></canvas>
  </div>
</template>

<script>



import Chart from 'chart.js'
export default {

name:"Chart1",
  data(){

  return{

    chartData: {

      type: 'bar',

      data: {
        labels:['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep'],
        datasets: [{
          label: 'User',
          barThickness: 7,
          borderRadius: 50,
          barPercentage: 0.5,
          data: [120, 95, 210, 220, 290, 280, 110, 200, 140, 180],
          backgroundColor: [
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',
            'rgba(90,141,238,0.81)',

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
            barThickness: 7,

            data: [100, 70, 180, 200, 250, 120, 150, 70, 45, 90, 120],
            backgroundColor: [
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',
              'rgba(90,141,238,0.63)',

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

          },

        scales: {
          xAxes: [{

            display:false

          }],
          yAxes: [{

            display:true

          }]
        }

      }

    }
    }
  },
  mounted() {
    const ctx = document.getElementById('my-chart');
    new Chart(ctx,this.chartData)
  }
}
</script>

<style>

</style>