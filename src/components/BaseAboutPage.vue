<template>
    <div class="container mb-4 p-2">
        <h1 class="fs-1 mx-auto my-1">關於我們</h1>
        
        <section>
            <div class="row mt-2 mt-lg-4">
                <div class="col">
                    <img class="mx-auto img-fluid img-thumbnail d-none d-lg-block" src="http://fakeimg.pl/400x400"
                        alt="社團LOGO" />
                    <img class="mx-auto img-fluid img-thumbnail d-block d-lg-none" src="http://fakeimg.pl/200x200"
                        alt="社團LOGO" />
                    <h2 class="fs-2 mt-1">復興高中 資訊傳播社</h2>
                </div>
            </div>
            <div class="row justify-content-center mt-1">
                <div class="col">
                    <p class="fs-3">[intro] Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat,
                        laudantium quas corporis qui deleniti animi recusandae maiores quia commodi tempore dignissimos
                        nemo vitae at, ea, nostrum nulla maxime dolorem accusantium in veritatis quam corrupti fugit
                        neque rerum. Omnis incidunt architecto aperiam fuga, consequuntur beatae eum ratione et odit?
                        Deleniti, nobis.</p>
                </div>
            </div>
        </section>

        <section>
            <div class="row mt-3 mt-lg-4">
                <div class="col">
                    <h3 class="fs-3">專案成員</h3>
                </div>
            </div>
            <div class="row mt-1 mt-lg-3">
                <div class="col">
                    <img src="http://fakeimg.pl/200x200" alt="PM照片" class="mx-auto img-fluid rounded-circle" />
                    <span class="d-block fs-5 mb-0">ＯＯＯ</span>
                    <span class="d-block fs-6 text-muted mt-0">專案管理人</span>
                </div>
            </div>
            <div class="row row-cols-1 row-cols-md-2 row-cols-lg-4 mt-1 mt-lg-2 g-4">
                <div class="col"><img src="http://fakeimg.pl/200x200" alt="組員#1"
                        class="mx-auto img-fluid rounded-circle"><span class="d-block fs-5 mb-0">ＯＯＯ</span><span
                        class="d-block fs-6 text-muted mt-0">組員#1</span></div>
                <div class="col"><img src="http://fakeimg.pl/200x200" alt="組員#2"
                        class="mx-auto img-fluid rounded-circle"><span class="d-block fs-5 mb-0">ＯＯＯ</span><span
                        class="d-block fs-6 text-muted mt-0">組員#2</span></div>
                <div class="col"><img src="http://fakeimg.pl/200x200" alt="組員#3"
                        class="mx-auto img-fluid rounded-circle"><span class="d-block fs-5 mb-0">ＯＯＯ</span><span
                        class="d-block fs-6 text-muted mt-0">組員#3</span></div>
                <div class="col"><img src="http://fakeimg.pl/200x200" alt="組員#4"
                        class="mx-auto img-fluid rounded-circle"><span class="d-block fs-5 mb-0">ＯＯＯ</span><span
                        class="d-block fs-6 text-muted mt-0">組員#4</span></div>
            </div>
        </section>

        <section>
            <div class="row mt-3 mb-2 mt-lg-5">
                <div class="col">
                    <span class="d-block d-md-none fs-5"><b>通訊地址</b><br />台北市北投區復興四路70號 資訊傳播社</span>
                    <span class="d-none d-md-block fs-3"><b>通訊地址: </b>台北市北投區復興四路70號 資訊傳播社</span>
                </div>
            </div>
            <a href="https://goo.gl/maps/XGYJAqqUxHs2rD2Q9" class="btn btn-light btn-lg d-block d-md-none mx-auto mb-4"><i class="fas fa-map-marker-alt"></i>&nbsp;&nbsp;Google Map</a>
            <div class="ratio ratio-16x9 d-none d-md-block mt-3 mb-4">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3611.7831626545426!2d121.4998564146744!3d25.14302074006711!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3442ae489abd4d87%3A0x4c654f929ad67cd3!2z6Ie65YyX5biC56uL5b6p6IiI6auY57Sa5Lit5a24!5e0!3m2!1szh-TW!2stw!4v1616874319470!5m2!1szh-TW!2stw" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
            </div>
            <div class="row mt-4 mb-4 mt-lg-5 justify-content-center">
                <div class="col-lg-4">
                    <a class="btn btn-primary btn-lg" @click="backToIndex"><i class="fas fa-undo-alt"></i>&nbsp;&nbsp;回首頁</a>
                </div>
            </div>
        </section>
    </div>
</template>
<script>

export default {
    setup(props, { emit }) {
        const backToIndex = () => {
            emit('backToIndex')
        }
        return {
            backToIndex,
        }
    }
}
</script>
<style>
    
</style>