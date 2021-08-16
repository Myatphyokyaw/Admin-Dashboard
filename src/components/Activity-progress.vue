<template>
<div>
  <div class="d-flex justify-content-center align-items-center">
    <RoundedCircle :color="this.circleColor" width="30px" height="30px"></RoundedCircle>

    <div class="w-100 ms-2">
      <div class="d-flex justify-content-lg-between mb-1">
        <small class="text-muted">{{ title }}</small>
        <small class="text-muted">{{ rate }}</small>
      </div>
      <div>
        <div class="progress">
          <div class="progress-bar" role="progressbar" :style="{width: this.progressWidth + '%',backgroundColor:this.progressColor,borderRadius:'1.5rem'}"  :aria-valuenow="this.progressWidth" aria-valuemin="0" aria-valuemax="100"></div>
        </div>
      </div>
    </div>
  </div>

</div>
</template>

<script>
import RoundedCircle from "@/components/Rounded-Circle";
export default {
  name: "Activity-progress",
  components: {RoundedCircle},
  data:function (){
    return{


    }
  },
  props:{
    title:String,
    rate:String,
    progressColor:String,
    progressWidth:String,
    circleColor:String,
  },
}
</script>

<style scoped>

</style>