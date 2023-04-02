<script setup>
import navbar from "../components/navbar.vue"
</script>

<template>
    <navbar title="without numbers" :links="[
      {
        id: 1,
        text: 'home',
        url: '/home'
      }
    ]"/>
    <div>
      <slot/>
    </div>
</template>