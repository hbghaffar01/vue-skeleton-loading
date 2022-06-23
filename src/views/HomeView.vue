<template>
<suspense>
  <template #default>
    <profileCard />
  </template>
  <template #fallback>
    <ProfileCardSkeleton />
  </template>
</suspense>
</template>

<script>
import profileCard from '@/components/profileCard.vue'
import ProfileCardSkeleton from '@/components/ProfileCardSkeleton.vue'

export default {
  components: {
    profileCard,
    ProfileCardSkeleton
  }
}
</script>

<style>

</style>