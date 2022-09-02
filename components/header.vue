<template>
  <header class="header">
    <nav class="nav container">
      <a href="#" class="nav__logo">Abel</a>
      <div class="nav__menu">
        <ul class="nav__list grid">
          <template v-for="menu in menuItems">
            <li class="nav__item">
              <a href="#home" class="nav__link active-link" @click="linkAction">
                <icon name="" class="uil uil-estate nav__icon"/>
                {{ menu.name }}
              </a>
            </li>
          </template>
        </ul>
        <i class="uil uil-times nav__close" @click="navClose" id="nav-close"/>
      </div>

      <div class="nav__btns">
        <!--Theme change button-->
        <i class="uil uil-moon change-theme" id="theme-button"></i>

        <div class="nav__toggle" @click="navToggle" id="nav-toggle">
          <i class="uil uil-apps"/>
        </div>
      </div>
    </nav>
  </header>
</template>

<script setup>
import {ref} from 'vue'

const menuItems = ref([
  {
    name: 'Home',
    icon: '',
    link: ''
  },
  {
    name: 'About',
    icon: '',
    link: ''
  },
  {
    name: 'Skills',
    icon: '',
    link: ''
  },
  {
    name: 'Services',
    icon: '',
    link: ''
  },
  {
    name: 'Portfolio',
    icon: '',
    link: ''
  },
  {
    name: 'Contact Me',
    icon: '',
    link: ''
  }
])

function navToggle() {
  document.getElementById('nav-menu')
      .classList.add('show-menu')
}

function navClose() {
  document.getElementById('nav-menu')
      .classList.remove('show-menu')
}

function linkAction() {
  document.getElementById('nav-menu')
      .classList.remove('show-menu')
}

</script>

<style scoped>

</style>
