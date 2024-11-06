<script setup>

defineProps({
    text : {
        type : String,
        Required : true
    },
    count : {
        type : Number,
        Required: true
    }
})

</script>

<template>
  <button @click="$emit('increase')">{{ text }} {{ count }}</button>
</template>