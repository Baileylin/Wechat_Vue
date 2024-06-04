<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'

function make() {
  fetch('https://api.coindesk.com/v1/bpi/currentprice.json').then(response => {
    return response.json()
  }).then(data => {
    console.log(data)
  })
  }
</script>

<template>
  <a href='https://api.coindesk.com/v1/bpi/currentprice.json' @click='make'>Hello World!</a> 
  
</template>