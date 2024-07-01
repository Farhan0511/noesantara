<template>
    <div class="hero">
        <!-- Desktop -->
        <div class="d-none d-md-block">
            <div class="container">
                <div class="row align-items-center justify-content-around">
                    <div class="col mt-3">
                        <h2 class="mb-3">"Menikmati Rasa Nusantara: Tempat yang Menghidangkan Kelezatan Lokal"</h2>
                        <p>Ayo pilih makanan kesukaanmu!</p>
                        <button class="btn btn-lg btn-success">Pesan Sekarang <b-icon-arrow-right></b-icon-arrow-right></button>
                    </div>
                    <div class="col-md-5 text-center">
                        <img src="../assets/image/hero2.png" alt="Hero Image" class="img-fluid" width="100%">
                    </div>
                </div>
            </div>

        </div>

        <!-- Mobile -->
        <div class="d-sm-block d-md-none">
            <div class="container">
                <div class="row align-items-center justify-content-around">
                    <div class="col-md-5 text-center mb-4">
                        <img src="../assets/image/hero.png" alt="Hero Image" class="img-fluid" width="400px">
                    </div>
                    <div class="col">
                        <h2>"Menikmati Rasa Nusantara: Tempat yang Menghidangkan Kelezatan Lokal"</h2>
                        <p>Ayo pilih makanan kesukaanmu!</p>
                        <button class="btn btn-lg btn-success">Pesan Sekarang<b-icon-arrow-right></b-icon-arrow-right></button>
                    </div>
                </div>
            </div>

        </div>
    </div>
    
</template>

<script>
// @ is an alias to /src

export default {
  name: 'HeroApp',
}
</script>