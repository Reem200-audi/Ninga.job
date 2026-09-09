<template>
  <div class="about">
    <h1>About</h1>
    <button
    @click="storeCount.increasecount">{{storeCount.count}}</button>
  </div>
</template>
<script setup>

import {useCounterStore} from '@/stores/counter'
const storeCount=useCounterStore()

</script>

