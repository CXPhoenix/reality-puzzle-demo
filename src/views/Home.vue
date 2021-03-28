<template>
  <BaseIndex @enterGame="enterTheGame" @howToBuy="buyGame" @aboutUs="aboutTeam"></BaseIndex>
</template>

<script>
import BaseIndex from '@/components/BaseIndex.vue'
import { useRouter } from 'vue-router'





export default {
  components: {
    BaseIndex,
  },

  setup() {
    const router = useRouter()

    const enterTheGame = () => {
      console.log('enter the game')
      router.push({ path: '/login'})
    }

    const buyGame = () => {
      console.log('Buying info')
    }

    const aboutTeam = () => {
      console.log('Team information')
      router.push({
        path: '/about'
      })
    }

    return {
      enterTheGame,
      buyGame,
      aboutTeam,
    }
  }
}
</script>
