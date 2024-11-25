<template>
  <div id='Menu'>
    <nav class="navbar navbar-expand-lg navbar-dark ftco_navbar ftco-navbar-light" id="ftco-navbar">
      <div class="container justify-content-end">
        <a class="navbar-brand"><span class="flaticon-pizza-1 mr-1"></span><small>Donut SHOP</small></a>

        <button class="navbar-toggler" type="button" @click="toggleMenu" aria-controls="ftco-nav" :aria-expanded="isMenuOpen.toString()" aria-label="Toggle navigation">
          <span class="oi oi-menu"></span> Menu
        </button>

        <div :class="['collapse', 'navbar-collapse', { 'show': isMenuOpen }]" id="ftco-nav">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <router-link to="/" class="nav-link" active-class="active">หน้าแรก</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/Product" class="nav-link" active-class="active">เมนู</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/About" class="nav-link" active-class="active">เกี่ยวกับฉัน</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/Contact" class="nav-link" active-class="active">ติดต่อ</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Menu',
  data() {
    return {
      isMenuOpen: false 
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen; 
    }
  }
}
</script>

<style scoped>
.navbar {
  background-color: #06aace;
}
</style>
