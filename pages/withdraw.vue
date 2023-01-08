<template>
  <div class="layout-content">
    <div class="layout-withdrow">
      <InputTextVue append-icon="ic_coin" />
      <button class="button-orange" @click="setShowPopup()">
        ยินยันการถอนเงิน
      </button>
    </div>
  </div>
  <PopupTopVue v-model="popup" />
</template>
<script setup>
import InputTextVue from "~/components/form-input/InputText.vue";
import PopupTopVue from "~/components/dialog/PopupTop.vue";
definePageMeta({
  title: "ถอนเงิน",
});

const popup = ref(false);

const setShowPopup = () => {
  popup.value = true;
};
</script>
