<template>
<div class="full-width padded app-bar">
  <div class="titles">
    <div class="title col centered">Henri Le Page</div>
    <div class="subtitle col centered">Aux âmes bien nées, le génie n'attend pas le nombre des années</div>
  </div>
  <div>
    <div v-for="route in routes">
      <router-link to={route.path} v->{{route.name}}</router-link>
    </div>
  </div>
</div>
</template>

<script lang="ts">
import {
	Component,
	Prop,
	Vue
} from 'vue-property-decorator'

@Component
export default class AppBar extends Vue {
	// @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.app-bar {
  background-color: lightgreen;
  border-bottom: 1px solid grey;
}

.titles {
  display: grid;
  grid-template-columns: 1fr 2fr;
}

.title {
  font-size: 2rem;
}

.subtitle {
  color: grey;
}
</style>
