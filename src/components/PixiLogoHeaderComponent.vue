<template>
  <canvas ref="pixiContainer"></canvas>
</template>

<script>
import * as PIXI from 'pixi.js';

export default {
  mounted() {
    const app = new PIXI.Application({
      view: this.$refs.pixiContainer,
      width: 200, 
      height: 150, 
      backgroundColor: 0xFFFFFF,
    });

    const sprite = PIXI.Sprite.from(
      'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQXXCMTOaMO660FONULKLX_Uxe0MsG3DuiufHuoMsvif0_cNiklb_C65lnQjtM81uVDu_A&usqp=CAU'
    );
    sprite.anchor.set(0.5);

    sprite.position.set(app.screen.width / 2, app.screen.height / 2);

    const maxDimension = Math.max(sprite.width, sprite.height);
    const scaleFactor = Math.min(app.screen.width, app.screen.height) / maxDimension;
    sprite.scale.set(scaleFactor);

    app.stage.addChild(sprite);

    app.ticker.add(() => {
      sprite.rotation += 0.01;
    });
  },
};
</script>