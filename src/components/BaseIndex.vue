<template>
    <div class="container mb-4">
        <div class="row justify-content-center align-items-center g-3 mb-5">
            <div class="col-lg-4 d-grid my-2"><button class="btn btn-primary btn-lg fs-2"
                    @click="enterGame">進入遊戲</button></div>
            <div class="col-lg-4 d-grid my-2"><button class="btn btn-primary btn-lg fs-2"
                    @click="howToBuy">如何購買</button></div>
            <div class="col-lg-4 d-grid my-2"><button class="btn btn-primary btn-lg fs-2" @click="aboutUs">關於我們</button>
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        setup(props, { emit }) {
            const enterGame = () => {
                emit('enterGame');
            };
            const howToBuy = () => {
                emit('howToBuy');
            };
            const aboutUs = () => {
                emit('aboutUs');
            };

            return {
                enterGame,
                howToBuy,
                aboutUs,
            };
        }
    };
</script>
<style>
    
</style>