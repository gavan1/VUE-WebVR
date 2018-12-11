<template>
  <div class="mycomp">
    <h1>BOOM: {{ msg_text }}</h1>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";



@Component
export default class MyComp extends Vue {
  @Prop() private msg_text!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h1 {
  padding-top: 10px;
}
</style>
