<template>
  <header class="header">
    <nav class="burger">
      <button 
        class="burger__btn"
        @click="submit"
      ></button>
    </nav>

    <div @click="submit" ref="menu"></div>
    <div class="menu menu-display" ref="menuShow">
      <ul class="menu__items">
        <li class="menu__item">
          <a>Путешествия</a>
        </li>
        <li class="menu__item">
          <a>О нас</a>
        </li>
        <li class="menu__item">
          <a>Отзывы</a>
        </li>
        <li class="menu__item">
          <a>Блог</a>
        </li>
      </ul>
    </div>
  
  </header>
</template>

<script>
export default {
  name: 'Menu',
  data() {
    return {
      showMenu: false
    }
  },
  methods: {
    submit(){
      this.showMenu = !this.showMenu
      this.$refs.menu.classList.toggle('backdrop')
      this.$refs.menuShow.classList.toggle('menu-display')
    }
  }
}
</script>