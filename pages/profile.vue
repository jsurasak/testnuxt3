<template>
  <NuxtLayout name="default">
    <template #right-header-bar>
      <div></div>
    </template>
    <template #body-content>
      <div class="body-bar-profile">
        <div class="body-bar-profile-name">
          <span>วิชกานต์ พลชำนิ</span>
          <img src="@/assets/icons/ic_verified.svg" alt="" />
        </div>
        <div class="body-bar-profile-coode">
          <span class="body-bar-profile-title">USER : </span>
          <span class="body-bar-profile-code">XOLP6991577</span>
        </div>
      </div>
    </template>
    <div class="layout-content">
      <div class="layout-profile-menu">
        <div class="layout-profile-menu-items">
          <div class="items-box-icon">
            <img src="@/assets/icons/ic_profile.svg" alt="" />
          </div>
          <div class="items-box-content">
            <span>ตั้งค่าโปรไฟล์</span>
          </div>
          <div class="items-box-action">
            <img src="@/assets/icons/ic_arrow_right.svg" alt="" />
          </div>
        </div>
        <div class="layout-profile-menu-items">
          <div class="items-box-icon">
            <img src="@/assets/icons/ic_history_money.svg" alt="" />
          </div>
          <div class="items-box-content">
            <span>ประวัติการเงิน</span>
          </div>
          <div class="items-box-action">
            <img src="@/assets/icons/ic_arrow_right.svg" alt="" />
          </div>
        </div>
        <div class="layout-profile-menu-items">
          <div class="items-box-icon">
            <img src="@/assets/icons/ic_bank.svg" alt="" />
          </div>
          <div class="items-box-content">
            <span>ธนาคารของคุณ</span>
          </div>
          <div class="items-box-action">
            <img src="@/assets/icons/ic_arrow_right.svg" alt="" />
          </div>
        </div>
        <div class="layout-profile-menu-items">
          <div class="items-box-icon">
            <img src="@/assets/icons/ic_contact.svg" alt="" />
          </div>
          <div class="items-box-content">
            <span>ติดต่อผู้ดูแล</span>
          </div>
          <div class="items-box-action">
            <img src="@/assets/icons/ic_arrow_right.svg" alt="" />
          </div>
        </div>
      </div>
    </div>
  </NuxtLayout>
</template>
<script setup>
definePageMeta({
  layout: false,
  title: "ข้อมูลผู้ใช้งาน",
});
</script>
