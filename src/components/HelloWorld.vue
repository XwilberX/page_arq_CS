<template>
  <v-container>
    <v-layout mt-5>
      <v-flex xs12>
        <v-row class="6">
          <v-carousel>
            <v-carousel-item
              v-for="(item,i) in items"
              :key="i"
              :src="item.src"
              reverse-transition="fade-transition"
              transition="fade-transition"
            ></v-carousel-item>
          </v-carousel>
        </v-row>
      </v-flex>
    </v-layout>
    
    <v-layout mt-5>
      <v-flex xs12>
        <div class="text-center">
          <v-bottom-sheet v-model="sheet" inset>
            <template v-slot:activator="{ on }">
              <v-btn color="orange" dark v-on="on">Open</v-btn>
            </template>
            <v-sheet class="text-center" height="200px">
              <v-btn class="mt-6" text color="error" @click="sheet = !sheet">close</v-btn>
              <div class="my-3">
                <p>Aqui el codigo</p>
              </div>
            </v-sheet>
          </v-bottom-sheet>
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>


<script>
export default {
  data() {
    return {
      items: [
        {
          src: "https://wallpaperbro.com/img/42696.jpg"
        },
        {
          src: "http://getwallpapers.com/wallpaper/full/b/9/2/488886.jpg"
        },
        {
          src:
            "https://www.cbtnuggets.com/blog/wp-content/uploads/2015/03/Programming-featured-image.jpg"
        },
        {
          src:
            "https://i.pinimg.com/originals/66/ad/af/66adaf7071d6c36b30a6dbe984be48dc.jpg"
        }
      ],
      sheet: false
    };
  }
};
</script>
