
<style>
  :root {
    --primaryColor: rgb(227, 6, 19);
    --primaryFont: sans-serif
  }
  :focus:not(:focus-visible) {
    outline: none
  }
  .maxWidth {
    padding: 2rem;
    max-width: min(1376px, calc(100vw - 4rem));
    margin: auto
  }
  :any-link {
    color: var(--primaryColor);
    font-weight: bold;
    text-decoration: none
  }

  /* Nav */
  nav.nav {
    display: grid;
    grid-auto-flow: column
  }
  .logo--container {
    display: grid;
    align-content: center;
    justify-content: left
  }
  .logo img {
    max-width: 100px
  }
  .nav--container {
    justify-self: end;
    display: grid;
    grid-gap: 1rem;
    grid-auto-flow: column;
    align-content: center
  }
  .nav--link {
    font-size: 1.25rem;
    padding: .5rem;
    transition: color .5s, border .5s;
    border-bottom: .15rem solid transparent;
    font-family: var(--primaryFont);
    letter-spacing: .05rem
  }
  .nav--link:hover {
    color: var(--primaryColor)
  }
  .nav--link:hover, .nav--link.nuxt-link-exact-active {
    border-bottom: .15rem solid var(--primaryColor)
  }
  .nav--icon {
    display: none
  }
  main {
    min-height: 70vh
  }

  @media (max-width: 768px) {
    .maxWidth {
      padding: 1rem
    }
    .nav--icon {
      display: block;
      height: 40px;
      width: 40px;
      justify-self: end;
      align-self: center
    }
    .nav--container {
      height: 100vh;
      min-height: -webkit-fill-available;
      position: absolute;
      grid-auto-flow: row;
      left: 100vw;
      top: 0;
      bottom: 0;
      width: 200px;
      background: var(--primaryColor);
      padding: 2.5rem;
      transition: left 1s
    }
    .nav_open .nav--container {
      left: calc(100vw - 200px)
    }
    .nav_close .nav--container {
      display: none
    }
    html {
      transition: margin 1s
    }
    html.nav_open {
      margin-left: -400px;
      overflow: hidden
    }
  }
  .button {
    background-color: var(--primaryColor);
    padding: .75rem 1rem;
    border-radius: .25rem;
    color: white;
    border: 2px solid
  }
  .button:hover {
    background-color: transparent
  }
</style>

<template>
  <div :style="'--motion: ' + motion">
    <header>
      <nav class="nav maxWidth">
        <div class="logo--container">
          <nuxt-link class="logo" to="/">
            <img src="icon.png">
          </nuxt-link>
        </div>
        <div class="nav--icon">
          <div @click="nav" v-html="require('../assets/svg/menu.svg?include')" />
        </div>
        <div class="nav--container">
          <a href="#" class="nav--link">
            Home
          </a>
          <a href="#how-we-can-help" class="nav--link">
            How We Can Help
          </a>
          <a href="#give-back" class="nav--link">
            Give Back
          </a>
          <a href="#events" class="nav--link">
            Events
          </a>
          <a href="#news" class="nav--link">
            News
          </a>
          <a href="https://eshop.solent.ac.uk/product-catalogue/public-and-alumni-services/donations/donate-online-now" class="nav--link button primary">
            Donate
          </a>
        </div>
      </nav>
    </header>
    <main>
      <nuxt keep-alive />
    </main>
  </div>
</template>

<script>
export default {
  data () {
    return {
      motion: 'auto'
    }
  },
  watch: {
    $route () {
      document.documentElement.classList.remove('nav_open')
      setTimeout(function () {
        document.documentElement.classList.add('nav_close')
      }, 1000)
    }
  },
  async beforeMount () {
    if (await this.WebpIsSupported()) {} else {
      document.querySelector('body').classList.add('no-webp')
    }
  },
  async mounted () {
    document.documentElement.classList.add('nav_close')
    this.motion = await window.matchMedia('(prefers-reduced-motion: reduce)').matches ? 'auto' : 'smooth'
  },
  methods: {
    async WebpIsSupported () {
      // If the browser doesn't have the method createImageBitmap, you can't display webp format
      if (!self.createImageBitmap) {
        return false
      }

      // Base64 representation of a white point image
      const webpData = 'data:image/webp;base64,UklGRiQAAABXRUJQVlA4IBgAAAAwAQCdASoCAAEAAQAcJaQAA3AA/v3AgAA='

      // Retrieve the Image in Blob Format
      const blob = await fetch(webpData).then(r => r.blob())

      // If the createImageBitmap method succeeds, return true, otherwise false
      return createImageBitmap(blob).then(() => true, () => false)
    },
    nav () {
      if (document.documentElement.classList.contains('nav_open')) {
        document.documentElement.classList.remove('nav_open')
        setTimeout(function () {
          document.documentElement.classList.add('nav_close')
        }, 1000)
      } else {
        document.documentElement.classList.remove('nav_close')
        setTimeout(function () {
          document.documentElement.classList.add('nav_open')
        }, 1)
      }
    }
  }
}
</script>
