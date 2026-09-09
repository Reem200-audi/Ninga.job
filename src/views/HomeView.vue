
<template>
  <div class="home">
<counter/>
<div class="buttons">
  <button @click="storeCount.decreasecount">-</button>
  <button @click="storeCount.increasecount">+</button>
</div>
<hr>
<div>
  the counter is: {{storeCount.oddOrEven}}
</div>
<hr>
<h3>Edit Counter:</h3>
<input type=" number" v-model="storeCount.count"/>

  </div>
</template>
<script setup>

import {useCounterStore} from '@/stores/counter'
import Counter from '@/components/Counter.vue'
const storeCount=useCounterStore()

</script>

<style>
.counts{
  font-size: 60px;
  margin: 20px;
}
.buttons button{
  font-size: 40px;
  margin: 10px;
}

  </style>
