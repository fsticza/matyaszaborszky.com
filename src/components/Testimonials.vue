<template>
  <div class="row align-items-center">
    <div class="col-sm-5">
      <h1 class="section__title">Testimonials</h1>
      <transition tag="div" name="carousel-text-fade" mode="out-in">
        <blockquote v-for="(item, index) in items"
          v-if="activeIndex === index"
          class="blockquote"
          :key="index">
          <p class="h2">
            &ldquo;{{item.text}}&rdquo;
          </p>
          <footer class="blockquote-footer my-3">
            <span class="">{{item.name}}</span>
            <a class="float-right inline-link" :href="item.link">&#9656; Visit his/her LinkedIn</a>
          </footer>
        </blockquote>
      </transition>
      <ol class="carousel-indicators">
        <li v-for="(item, index) in items" 
          class="carousel-indicator"
          :class="{'carousel-indcator--active': index === activeIndex}" 
          :key="index">
        </li>
      </ol>
    </div>
    <div class="col-sm-5 offset-sm-2">
      <transition tag="div" name="carousel-image-fade" mode="out-in">
        <img width="480" v-for="(item, index) in items"
          v-if="activeIndex === index" 
          class="img-fluid shaded"
          src="../assets/img/rawpixel-648567-unsplash.jpg"
          :key="index" />
      </transition>    
    </div>
  </div>
</template>

<script>

const requestInterval = function (fn, delay) {
  var requestAnimFrame = (function () {
    return window.requestAnimationFrame || function (callback) {
      window.setTimeout(callback, 1000 / 60);
    }
  })(),
  start = Date.now(),
  handle = {}
  function loop() {
    handle.value = requestAnimFrame(loop)
    var current = new Date().getTime(),
    delta = current - start
    if (delta >= delay) {
      fn.call()
      start = Date.now()
    }
  }
  handle.value = requestAnimFrame(loop)
  return handle
}

export default {
  name: 'Testimonials',
  data () {
    return {
      activeIndex: 0,
      items: [{
        text: `If you want real marketing that works and effective implementation - Ikkk's got you covered. 
          If you aren't sure, always go for Ikkk.`,
        name: 'Dyanna Y.',
        link: '',
      }, {
        text: `Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...`,
        name: 'Name #2',
        link: '',
      }]
    }
  },
  mounted () {
    requestInterval(() => {
      this.activeIndex = this.activeIndex < this.items.length - 1 
        ? this.activeIndex + 1
        : 0
    }, 5000)
  }
}
</script>

<style lang="scss">
@import "../assets/scss/abstracts/variables";

.carousel-text-fade-enter-active {
  transition: all .6s ease-in;
}
.carousel-text-fade-leave-active {
  transition: all .3s ease-in;
}
.carousel-text-fade-enter, .carousel-text-fade-leave-to {
  opacity: 0;
  transform: translateX(-20px);
}
.carousel-image-fade-enter-active {
  transition: all .6s ease-out;
}
.carousel-image-fade-leave-active {
  transition: all .3s ease-out;
}
.carousel-image-fade-enter, .carousel-image-fade-leave-to {
  opacity: 0;
  transform: translatey(20px);
}

.carousel-indicators {
  list-style-type: none;
  margin: 2rem 0;
  padding: 0;
}
.carousel-indicator {
  display: inline-block;
  margin-right: 10px;
  height: 8px;
  width: 48px;
  border-bottom: 2px solid $semi-light-gray;
  position: relative;
}
.carousel-indcator--active {
  &:before {
    content: ' ';
    position: absolute;
    display: inline-block;
    height: 8px;
    width: 50%;
    background: $pink;
  }
}
</style>

