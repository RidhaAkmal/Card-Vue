<script setup>
import { ref } from 'vue'
import Item from './Item.vue'
  
const cards = ref([
    {
        title: "Personality Test",
        link: {
            url: "#",
            src: "https://perceptionprofiling.com/wp-content/uploads/sites/4/2019/02/pp_icons_shadow-150x150.png"
        },
        text: "Pilih satu dari pernyataan yang PALING SESUAI dengan diri Anda."
    },
    {
        title: "ENGTEST",
        link: {
            url: "#",
            src: "https://languageadvisor.net/wp-content/uploads/2021/06/Check-your-Progress1-150x150.png"
        },
        text: "Choose the correct word or phrase to fill the blank of these sentences!"
    },
    {
        title: "Mathematical Test",
        link: {
            url: "#",
            src: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT6LB48YyXpWSEfXg0-02A4CwBx1lLpD7P4yVmCMHYykA6_QRBv3reSmH0mFNb5C8morys&usqp=CAU"
        },
        text: "Solve this mathematical problem with the correct answer."
    }
])
</script>

<template>
	<Item
  	v-for="card in cards"
	:key="card.id"
  	:title="card.title"
    :text="card.text"
    :link="card.link"
	></Item>
</template>