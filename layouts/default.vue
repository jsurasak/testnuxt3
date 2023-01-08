<template>
  <header class="header-content">
    <div class="header-bar">
      <slot name="left-header-bar">
        <p class="back-button" @click="eventBack">ย้อนกลับ</p>
      </slot>
      <slot name="center-header-bar">
        <p class="text-header-bar">{{ route.meta.title }}</p>
      </slot>
      <slot name="right-header-bar">
        <img
          @click="eventPageProfile"
          src="@/assets/icons/ic_user.svg"
          class="btn_profile"
        />
      </slot>
    </div>
    <slot name="body-content">
      <div class="body-bar">
        <div class="body-bar-left">
          <div class="body-bar-title">เครดิตทั้งหมด</div>
          <div class="body-bar-content">450,000.00</div>
        </div>
        <div class="body-bar-right">
          <div class="body-bar-title">ค่าแนะนำ</div>
          <div class="body-bar-content">1,200.00</div>
        </div>
      </div>
    </slot>
  </header>
  <div class="body-content">
    <slot />
  </div>
  <footer class="footer-content">
    <p>*หากมีข้อสงสัย กรุณาติดต่อ ฝ่ายบริการลูกค้า</p>
  </footer>
</template>
<script setup>
const route = useRoute();
const router = useRouter();

const eventBack = () => {
  router.back();
};

const eventPageProfile = () => {
  router.push({ path: "/profile" });
};

useHead({
  title: route.meta.title,
});
</script>
