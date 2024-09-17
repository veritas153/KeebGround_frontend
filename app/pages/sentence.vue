<script setup lang="ts">
import { sub } from 'date-fns'
import type { Period, Range } from '~/types'

const { isNotificationsSlideoverOpen } = useDashboard()

const range = ref<Range>({ start: sub(new Date(), { days: 14 }), end: new Date() })
const period = ref<Period>('daily')
</script>

<template>
  <UDashboardPage>
    <UDashboardPanel grow>
      <UDashboardNavbar title="Sentence Practice">
        
      </UDashboardNavbar>

    </UDashboardPanel>
  </UDashboardPage>
</template>
