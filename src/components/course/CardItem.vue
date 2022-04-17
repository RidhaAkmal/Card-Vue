<script setup>
defineProps(["title", "link", "text"])
</script>

<template>
    <div class="card">

      <h2>{{ title }}</h2>

      <img v-bind:src="link.src"/>

      <p>{{ text }}</p>

      <a :href="link.url">
        <button>
          Mulai {{ title }}
        </button>
      </a>
    </div>
</template>

<style>
p{
    text-align: justify;
}
</style>