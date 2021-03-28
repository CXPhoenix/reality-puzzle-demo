<template>
    <BaseLoginPage @signIn="signIn" @forgetPW="forgetPW" @signUp="signUp" @googleSignIn="googleSignIn"></BaseLoginPage>
</template>
<script>
import BaseLoginPage from '@/components/BaseLoginPage.vue'

export default {
    components: {
        BaseLoginPage,
    },
    setup() {
        const signIn = () => {
            console.log('sign in')
        }
        const forgetPW = () => {
            console.log('reply password')
        }
        const signUp = () => {
            console.log('sign up')
        }
        const googleSignIn = () => {
            console.log('google sign in')
        }

        return {
            signIn,
            forgetPW,
            signUp,
            googleSignIn,
        }
    }
}
</script>
