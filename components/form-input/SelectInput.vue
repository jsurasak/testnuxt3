<template>
  <div class="select-inputForm">
    <select>
      <option>{{ placeholder }}</option>
      <option>Items 1</option>
      <option>Items 2</option>
      <option>Items 3</option>
    </select>
  </div>
</template>
<script>
export default {
  props: {
    placeholder: String,
  },
  setup(props) {
    const { placeholder } = props;

    return {
      placeholder,
    };
  },
};
</script>
