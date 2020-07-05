<template>
  <div class="col full-width padded app-bar">
    <div class="title">Henri Le Page</div>
    <div class="subtitle">Aux âmes bien nées, le génie n'attend pas le nombre des années</div>

  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class AppBar extends Vue {
  // @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .app-bar {
    background-color: lightgreen;
    display: grid;
    grid-template-columns: 30rem 30% 1fr;
  }

  .title {
    font-size: 2rem;
  }

  .subtitle {
    font-style: 1rem;
  }
</style>
