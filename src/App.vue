<template>
  <div id="app">
    <header>
      <nav :class="[navbarClass]" class="navbar fixed-top navbar-expand-lg navbar-dark bg-primary fade">
        <div class="container">
          <a class="navbar-brand" href="/">
            <img src="./assets/img/logo.svg" alt="Matyas Zaborszky" height="16">
          </a>
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>

          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ml-auto">
              <li class="nav-item active">
                <a class="nav-link" href="#services">Services</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#testimonials">Testimonials</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#blog">Blog</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#about">About</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#contact">Contact</a>
              </li>
            </ul>
          </div>
          <span>
            <a href="">f</a>
            <a href="">t</a>
            <a href="">y</a>
          </span>
        </div>
      </nav>
    </header>

    <main class="main-content">
      <div class="section section--head">
        <div ref="first-content" class="container text-white">
          <h1>
            <img class="text-white" src="./assets/img/logo.svg" alt="Matyas Zaborszky" height="32">
          </h1>
          <div class="row">
            <div class="col-sm-6">
              <h2 class="section__lead">The killer ingredient on your road to success</h2>
              <p class="section__sub-lead">
                Winning marketing and PR strategies for a knockout token sale!
              </p>
              <a href="#contact" class="btn btn-light">Contact me now</a>
            </div>
          </div>
        </div>
      </div>

      <section id="services">
        <div class="section">
          <div class="container">
            <div class="row">
              <div class="col-sm-6 order-6">
                <h1 class="section__title">Services</h1>
                <h2 class="section__lead">Guaranteed to WIN with your token offering</h2>
                <p>
                  With the number of crypto products skyrocketing, having a great product just isn’t
        enough anymore without best in class marketing skills to command the audience’s attention. I
        have guided great crypto brands to success and I can help you too make the leap from your Big
        Idea to a Blowout Token Sale!
                </p>
                <a href="#contact" class="btn btn-primary"
                  style="position:relative;top:8.675rem;">Contact me now</a>
              </div>
              <div class="col-sm-6 order-1">

              </div>

            </div>
          </div>
        </div>

        <div class="section section--gray">
          <div class="container">
            <div class="row">
              <article class="col-lg-3 offset-lg-2 col-md-4 offset-md-1">
                <svg width="64" height="64" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                  <rect width="64" height="64" fill="url(#pattern0)"/>
                  <defs>
                  <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                  <use xlink:href="#image0" transform="scale(0.01)"/>
                  </pattern>
                  <image id="image0" width="100" height="100" xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAGQAAABkCAYAAABw4pVUAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAAApQSURBVHhe7V15jB11Hd+l3vcRRbDsO3YjupG2b+bt7vzmvboa5Yii0ehqxD88YjE2aq1aMa3UoBCptgoaGjAQKo3lMqiRarSRxgAasYBKWMV6cghGytV6ll39fH7zfe/NzJv3Zt61uy7fT/LNvDe/6zvfz/zuY4YUCoVCoVAoFAqFQqFYUIyPjz9l5KTq8ylDMzMr5PaSQW719POo23Gu+wy59f+LsTXVFxXcyskF1/9YwfEvhHwLcmve9f9acM3DuP/fJMk75jH4OYjrjfB3FcKcn3cq7y643uSxq05+pkTfE1zXfXJ+TWV1vuS/A2mck3fN7oJjbkD6s/j/UFynmlA36PNg3vHvgFyP/zuLrvlUvuy/qehWRiT6JYHhguOdBAU/ggf7NpS/N/4w/RDEfxQG+wUNUSj7bz3R958t6bcFc2KxZF6LOL4IQ94Mo/4jHndfxPEP4fl/gN9biq5XmZ6efpKosCAYzpV8g8S/jIe8J6LYAgly0r+R9r6c4300/oYWXfe5IOG9IO+bkMeSwg9eWBKYXUXXfz1fClGtv8itnsrjLdiGh7w7WYlsgmLicFA8mPvsm8Xfjnk8yW8mQVjotLdQNu9DfFf0ngusbg8FLxuurv9Isr+swrjMpaNO1RVT9g5E+IkOjHYvy1ko8gUaiUXGyJrquK3A24Dl+9jk5Mq8U53KuebNiGMT5DLIz0DivxLS6UbmEB/rgT2QraxLWMSMlKvFlZ73dFElEazHChPVl4HwtZB3wSbnIo5rcb0rIZ1Egf9vIKrhIMYuwSzHIiIpgUDs27QHdckZg6rgxsZOe+po2fh4+LNBzs+R7nyzHskC3X8L/bazoZG17ukUx09MvBAv7OnQbyekbQnSc05hmRyP1BY7jn9xzvFfs9AVGHFCyT8e6X8Qhr4lrpsVx/wB7ptzpalXSJCFxPCI4zmw0XnQ4f4E3d4g/rpDnBAY4QEULc8R50UHdNoS1g859ircPiZwXVzYZrZtxof06z8h5s/itCTAnBLTb6c4LQngBUZ92tBPCVlkKCHLkRCWfSOTawtsEeTL3nQ4wuVOyMrV3kv53DXhUJA4dYU4IdBvA+NF0/7laU3toaAfwLZ/6x7ucicEz//5cHyMX5y6QlMOCYmMOFyfm/DXiPcG0ImbwMP8LSlgWJSQztCOkJqw48tOqgRBNvW8FyDgA0me46KEdIYshFCYW1iUBYHYiYl7QI8T9w+gEro9dl8J6QBxQmD4g2LX3+B/fMTh+zYQOlN3hh0QyWesA/BEaGWNOGuPQ7izYYef4Ho0Eh/H0RyzHzZZ183IbVMOCbWyCqXKG3GvTgrTtp1um2gjwOPh2n9ZEzIzswIkcKLqcDiONjLLVqeEzoR2hBDIMb+MuJemVnH4oX4DHh4RvxbLlRBOzzYZK4tw1NvxzpBoUpFKSGxopehWqk9IQpArdofDNcQcQRx3wZ2jyn+CQf/T5MfOwfinSFRtoYRkIIRGCYcJwvm3cIYPzpGBSTsP4pj1ICoy5047ZJnrV0KyEbI/HIb/c9PTTxPnRLDz1lTXIG1xbgklJIUQO5cS9X+UM4Hi3BbwHxnqZ7EmTi2hhKQQgqLnbTH/PxSnVHBmEPYJz57OpU1NKyGphPgbw/5hoG3ilAnsq4TDpzWDlZA0Qhz//WH/kAvEKRPsAjnH31eXknmVOCVCCUkhRBbONfyjY4bbva0EaQMlJIUQtqbiTVjEsVmc+w4lJIUQAn52hMPYcK5/EZ9VvPQNSkgGQrg+C37/GA4XCFdT2mGRvq1aUUIyEELkyqaEsA+Gw9bjsKvw/XVcoCfeu4YSkpEQolg2r0SY2XD4iDj+/ej8ndVLUaaEdEAIIaO+2/HcLZfLwv1RpPO58fHpZ0mwzFBCOiSkBq6ywbNfhPjarJ5HHVP2XidBMkEJ6ZKQGoqrzIsRx7lNTeOGzEE2ivdUKCE9ElIDW2Iw5iYY8C/h+Bvp+OvEa1soIX0ipAbbROZeySBn1NNBDjoy5vij4q0llJA+E1IDN/YgrUPhtEDK5eLcEkrIgAghuB8mkpZrDqdtnVZCUgixM3+OObMmXLEpTpkAEg6E06svbmsBJSSFEPiPDb+br4lTJiD8FeHwOcd7izglQglJISS+mh+E3ClOmYD494bDy8KIllBCUgixPfOmXb3epDi3BY/cgIEfDYfldnFxToQSkqFSh5H2xMLcmOXMFfj7UjgcZFacWkIJyUBIzql48Btf6Hwde+niJQIurYVhuQg7GsYx68VLSyghGQgh4PeScDgrjvknrtchjh0c5bVXezhAtJii4N6v0tZyEUpIRkJklHdfOGxm4bB82T9RomoLJSQjIQRJQStrF8J1cDKEOQCjZT6xQgnpgJAapCn8Y0grYuYCIsw74b2j6V0lpAtCauDGHeSYq2PxfbWXnbhKSA+EEDDgYPcYKiGdQQnpEUrIcicEFbztg4hwuZA4dQUlpEdC+g0lRAlZXCghSkhHUEKUkMWFEqKEdIQlRUhuYuIl3INX4M5Xx6zn/jwY8HwK4tlR+w33c+D+cXv4PhTmeR9ZtwJ0TcjMzIrRkjcG/6ciDh6MvAHG21rTKawf+iOfhl0+zMFFbomTadtM2+AWi5Bj7H4L198IBXga9c0wcqu1sdmEx1e4/kFcvwPZRlK5LVnSqwMGSyUkmPuA4Um8618D/e6AkXs7Ldvx/w65DXFxOngLO5RJpwUtGCG8n3P89+Ahr8a91JPo+iR2GNy+ubKeqhUhXOYJt80wwA09Gz+zmCNI73v8SAAPKKAeAycEiT6MB70SMphPP3Qijv9r6Puj8D1LWLCXPPOk00AkOKBmHwwePRu+/4RkF5tzkK2hBIudr+A3y+TNUHQT3M4suJUPwYBn4d5n4b4N16/juh9uvxv4W20NZu6GLjch3Stx3Y40z6M+uI/6hPqhCLb/7YAjP89xLcj+KeQ+/O+O8IUiBMreA+V3M7tyDSzPcZQougMqXZ7dzsMhaRAqDt3afBSgrczB6LfhegG/2MCz2Xv9rkdQL1Wn8q73AcR7CUiKnMrXUnolhCsrEChy7J3IPAx1E9w2sLUi3gcKWZhwCox7MdJtX2+x0rWzf2Ym7TySfqEwNXUsW4qw4XdbvTz8yoN4t+iYEAIPdXndT3B448bR8toTxHlRwK8yBN+6MrtCxRteErMXRnl7v75b1S34EgSNHjtXX7Pd7TykWrxYJBKCt65+ahqZjQeyxYdbeTWzKP4N7BiKbsE3k9+mynrM0kKDp1jnSt5pzOFyqw7k5FvDhLA4xU3z+/BNlrPiXzFAcCtDODNA5m3dC5a4ZatBCFsQwefkrlEZkKC/ArtHug6skwOmUB+gLFukL5qpiMxHtlyDsdMhXNua5FllsDKPuvuTQkUDrFDg2G4Fn0r/ZZaZQShIBr+hwezDNvxSFRSxlyY8XENsHZgcdkkIOohLtVXYNaSdHz1myfEPoXLc2o+TfBTdYZhDLMzRLHKb+lAKhUKhUCgUCoVCoVAoFAqFYkAYGvofZvPN/GfknbIAAAAASUVORK5CYII="/>
                  </defs>
                </svg>

                <h1 class="section__sub-title">Have world class marketing team?</h1>
                <p>
                  If you have experts with token marketing experience, read THE primer on ICO/STO
                  marketing and PR, and find out what really works! Learn the six easy steps to
                    guaranteed success and see if you are headed in the right direction.
                </p>
                <a class="inline-link" href="#contact">&#9656; Just click for more!</a>
              </article>
              <article class="col-lg-3 offset-lg-2 col-md-4 offset-md-1">
                <svg width="64" height="64" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                  <rect width="64" height="64" fill="url(#pattern0)"/>
                  <defs>
                  <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                  <use xlink:href="#image0" transform="scale(0.01)"/>
                  </pattern>
                  <image id="image0" width="100" height="100" xlink:href="data:image/png;base64,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"/>
                  </defs>
                </svg>

                <h1 class="section__sub-title">Have marketing team but need guidance?</h1>
                <p>
                  If your experts don’t have enough token marketing experience, you will need an
                  insider for supervision and creating the strategy. I will also represent your
                    brand at events and media appearances, and utilize my network if needed.
                </p>
                <a class="inline-link" href="#contact">&#9656; Just click for more!</a>
              </article>
            </div>
            <div class="row">
              <article class="col-lg-3 offset-lg-2 col-md-4 offset-md-1">
                
                <svg width="64" height="64" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                  <rect width="64" height="64" fill="url(#pattern0)"/>
                  <defs>
                  <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                  <use xlink:href="#image0" transform="scale(0.01)"/>
                  </pattern>
                  <image id="image0" width="100" height="100" xlink:href="data:image/png;base64,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"/>
                  </defs>
                </svg>

                <h1 class="section__sub-title">No marketing team? No problem!</h1>
                <p>
                  My team of top-notch experts and I will take the load off your back and provide a
                  beautiful white paper, a winning strategy, airdrop and proof-of-care campaigns, marketing
                  materials, events, analytics and so much more in one neat package.
                </p>
                <a class="inline-link" href="#contact">&#9656; Just click for more!</a>
              </article>
              <article class="col-lg-3 offset-lg-2 col-md-4 offset-md-1">
                
                <svg width="64" height="64" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                  <rect width="64" height="64" fill="url(#pattern0)"/>
                  <defs>
                  <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
                  <use xlink:href="#image0" transform="scale(0.01)"/>
                  </pattern>
                  <image id="image0" width="100" height="100" xlink:href="data:image/png;base64,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"/>
                  </defs>
                </svg>

                <h1 class="section__sub-title">Looking for the best private sales?</h1>
                <p>
                  Are you a crypto investor looking for some early intel on private sales yo wish you were invited for?
                  You’ve come to the right place!
                </p>
                <a class="inline-link" href="#contact">&#9656; Just click for more!</a>
              </article>
            </div>
          </div>
          <div class="text-center">
            <a href="#contact" class="btn btn-primary"
                    style="position:relative;top:8.675rem;">Contact me now</a>
          </div>
        </div>
      </section>

      <article class="section">
        <div class="container">
          <div class="row">
            <div class="col-sm-5">
              <h1 class="section__title">Testimonials</h1>

              <blockquote class="blockquote">
                <p class="h2">
                  If you want real marketing that works and effective implementation - Ikkk's got you covered. 
                  If you aren't sure, always go for Ikkk.
                </p>
                <footer class="blockquote-footer my-3">
                  <span class="">Dyanna Y.</span>
                  <a class="float-right inline-link" href="">&#9656; Visit his/her LinkedIn</a>
                </footer>
              </blockquote>
            </div>
            <div class="col-sm-5 offset-sm-2">
              <img width="480" class="img-fluid shaded" src="./assets/img/rawpixel-648567-unsplash.jpg" />
            </div>
          </div>
        </div>

      </article>

      <section class="section section--gray">
        <div class="container">
          <div class="row">
            <div class="col-sm-5 offset-sm-1 order-6">
              <h1 class="section__title">Blog</h1>
              <h2 class="section__lead">Get up to date on crypto news</h2>
              <div class="py-4">
                <follow-me />
              </div>
              <a href="#contact" class="btn btn-primary">Contact me now</a>
            </div>
            <div class="col-sm-6 order-1">
              <blog-posts />
            </div>
          </div>
        </div>

      </section>

      <article class="section">
        <div class="container">
          <div class="row">
            <div class="col-sm-5 offset-sm-1">
              
              <h1 class="section__title">About</h1>

              <p class="font-weight-bold">
                I have worked as a marketing and PR expert for over 15 years, consulting in over 20
            countries for companies such as BMW, Lufthansa, LG and Samsung. Later I worked with several
            high-profile crypto organizations, such as Bitcoinist and Bitcoin.com, and established my simple
            method for all but guaranteed success in the industry’s first go-to-market handbook: 
            <a class="inline-link" href="http://www.6steps.online/" target="_blank">“6 Proven Steps to Attract ICO Investors.”</a>
            I also founded <a class="inline-link" href="https://6slambo.com/" target="_blank">6S•LAMBO</a> 
            to provide a hassle-free, end to end integrated solution, using the 6-step methodology to connect 
            ICOs and STOs with their audience, build their trust and turn them into investors.
              </p>

              <p>
                I post regular opinion pieces on crypto investments on 
              <a class="inline-link" href="https://medium.com/@matyaszaborszky" target="_blank">my blog</a> and social media
              channels, frequently present at crypto and blockchain conferences, and am also a mentor,
              investor, entrepreneur, university lecturer and PGA enthusiast.
              </p>

              <p>
                My other interests include self improvement and business excellence. I am an avid
              follower of the Silva Method and have been publishing meditations, positive affirmations and
              other related material for years as a hobby. It’s fun and could really help you grow as a person
              and an entrepreneur. <a class="inline-link" href="">See for yourself!</a>
              </p>
            </div>
            <div class="col-sm-5 offset-sm-1">
              <img class="img-fluid" src="./assets/img/matyaslaunch.png" alt="">
            </div>
          </div>  
        </div>

      </article>

      <article id="contact" class="section section--gray">
        <div class="container">
          <div class="row">
            <div class="col-sm-6">
              <h1 class="section__title">Contact</h1>
              <h2 class="section__lead">Send me a message</h2>

              <p>
                For more detailed information on how I can help you achieve your goals, let me know how to reach
                you and I will get back to you within two working days.
              </p>

              <follow-me />
            </div>
            <div class="col-sm-6">
              <form action="">
                
                <div class="form-group">
                  <label class="form-label" for="">Full name</label>
                  <input type="text" class="form-control" name="name" maxlength="50" required />
                </div>

                <div class="form-group">
                  <label class="form-label" for="">Country</label>
                  <input type="text" class="form-control" name="country" maxlength="30" required />
                </div>

                <div class="form-group">
                  <label class="form-label" for="">Email</label>
                  <input type="email" class="form-control" name="email" maxlength="30" required />
                </div>

                <div class="form-group">
                  <label class="form-label" for="">Phone</label>
                  <input type="tel" class="form-control" name="tel" maxlength="30" required />
                </div>

                <div class="form-group">
                  <label class="form-label" for="">Telegram (optional)</label>
                  <textarea class="form-control" name="telegram"></textarea>
                </div>

                <button type="submit" class="btn btn-primary">
                  Done
                </button>

              </form>
            </div>
          </div>

        </div>


      </article>

    </main>

    <footer class="bg-primary text-white">
      <div class="section">

        <div class="container">

          <h1 class="sr-only">Matyas Zaborszky</h1>
          <div class="row">
            <div class="col">
              Matyas Zaborszky

              <follow-me />
            </div>

            <div class="col">
              <h1 class="h3">Contact</h1>

              <div class="my-3">
                Mátyás Zaborszky
              </div>

              <div class="my-3">
                <a class="inline-link" href="tel:1-305-447-7816">
                  1-305-447-7816
                </a>
              </div>

              <div class="my-3">
                <a class="inline-link" href="mailto:mz@matyaszaborszky.com">
                  mz@matyaszaborszky.com
                </a>
              </div>

              <address>
              10685-B Hazelhurst Dr. # 21025
              Houston, TX 77043
              </address>

            </div>

            <div class="col">
              <h1 class="h3">Services</h1>

              <div class="mt-3">My book</div> 
              <a class="inline-link" href="http://www.6steps.online/" target="_blank">&#9656; www.6steps.online</a>

              <div class="mt-2">Guide for you team</div>
              <a class="inline-link" href="" target="_blank">&#9656; www.tokenmarketing.expert</a>

              <div class="mt-2">Team for your Lambo</div>
              <a class="inline-link" href="https://6slambo.com/" target="_blank">&#9656; www.6slambo.com</a>
              
              <div class="mt-2">Tuti tippek</div>
              <a class="inline-link" href="" target="_blank">&#9656; www.privatesale.vip</a>

              <div class="mt-2">Blog, tuti hírekkel</div>
              <a class="inline-link" href="" target="_blank">&#9656; www.icoexpert.blog</a>

            </div>

            <div class="col">
              <h1 class="h3">Etc.</h1>
              <div class="mt-3">
                Privacy Policy
              </div>
              <div class="mt-3">
                Terms & Conditions 
              </div>
              <div class="mt-3">
                Earnings Disclaimer
              </div>
            </div>

          </div>
        </div>
      </div>

      <div class="copyright">
        <div class="container">
          Copyright &copy; 2018 &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;Matyas Zaborszky
          &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;All rights reserved.
          &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;AZ Organization LLC,  
           <address class="d-inline"> 10685-B Hazelhurst Dr. # 21025, Houston, TX 77043</address>
        </div>
      </div>

    </footer>
  </div>
