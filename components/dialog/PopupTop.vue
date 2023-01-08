<template>
  <div class="modal-overlay" v-if="props.modelValue">
    <div class="modal">
      <p class="model-text-title">ยินยันการถอน</p>
      <p class="model-text-subtitle">โปรดตรวจสอบการทำรายการทุกครั้งเสมอ</p>
      <InputTextVue append-icon="ic_coin" />
      <div class="popup-action">
        <button class="button-white" @click="closePopup">ยกเลิกรายการ</button>
        <button class="button-orange" @click="closePopup">
          ยืนยันทำรายการ
        </button>
      </div>
    </div>
  </div>
</template>
<script setup>
import InputTextVue from "../form-input/InputText.vue";

const props = defineProps({
  modelValue: Boolean,
});

const emit = defineEmits(["update:modelValue"]);

const closePopup = () => {
  emit("update:modelValue", false);
};
</script>
<style lang="scss" scoped>
@import "~/assets/scss/color.scss";
@import "~/assets/scss/text.scss";
.modal-overlay {
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: #000000da;
  animation: fadein 0.5s;
  .modal {
    text-align: center;
    background-color: $black-base;
    border: 1px solid $border-input;
    border-radius: 10px;
    margin: 90px 30px 0 30px;
    padding: 20px;
    .model-text-title {
      @include text-lg-bold;
      color: $white;
    }
    .model-text-subtitle {
      @include text-md;
      color: $gray;
      margin-bottom: 20px;
    }

    .popup-action {
      display: flex;
      button {
        flex: 1 1 auto;
        &:first-child {
          margin-right: 10px;
        }
        &:last-child {
          margin-left: 10px;
        }
      }
    }
  }
}
@keyframes fadein {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
</style>
