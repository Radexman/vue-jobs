<script setup>
import { RouterLink } from 'vue-router';
import { ArrowLeft } from '@primeicons/vue';
</script>

<template>
  <section>
    <div class="container m-auto px-6 py-6">
      <RouterLink to="/jobs" class="flex items-center text-green-500 hover:text-green-600">
        <ArrowLeft class="mr-2" />
      </RouterLink>
    </div>
  </section>
</template>
