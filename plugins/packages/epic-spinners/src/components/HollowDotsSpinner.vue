<template>
  <HollowDotsSpinner
    :animation-duration="animationDuration"
    :size="size"
    :color="color"
    :style="{
      position: 'absolute',
      left: (width - size) / 2 + 'px',
      top: (height - size) / 2 + 'px'
    }"
  />
</template>

<script>
import mixinComponent from "./MixinComponent";
import HollowDotsSpinner from "epic-spinners/src/components/lib/HollowDotsSpinner";

export default {
  name: "HollowDotsSpinnerWrapper",
  mixins: [mixinComponent],
  components: {
    HollowDotsSpinner
  }
};
</script>
