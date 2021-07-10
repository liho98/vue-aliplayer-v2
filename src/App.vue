<template>
  <ali-player-v3
    :source="source"
    :options="options"
    class="h-64 md:h-96 w-full rounded-lg"
    style="height: 20rem; width: 100%; border-radius: 1rem"
  />
</template>

<script>
import AliPlayerV3 from "@/components/AliPlayerV3.vue";

export default {
  name: "App",
  components: {
    AliPlayerV3,
  },
  setup(props, context) {
    return {};
  },
  data() {
    return {
      source: "//player.alicdn.com/video/aliyunmedia.mp4",
      options: {
        isLive: false, //切换为直播流的时候必填
        // format: 'm3u8'  //切换为直播流的时候必填
      },
    };
  },
};
</script>
