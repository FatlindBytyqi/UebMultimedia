<template>
  <!-- About 2 - Bootstrap Brain Component -->
  <section class="bg-light py-5 py-xl-8">
    <div class="container">
      <div class="row gy-5 gy-lg-0 gx-lg-6 gx-xxl-8 align-items-lg-center">
        <div class="col-12 col-lg-6 order-lg-first">
          <video class="video-fluid rounded" controls autoplay loop muted width="600" height="600"> 
            <source src="../assets/judoVideo.mp4" type="video/mp4">
          </video>
        </div>
        <div class="col-12 col-lg-6">
          <canvas ref="canvas"></canvas>
          <p class="lead fs-4 text-secondaryX mb-5">Judo is a martial art that can be practiced and enjoyed at any age. Whether you start as a child or an adult, you can continue to learn and progress throughout your life. Judo offers a path of continual self-improvement, allowing individuals to set and achieve new goals.</p>
          <div class="d-flex align-items-center mb-3">
            <div class="me-3 text-primary">
              <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" fill="currentColor" class="bi bi-check-circle-fill" viewBox="0 0 16 16">
                <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z" />
              </svg>
            </div>
            <div>
              <p class="fs-5 m-0">Character development</p>
            </div>
          </div>
          <div class="d-flex align-items-center mb-3">
            <div class="me-3 text-primary">
              <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" fill="currentColor" class="bi bi-check-circle-fill" viewBox="0 0 16 16">
                <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z" />
              </svg>
            </div>
            <div>
              <p class="fs-5 m-0">Lifelong learning</p>
            </div>
          </div>
          <div class="d-flex align-items-center mb-5">
            <div class="me-3 text-primary">
              <svg xmlns="http://www.w3.org/2000/svg" width="28" height="28" fill="currentColor" class="bi bi-check-circle-fill" viewBox="0 0 16 16">
                <path d="M16 8A8 8 0 1 1 0 8a8 8 0 0 1 16 0zm-3.97-3.03a.75.75 0 0 0-1.08.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-.01-1.05z" />
              </svg>
            </div>
            <div>
              <p class="fs-5 m-0">Mental discipline</p>
            </div>
          </div>
          <button type="button" class="btn btn-outline-primary btn-2xl rounded-pill px-4 gap-3">Enroll Now</button>
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
      width: 800,
      height: 600,
      backgroundColor: 0xf8f9fa,
    });

    const textStyle = new PIXI.TextStyle({
      fontFamily: 'Arial',
      fontSize: 48,
      fill: 'black', 
      fontWeight: 'bold',
    });

    const text = new PIXI.Text('What is Judo?', textStyle);
    text.anchor.set(0.5);
    text.position.set(app.screen.width / 2, app.screen.height / 2);
    app.stage.addChild(text);

    const amplitude = 20;
    const frequency = 0.002;
    const initialY = text.position.y;

    app.ticker.add((delta) => {
      const time = performance.now() * frequency;
      const displacement = Math.sin(time) * amplitude;
      text.position.y = initialY + displacement;
    });
  },
};
</script>
