<template>
  <q-layout>
  <div class="q-pa-md">

      <q-header elevated style="position: fixed; width: 100%; z-index: 1000;" class="header">
        <q-toolbar>
          <q-btn flat round dense icon="menu" class="q-mr-sm" />
          <q-toolbar-title> ANIME FIGURES</q-toolbar-title>
          <q-btn flat round dense icon="whatshot" />
        </q-toolbar>

      </q-header>
      
      <q-page-container>
        <q-page class="q-pa-md">
          <div class="q-pa-md">
            <div class="q-gutter-md">
            <q-carousel class="banner"
              animated
              v-model="slide"
              arrows
              navigation
              infinite
              >
              <q-carousel-slide name="style" class="column no-wrap flex-center">
                <q-img 
                  src="https://nerdarena.in/cdn/shop/files/Website-banner_anime.jpg?v=1657633543&width=1920" 
                  class="banner"
                />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
              <q-carousel-slide name="tv" class="column no-wrap flex-center">
                <q-img class="banner"
                  src="https://animefigure.co.uk/wp-content/uploads/2023/07/bANNER-1.jpg" 
                />
                <div class="q-mt-md text-center">
                  {{ lorem }}
                </div>
              </q-carousel-slide>
            </q-carousel>

          </div>

          <div class="q-pa-md row items-start q-gutter-md">

            <q-card class="my-card">
              <q-img src="https://animefigure.co.uk/wp-content/uploads/2023/06/Naruto-Itachi-Anime-Figur-30CM-Uchiha-Sasuke-Uzumaki-Naruto-PVC-Action-Shippuden-Vibration-Sterne-Figurine-Modell-1-441x441.jpg">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Uzumaki Naruto
                </div>
              </q-img>
            </q-card>

            <q-card class="my-card">
              <q-img src="https://animefigure.co.uk/wp-content/uploads/2023/05/anime-figure-demon-slayer-figures-battle-nezuko-kamado-blood-demon-441x441.jpg">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Nezuko Kamado
                </div>
              </q-img>
            </q-card>

            <q-card class="my-card">
              <q-img src="https://animefigure.co.uk/wp-content/uploads/2023/07/Anime-Nika-Ruffy-Gear-5-Action-figur-Spielzeug-ein-St-ck-Figuren-20cm-gk-Statue-Manga-1-441x441.jpg">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Nika Luffy Gear 5
                </div>
              </q-img>
            </q-card>

                        <q-card class="my-card">
              <q-img src="https://animefigure.co.uk/wp-content/uploads/2023/06/48cm-One-Piece-Abbildung-Lorenor-Zorro-Neun-Messer-Fluss-Pop-Max-Asura-Zoro-Action-figuren-PVC-1-441x441.jpg">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Rononoa Zoro
                </div>
              </q-img>
            </q-card>
            <q-card class="my-card">
              <q-img src="https://animefigure.co.uk/wp-content/uploads/2023/06/32cm-Anime-Einem-St-ck-Tiere-Piraten-K-nig-Vier-Kaiser-Kaido-King-Figur-YAN-ZAI-1-441x441.jpg">
                <div class="absolute-bottom text-subtitle2 text-center">
                  King Four Emperor Kaido 
                </div>
              </q-img>
            </q-card>
            <q-card class="my-card">
              <q-img src="https://cdn.kyou.id/thumbnail/items/43225-pvc-figure-17-megumi-kato-first-meeting-outfit-ver.jpg.webp">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Megumi Kato - First Meeting Outfit
                </div>
              </q-img>
            </q-card>
            <q-card class="my-card">
              <q-img src="https://cdn.kyou.id/items/147061-pvc-figure-14-suguru-geto-jujutsu-kaisen-0.jpg.webp">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Suguru Geto
                </div>
              </q-img>
            </q-card>
            <q-card class="my-card">
              <q-img src="https://cdn.kyou.id/items/195328-pvc-figure-17-makima-chainsaw-man.jpg.webp">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Makima
                </div>
              </q-img>
            </q-card>
            <q-card class="my-card">
              <q-img src="https://cdn.kyou.id/items/136224-s-fire-figure-18-bakugo-katsuki-boku-no-hero-academia.jpg.webp">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Bakugo Katsuki
                </div>
              </q-img>
            </q-card>

            <q-card class="my-card">
              <q-img src="https://cdn.kyou.id/items/114793-exclusive-sale-pvc-figure-the-ghost-bride-illustration-by-fuzichoco.jpg.webp">
                <div class="absolute-bottom text-subtitle2 text-center">
                  Figure The Ghost Bride Illustration by fuzichoco
                </div>
              </q-img>
            </q-card>

          </div>
          </div>
        </q-page>
      </q-page-container>
 
  </div>
  <q-footer reveal elevated>
        <q-toolbar class="footer">
          <q-toolbar-title>Thyo aji Dinata -- 223510553</q-toolbar-title>
        </q-toolbar>
      </q-footer>

</q-layout>
  <q-footer elevated>
    <q-toolbar class="glossy">
      <q-toolbar-title>Footer</q-toolbar-title>
    </q-toolbar>
  </q-footer>
</template>

<script>
import { ref } from "vue";

export default {
  setup() {
    return {
      tab: ref("images"),
      time: ref("10:56"),
      timeWithSeconds: ref("09:24:10"),
      slide: ref("style"),
      lorem: "",
    };
  },
};
</script>

<style>
.header {
  background-image: linear-gradient(120deg, #3b3131 0%, #db1d17 100%);
}

.my-card {
  width: 100%;
  max-width: 250px;
}


.banner {
  border-radius: 16px;
  content: center;
  align-self: center;
}

.footer {
  background-image: linear-gradient(120deg, #3b3131 0%, #db1d17 100%);
  text-align: center;
}
</style>
