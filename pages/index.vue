<template>
  <NuxtLayout name="default">
    <template #left-header-bar>
      <img src="@/assets/images/logo.png" width="100" alt="" />
    </template>
    <template #center-header-bar>
      <div></div>
    </template>
    <div class="layout-content">
      <div class="layout-content-botton-top">
        <button class="button-orange">
          <img src="@/assets/icons/ic_money_box.svg" alt="" />
          <span>ฝากเงิน</span>
        </button>
        <button class="button-orange-rounder">
          <img src="@/assets/icons/ic_atm.svg" alt="" />
          <span>ถอนเงิน</span>
        </button>
      </div>
      <div class="layout-content-menu">
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_money_box.svg" class="color-orange" />
          </div>
          <div class="text-menu">ฝากเงิน</div>
        </div>
        <nuxt-link to="/withdraw" tag="div" class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_atm.svg" />
          </div>
          <div class="text-menu">ถอนเงิน</div>
        </nuxt-link>
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_history.svg" />
          </div>
          <div class="text-menu">ประวัติ</div>
        </div>
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_friend.svg" />
          </div>
          <div class="text-menu">แนะนำเพื่อน</div>
        </div>
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_cashback.svg" />
          </div>
          <div class="text-menu">รับเงินคืน</div>
        </div>
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_bonus.svg" />
          </div>
          <div class="text-menu">รับโบนัส</div>
        </div>
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_cashback.svg" />
          </div>
          <div class="text-menu">รับเครดิตฟรี</div>
        </div>
        <div class="content-menu">
          <div class="box-img-menu">
            <img src="@/assets/icons/ic_contact_us.svg" />
          </div>
          <div class="text-menu">ติดต่อเรา</div>
        </div>
      </div>
      <div class="layout-content-game">
        <div class="layout-menu-game">
          <button class="menu-game activity">คาสิโนสด</button>
          <button class="menu-game">สล็อต</button>
          <button class="menu-game">เกมส์</button>
          <button class="menu-game">หวย</button>
        </div>
        <div class="layout-list-game">
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_1.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_2.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_3.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_4.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_5.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_6.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_7.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_8.png" alt="" />
            </div>
          </div>
          <div class="layout-box-game">
            <div class="box-list-game">
              <img src="@/assets/images/logo_game_9.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </NuxtLayout>
</template>
<script setup>
definePageMeta({
  layout: false,
  title: "Home",
});
</script>
