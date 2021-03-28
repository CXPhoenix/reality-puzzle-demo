<template>
  <BaseAboutPage @backToIndex="backToIndex"></BaseAboutPage>
</template>

<script>
  import BaseAboutPage from '@/components/BaseAboutPage.vue'
  import { useRouter } from 'vue-router'

  export default {
    components: {
      BaseAboutPage,
    },
    setup() {
      const router = useRouter()
      
      const backToIndex = () => {
        router.push({ path: '/' })
      }
      return {
        backToIndex,
      }
    }
  }
</script>
