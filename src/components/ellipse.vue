<template>
<div>
    <canvas id="ellipse_component" class="ellipse" width="200" height="200">
    </canvas>
</div>

    
</template>

<script>
export default {
  name: 'ellipse',
  mounted() {
      console.log('mounted called');
      this.drawEllipse();
  },
  methods: {
      drawEllipse() {
        const canvas = document.getElementById('ellipse_component');
        const ctx = canvas.getContext('2d');

        // Draw the ellipse
        ctx.beginPath();
        ctx.ellipse(100, 100, 50, 75, Math.PI / 4, 0, 2 * Math.PI);
        ctx.stroke();

        // Draw the ellipse's line of reflection
        ctx.beginPath();
        ctx.setLineDash([5, 5]);
        ctx.moveTo(0, 200);
        ctx.lineTo(200, 0);
        ctx.stroke();
      }
  }
}
</script>

<style>

.ellipse {

    width: 400;
    height: 400;
}
</style>