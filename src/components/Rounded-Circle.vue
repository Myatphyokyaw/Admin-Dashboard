<template>
  <div class="text-center rounded-circle"
       :style="{backgroundColor: bgcolor,width:circleWidth,height:circleHeight}">
    <i class="feather-dollar-sign text-warning"></i>
  </div>
</template>

<script>
export default {
  name: "Rounded-Circle",
  props: ['color','width','height'],
  data() {
    return {
      bgcolor: this.color,
      circleWidth: this.width,
      circleHeight: this.height,



    }
  },


}
</script>

<style scoped>

</style>