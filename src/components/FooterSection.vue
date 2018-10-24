<template>
  <footer class="bg-primary text-white">
      <div class="section">

        <div class="container">

          <h1 class="sr-only">Matyas Zaborszky</h1>
          <div class="row">
            <div class="col-md-6 col-lg-3 mb-3">
              <img src="../assets/img/logo.svg" alt="Matyas Zaborszky" class="mb-4 mt-2 img-fluid">
              <follow-me />
            </div>

            <div class="col-md-6 col-lg-3 mb-3">
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

            <div class="col-md-6 col-lg-3 mb-sm-4">
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

            <div class="col-md-6 col-lg-3">
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
</template>

<script>
import FollowMe from '@/components/FollowMe'
export default {
  name: 'FooterSection',
  components: {
    FollowMe
  }
}
</script>

