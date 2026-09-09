<template>
    <div class="counts">
{{storeCount.count}}
</div>
</template>
<script setup>

import {useCounterStore} from '@/stores/counter'
const storeCount=useCounterStore()

</script>
