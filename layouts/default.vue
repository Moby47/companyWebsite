<template>
  
    <div>
    
        <!-- site header -->
<header id="site-header" class="fixed-top">
    <nav class="navbar navbar-expand-lg navbar-dark">
        <nuxt-link  class="navbar-brand" to="/">
            <span class="fa fa-shield"></span> CohoTek
        </nuxt-link>
        <button class="navbar-toggler bg-gradient" type="button" data-toggle=""
            data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
            aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
  
        <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav m-auto">
                <li class="nav-item">
         <nuxt-link  class="nav-link" to="/">Home <span class="sr-only">(current)</span></nuxt-link >
                </li>
                <li class="nav-item">
                    <nuxt-link class="nav-link" to="/about">About</nuxt-link>
                </li>
                <li class="nav-item">
                    <nuxt-link class="nav-link" to="/services">Services</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link" to="/portfolio">portfolio</nuxt-link>
              </li>
              <li class="nav-item">
                  <nuxt-link class="nav-link" to="/blog">blog</nuxt-link>
              </li>
                <li class="nav-item">
                    <nuxt-link class="nav-link" to="/contact">Contact</nuxt-link>
                </li>
            </ul>
          <!--  <ul class="navbar-nav">
                <li class="nav-item">
                    <a href="#demo" class="btn btn-primary btn-style">View Demo</a>
                </li>
            </ul>
          -->
        </div>
    </nav>
  </header>
  <!-- //site header -->

        <nuxt />
    
        
  <!-- site footer -->
  <footer id="site-footer">
      <div class="top-footer">
        <div class="container">
          <div class="row">
            <div class="col-lg-8">
              <div class="footer-logo mb-3">
                  <nuxt-link  class="navbar-brand" to="/">
                    <span class="fa fa-shield"></span> CohoTek
                </nuxt-link>
              </div>
              <div>
                <p class="">CohoTek IT Solutions is a one-stop IT company dedicated to creating value
                    through our products and services. We focus on efficiency, easy of use and affordability in all of 
                   our products and services and have only one major goal – making our customers happy.
                  </p>
              </div>
            </div>
            <!-- Quick Links -->
            <div class="col-lg-4 col-md-12 mt-lg-0 mt-5">
              <h4 class="footer-title">Quick Links</h4>
              <ul class="footer-list">
                <li><nuxt-link to="/about"> About company</nuxt-link></li>
                <li><nuxt-link to="/services"> Explore services</nuxt-link></li>
                <li><nuxt-link to="/contact"> Contact us?</nuxt-link></li>
                <li><nuxt-link to="/portfolio"> View projects</nuxt-link></li>
              </ul>
            </div>
            <!-- Newsletter 
            <div class="col-lg-5 col-md-8 mt-lg-0 mt-5">
              <h4 class="footer-title">Newsletter</h4>
              <p class="mb-4">By subscribing to our mailing list you will be updated with the latest news from us.
              </p>
              <form class="newsletter-form">
                <input class="input-rounded" type="text" required="" placeholder="Enter Email Address">
                <button type="submit" title="Subscribe" class="btn btn-primary btn-style" name="submit" value="Submit">
                  Subscribe
                </button>
              </form>
            </div>
            -->
          </div>
        </div>
      </div>
      <div class="bottom-footer">
        <div class="container">
          <div class="row">
            <div class="col-lg-8 text-lg-left text-center mb-lg-0 mb-3">
            <!-- <p class="copyright">© 2020 Captivate. All Rights Reserved. Design by <a
                href="https://w3layouts.com/">W3Layouts</a></p>--> 
                <p class="copyright">© 2020. All Rights Reserved. <a
                  href="https://cohotek.tech">CohoTek</a></p>
            </div>
            <div class="col-lg-4 align-center text-lg-right text-center">
              <a href="#facebook" class="social-item"><span class="fa fa-facebook-f"></span></a>
              <a href="#twitter" class="social-item"><span class="fa fa-twitter"></span></a>
              <a href="#linkedin" class="social-item"><span class="fa fa-linkedin"></span></a>
            </div>
          </div>
        </div>
      </div>
    </footer>
    <!-- //site footer -->
  
    <!-- move top -->
  <button onclick="topFunction()" id="movetop" class="bg-primary" title="Go to top">
      <span class="fa fa-angle-up"></span>
    </button>

    
    </div>
    
</template>

<script>
export default {

  head () {
    return {
     /* script: [
      { src: 'js/jquery-3.3.1.min.js' },
      { src: 'https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js' },
      { src: 'js/particles.min.js' },
      { src: 'js/script.js' },
      { src: 'js/lightbox-plus-jquery.min.js' },
      { src: 'js/custom.js' },
      { src: 'js/owl.carousel.js' },
      ]*/
    }
  },

  mounted(){
    
  },

  data () {
    return {
    /*
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'

      */
    }
    
  }
}
</script>