</template>

<script>

import FollowMe from '@/components/FollowMe'
import BlogPosts from '@/components/BlogPosts'

export default {
  name: 'app',
  data () {
    return {
      navbarClass: ''
    }
  },
  mounted () {
    const callback = entries => { 
      entries.forEach(entry => {
        if (entry.intersectionRatio < 0.9) {
          this.navbarClass = 'show'
          return
        }
        this.navbarClass = ''
      })
    }
    const observer = new IntersectionObserver(callback, {
      root: null,
      rootMargin: '-100px',
      threshold: Array(100 + 1)
        .fill(0)
        .map((_, index) => index / 100 || 0)
    })
    observer.observe(this.$refs['first-content'])

  },
  components: {
    FollowMe,
    BlogPosts
  }
}
</script>

<style lang="scss">
@import "./assets/scss/app";

.section {
  padding-top: $section-spacing;
  padding-bottom: $section-spacing;
}
.section--head {
  background: url('./assets/img/header-bg.png') no-repeat;
  background-position: 0 0;
  background-size: 100% auto;
}
.section--gray {
  background: $light-gray;
}
.section__title {
  font-size: 1rem;
  font-weight: 300;
  color: $gray;
  font-family: $font-family-base;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
}
.section__sub-title {
  font-family: $font-family-base;
  font-size: 1.5rem;
  margin: 1.5rem 0;
}
.section__lead {
  font-size: 3.5rem;
  margin: 1.5rem 0;
}
.section__sub-lead {
  font-size: 1.5rem;
  margin: 2rem 0;
}
.form-label {
  color: $gray;
  text-transform: uppercase;
}
.shaded {
  box-shadow: 20px 20px 0 rgba(0, 0 , 0, .05)
}
.inline-link {
  display: inline-block;
  font-weight: bold;
  padding-left: 3px;
  padding-right: 3px;
  margin-left: -3px;
  margin-right: -3px;
}

.copyright {
  background: $dark-green;
  padding: 1.5rem 0;
}

</style>