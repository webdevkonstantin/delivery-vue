<template>
  <header class="header">
    <div class="container">
      <div class="header-box">
        <router-link to="/" class="header-logo logo">
          <img src="../assets/img/logo.png" alt="logo">
        </router-link>
        <div class="header-controls">
          <button class="btn btn-primary">
            <img src="../assets/img/icons/profile.png" alt="user">
            Войти
          </button>
          <button class="btn btn-outline" @click="openModal()">
            <img src="../assets/img/icons/cart.png" alt="cart">
            Корзина
          </button>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
  const emit = defineEmits(['toggleModal'])
  const openModal = () => emit('toggleModal')
</script>

<style scoped>
.header {
  display: flex;
  align-items: center;
  min-height: 124px;
}

.header-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100%;
}

.header-controls {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 10px;
}
</style>