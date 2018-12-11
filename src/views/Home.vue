<template>
  <v-app>
    <v-content>
      <!-- <HelloWorld/> -->
    <MyComp msg_text="vue-bak" />
    </v-content>
      <Pano
           type='video'
            source="assets/video.mp4">
        </Pano>
  </v-app>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
import MyComp from "@/components/MyComp.vue"
import {Pano} from "vuejs-vr";

@Component({
  components: {
    HelloWorld,
    MyComp,
    Pano
  }
})
export default class Home extends Vue {}
</script>
