<template>
  <div class="q-pa-md q-gutter-sm flex-between aa">
    <div class="left">
      <q-avatar class="profile">
        <q-icon name="account_circle" size="45px" />
      </q-avatar>
    </div>
    <div class="right">
      <q-btn flat style="color: #001499cc" label="Keranjang" />
      <q-btn flat style="color: #001499cc" label="Pengaturan" />
      <q-btn flat style="color: #001499cc" label="CS" />
      <q-btn style="background: #001499cc; color: white" label="Akun" />
    </div>
  </div>

  <div class="q-pa-md">
    <q-carousel
      v-model="slide"
      swipeable
      animated
      navigation-position="bottom"
      navigation
      padding
      height="200px"
      class="bg-indigo-9 text-white rounded-borders"
    >
      <q-carousel-slide name="style" class="column no-wrap flex-center">
        <q-icon name="shopping_cart" size="56px" />
        <div class="q-mt-md text-center">
          {{ satu }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="tv" class="column no-wrap flex-center">
        <q-icon name="checkroom" size="56px" />
        <div class="q-mt-md text-center">
          {{ dua }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="layers" class="column no-wrap flex-center">
        <q-icon name="local_mall" size="56px" />
        <div class="q-mt-md text-center">
          {{ tiga }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="map" class="column no-wrap flex-center">
        <q-icon name="redeem" size="56px" />
        <div class="q-mt-md text-center">
          {{ empat }}
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>

  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card" flat bordered>
      <q-img
        src="https://i0.wp.com/zilbest.com/wp-content/uploads/2022/11/Angled-top-down-view-of-the-ROG-Strix-GeForce-RTX-4090-graphics-card-highlighting-the-fans-ARGB-element.jpg?w=1469&ssl=1"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 30.000.000</div>
        <div class="text-h5 q-mt-sm q-mb-xs">RTX 4090</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://pcgamebali.com/wp-content/uploads/2023/12/PC-Gamer-Bali-Motherboard-Asrock-Z790-Pro-RS-DDR5.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 6.000.00</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Motherboard Asrock</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQH1cbO00bPx_gm5EJge2rYEX_YyVeW6FREEA&usqp=CAU"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 1.200.00</div>
        <div class="text-h5 q-mt-sm q-mb-xs">RAM 64GB Samsung</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://images.tokopedia.net/img/cache/700/VqbcmM/2023/8/1/b27e6dfb-d595-4d00-a71e-cadf25d2becc.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 1.050.000</div>
        <div class="text-h5 q-mt-sm q-mb-xs">SSD Transcend 1TB</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://images.tokopedia.net/img/cache/700/VqbcmM/2023/10/3/462250bc-a59b-4753-92f1-26b2897a1bd2.jpg"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 25.000.000</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Monitor ASUS ROG 540hz</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://img.ws.mms.shopee.co.id/id-11134207-7r98q-lp55pz0nxuoe71"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 899.999</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Keyboard AJAZZ ak820 pro </div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="https://images.tokopedia.net/img/cache/700/VqbcmM/2023/11/10/7c4ba7ef-b707-45e4-b983-cc442d7b24ed.png"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 650.000</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Mouse GOZO</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    <q-card class="my-card" flat bordered>
      <q-img
        src="data:image/jpeg;base64,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"
        class="same-size-image"
      />
      <q-card-section>
        <div class="text-overline text-orange-9">Rp 699.999</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Gamepad 8bitdo ultimate</div>
        <div class="text-caption text-grey">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
      </q-card-section>
      <q-card-actions>
        <q-btn flat color="indigo-10" label="Share" style="font-weight: 550;" />
        <q-btn flat color="orange-8" label="Keranjang" style="font-weight: 550;" />
        <q-space />
        <q-btn
          color="grey"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>
      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subtitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>

    
  </div>
    <footer class="q-pa-md text-center bg-indigo-10 text-white">
      <div class="q-mb-md">© 2024 RandyIvando.com All Rights Reserved.</div>
      <div class="text-caption">JL. Kubang Raya | email@gmail.com | telpon 08********</div>
    </footer>


</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('style'),
      satu: 'Nikmati hingga discount 100%, hanya disini dan pastikan lu ga kelewatan ya hidupin loncengnya anjay',
      dua: 'Kapan lagi kan discount besar besaran anjay, anda bisa mendapatkan barang apapun yang anda inginkan xixixi',
      tiga: 'saya udah bingung mau nulis gimik apalagi jadi yaudah deh ini aja ehe',
      empat: 'bang tolong kasihani kami bang banyak kali tugas didunia ini',
      expanded: ref(false),
      lorem: 'pokoknya ini detailnya capek ngetiknya satu satu hehe'
    }
  }
}
</script>

<style scoped>
.flex-between {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #e3e3e3;
  padding: 1rem 3rem;
}

.left {
  display: flex;
  align-items: center;
}

.right {
  display: flex;
  align-items: center;
}

.my-card {
  width: 100%;
  max-width: 350px;
}

.same-size-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.aa{
  max-width: 100%;
}
</style>
