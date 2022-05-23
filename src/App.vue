<script setup lang="ts">
import {toRefs} from "vue";

let obj = $ref({
  count: 0
})

function increment() {
  obj.count++
}

let {count} =  toRefs(obj)

</script>

<template>
  <div>
    Count: {{ count }}
    <button @click="increment">Add</button>
  </div>
</template>
