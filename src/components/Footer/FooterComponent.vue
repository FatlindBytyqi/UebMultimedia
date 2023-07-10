<template>
  <footer class="footer">
    <section>
      <div class="container-fluid">
        <div class="row">
          <LeftSideFooter />
          <RightSideFooter />
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
import LeftSideFooter from './LeftSideFooter.vue';
import RightSideFooter from './RightSideFooter.vue';

export default {
  components: {
    LeftSideFooter,
    RightSideFooter
  }
};
</script>
