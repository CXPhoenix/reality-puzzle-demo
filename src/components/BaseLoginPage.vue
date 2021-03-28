<template>
    <div class="container mb-4">
        <header>
            <span class="p-1 display-3 mx-auto my-3 fw-bold">使用者登入</span>
        </header>

        <section>
            <div class="form-floating mt-3 mb-2">
                <input type="email" class="form-control form-control-lg" id="floatingInput" placeholder="Email">
                <label for="floatingInput">輸入帳號</label>
            </div>
            <div class="form-floating mb-3">
                <input type="password" class="form-control form-control-lg" id="floatingPassword" placeholder="Password">
                <label for="floatingPassword">輸入密碼</label>
            </div>
            <div class="row justify-content-center g-1">
                <div class="col-lg-4 d-grid">
                    <button class="btn btn-success btn-lg" @click="signIn">登入</button>
                </div>
                <div class="col-lg-4 d-grid">
                    <button class="btn btn-secondary btn-lg" @click="forgetPW">忘記密碼</button>
                </div>
                <div class="col-lg-4 d-grid">
                    <button class="btn btn-warning btn-lg" @click="signUp">前往註冊</button>
                </div>
            </div>

            <div class="row justify-content-start mt-3 mb-5">
                <div class="col-lg-6 d-grid">
                    <button class="border-top-0 btn btn-light btn-lg p-2 fs-2 shadow d-flex align-items-center justify-content-center" @click="googleSignIn"><img class="img-fluid" src="../assets/googleIcon.svg" alt="" style="width: 2.5rem; height: 2.5rem;">&nbsp;&nbsp;Google 登入</button>
                </div>
            </div>
        </section>
        
    </div>
</template>
<script>
export default {
    setup(props, { emit }) {
        const signIn = () => {
            emit('signIn')
        }
        const forgetPW = () => {
            emit('forgetPW')
        }
        const signUp = () => {
            emit('signUp')
        }
        const googleSignIn = () => {
            emit('googleSignIn')
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