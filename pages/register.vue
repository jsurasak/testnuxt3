<template>
  <div class="body-form">
    <p class="body-text-title">กรอกข้อมูล เพื่อสมัครสมาชิก</p>
    <form @submit.prevent="registerEvent" class="form-body">
      <InputTextVue placeholder="เบอร์โทรศัพท์" />
      <InputTextVue placeholder="รหัสผ่านของคุณ" />
      <InputTextVue placeholder="ยืนยันรหัสผ่านอีกครั้ง" />
      <SelectInputVue placeholder="เลือกบัญชีธนาคาร" />
      <InputTextVue placeholder="เลขบัญชีธนาคาร" />
      <InputTextVue placeholder="ชื่อจริง - นามสกุล" />
      <button type="submit" class="button-orange">สมัครสมาชิก</button>
    </form>
  </div>
</template>
<script setup>
import InputTextVue from "~~/components/form-input/InputText.vue";
import SelectInputVue from "~/components/form-input/SelectInput.vue";
const router = useRouter();

definePageMeta({
  layout: "layoutlogin",
});

const registerEvent = () => {
  router.push("/login");
};
</script>
