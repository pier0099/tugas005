  <template>

    <h3 class="text-center">Featured Products</h3>
     <div class="carousel">
            <div class="carousel-inner" :style="{ transform: 'translateX(-' + currentIndex * 100 + '%)' }">
                <div class="carousel-item" v-for="(slide, index) in slides" :key="index">
                    <img :src="slide.image" alt="carousel image">
                    <div class="carousel-caption">
                      <div class="title-carousel">
                        <b>{{ slide.text }}</b>
                        <hr>
                        <p>${{ slide.price }},-</p>
                      </div>
                    </div>
                </div>
            </div>
            <button class="carousel-control prev" @click="prev">&lt;</button>
            <button class="carousel-control next" @click="next">&gt;</button>
        </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
            currentIndex: 0,
            slides: [
                { image: 'src/assets/no1.jpg', text: 'BACARDI', price: 145 },
                { image: 'src/assets/no2.jpg', text: 'KRAKEN', price:  256},
                { image: 'src/assets/no03.jpg', text: 'RAYNAL VSOR', price: 476 }
            ]
      };
    },
    methods: {
        next() {
            this.currentIndex = (this.currentIndex + 1) % this.slides.length;
        },
        prev() {
            this.currentIndex = (this.currentIndex - 1 + this.slides.length) % this.slides.length;
        }
    }
  }
  </script>
  