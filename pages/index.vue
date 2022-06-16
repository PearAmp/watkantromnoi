<template>
  <div>
    <ImageHeader />
    <RecommendPage />
    <Community />
    <Morale />
    <Personal />
  </div>
</template>

<script>
import Personal from '~/components/Personal/Personal.vue'
export default {
  components: { Personal },
  name: 'IndexPage',
}
</script>

<style lang="scss" scoped>
</style>
