<template>
  <footer class="footer">
    <div class="container">
      <div class="footer-box">
        <router-link to="/" class="footer-logo logo">
          <img src="../assets/img/logo.png" alt="logo">
        </router-link>
        <div class="footer-nav">
          <ul>
            <li>Ресторанам</li>
            <li>Курьерам</li>
            <li>Пресс-центр</li>
            <li>Контакты</li>
          </ul>
        </div>
        <div class="footer-social">
          <img src="../assets/img/social/ig.png" alt="inst">
          <img src="../assets/img/social/fb.png" alt="fb">
          <img src="../assets/img/social/vk.png" alt="vk">
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer {
  display: flex;
  align-items: center;
  min-height: 156px;
  padding: 60px 0;
}

.footer-box {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 36px;
  height: 100%;
}

.footer-nav {
  flex-grow: 1;
}

.footer-nav ul {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  gap: 15px;
  margin: 0;
  padding: 0;
  list-style: none;
}

.footer-nav ul li {
  font-size: 18px;
  font-weight: 400;
  color: #595959;
}

.footer-social {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 20px;
}
</style>