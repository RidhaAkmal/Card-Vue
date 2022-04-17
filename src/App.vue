<script setup>
import Atas from './components/course/CourseHeader.vue'
import Tengah from './components/course/CourseMain.vue'
import Bawah from './components/course/CourseFooter.vue'
</script>

<template>
  <header>
    <Atas/>
  </header>
    
  <main>
    <Tengah/>
  </main>

  <footer>
    <Bawah/>
  </footer>
</template>

<style>
@import './assets/base.css';

main{
  text-align: center;
}

</style>