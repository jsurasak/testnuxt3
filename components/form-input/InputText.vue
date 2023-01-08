<template>
  <div class="inputForm">
    <img v-if="appendIcon" class="append-icon" :src="images[appendIcon]" />
    <input :placeholder="placeholder" type="text" name="" id="" />
  </div>
</template>
<script>
import { filename } from "pathe/utils";
export default {
  props: {
    placeholder: String,
    appendIcon: String,
  },
  setup(props) {
    const { placeholder, appendIcon } = props;

    const glob = import.meta.glob("~/assets/icons/*.svg", { eager: true });
    const images = Object.fromEntries(
      Object.entries(glob).map(([key, value]) => [filename(key), value.default])
    );

    return {
      placeholder,
      images,
      appendIcon,
    };
  },
};
</script>
