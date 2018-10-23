<template>
  <section>
    <h1 class="sr-only">Latest posts</h1>
    <a :href="link" 
      class="blog-post shaded"
      v-for="{guid, isHighlighted, pubDate, title, thumbnail, link} in posts" 
      :key="guid">
      <article :class="{'row': isHighlighted}" >
        <div v-if="isHighlighted" :class="{'col-sm-6': isHighlighted}" class="blog-post__tn-wrapper">
          <img class="blog-post__tn" :src="thumbnail" />
        </div>
        <div :class="{'col-sm-6': isHighlighted}">
          <time class="text-primary" :datetime="pubDate">{{new Intl.DateTimeFormat('en-US', {
            month: 'long', day: 'numeric', year: 'numeric'
          }).format(new Date(pubDate))}}</time>
          <h1 class="h3 my-3 text-primary">{{title}}</h1>
          <span class="font-weight-bold">&#9656; Read more</span>
        </div>
      </article>
    </a>
    <a class="inline-link ml-4" href="https://medium.com/@matyaszaborszky" target="_blank">&#9656; More posts</a>
  </section>
</template>

<script>
export default {
  name: 'BlogPosts',
  data () {
    return {
      posts: []
    }
  },
  beforeMount () {
    fetch('https://api.rss2json.com/v1/api.json?rss_url=https://medium.com/feed/@matyaszaborszky')
      .then(res => res.json())
      .then(json => {
        this.posts = json.items.slice(0, 3).map((post, index) => {
          if (index === 0) {
            post.isHighlighted = true
          }
          return post
        })
      })
  }
}
</script>

<style lang="scss">
.blog-post {
  display: block;
  margin: 0 0 3rem;
  background: white;
  padding: 1.5rem 2rem;
}
.blog-post__tn-wrapper {
  margin: -1.5rem 2rem -1.5rem -2rem;
  width: 50%;
  overflow: hidden;
  position: relative;
}
.blog-post__tn {
  position: absolute;
  max-height: 100%;
  width: auto;
}
</style>

