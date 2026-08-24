<script setup>
import { ref } from 'vue'

import jobData from '@/jobs.json'
import JobListing from './JobListing.vue'

const jobs = ref(jobData.jobs)
</script>

<template>
  <section class="bg-blue-50 px-4 py-10">
    <div class="container-xl m-auto lg:container">
      <h2 class="mb-6 text-center text-3xl font-bold text-green-500">Browse Jobs</h2>
      <div class="grid grid-cols-1 gap-6 md:grid-cols-3">
        <JobListing v-for="job in jobs" :key="job.id" :job="job" />
      </div>
    </div>
  </section>
</template>
