<template>
  <!-- Hero 4 - Bootstrap Brain Component -->
  <section class="" data-bs-theme="dark" style="background-color: #d3a34b;">
    <div class="container-fluid overflow-hidden">
      <div class="row">
        <div class="col-12 col-md-6 order-1 order-md-0 align-self-md-center">
          <div class="row py-3 py-sm-5 py-xxl-9 mt-md-16 justify-content-sm-center">
            <div class="col-12 col-sm-10">
          <canvas ref="canvas"></canvas>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 p-0">
          <img class="img-fluid w-100 h-100 object-fit-cover" loading="lazy" src="../../assets/akil2.jpg" alt="">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  import * as PIXI from 'pixi.js';

  export default {
    mounted() {
      const app = new PIXI.Application({
        view: this.$refs.canvas,
        width: 600,
        height: 150,
        backgroundColor: 0xd3a34b,
      });

      const text = new PIXI.Text('Calm your mind!', {
        fontFamily: 'Times New Roman',
        fontSize: 48,
        fill: 'white',
      });
      text.anchor.set(0.5);
      text.position.set(app.screen.width / 2, app.screen.height / 2);
      app.stage.addChild(text);

      const speed = 3;

      app.ticker.add(() => {
        text.position.x += speed;
        if (text.position.x > app.screen.width + text.width / 2) {
          text.position.x = -text.width / 2;
          
        }
      });
    },
  };
  </script>
