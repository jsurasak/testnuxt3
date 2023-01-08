<template>
  <div class="body-form">
    <p class="body-text-title">กรอกข้อมูล เพื่อเข้าสู่ระบบสมาชิก</p>
    <form @submit.prevent="loginEvent" class="form-body">
      <InputTextVue placeholder="เบอร์โทรศัพท์" />
      <InputTextVue placeholder="รหัสผ่านของคุณ" />
      <button type="submit" class="button-orange">เข้าสู่ระบบ</button>
      <router-link to="/register" class="button-orange-rounder" tag="button"
        >สมัครสมาชิก</router-link
      >
    </form>
  </div>
</template>
<script setup>
import InputTextVue from "~~/components/form-input/InputText.vue";
// const route = useRoute();
const router = useRouter();

const loginEvent = () => {
  router.push("/");
};

definePageMeta({
  layout: "layoutlogin",
});
</script>
