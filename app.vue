<template>
  <div>
    {{ timezone }}<br/>
    {{ dayjs().format() }}
  </div>
</template>

<script setup>
import dayjs from 'dayjs'
const timezone = Intl.DateTimeFormat().resolvedOptions().timeZone
</script>