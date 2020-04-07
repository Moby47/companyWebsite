<template>
  
    <!--
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-btn
        icon
        @click.stop="miniVariant = !miniVariant"
      >
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>
      <v-btn
        icon
        @click.stop="clipped = !clipped"
      >
        <v-icon>mdi-application</v-icon>
      </v-btn>
      <v-btn
        icon
        @click.stop="fixed = !fixed"
      >
        <v-icon>mdi-minus</v-icon>
      </v-btn>
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-btn
        icon
        @click.stop="rightDrawer = !rightDrawer"
      >
        <v-icon>mdi-menu</v-icon>
      </v-btn>
    </v-app-bar>
-->
    <div>
    
        <!-- site header -->
<header id="site-header" class="fixed-top">
    <nav class="navbar navbar-expand-lg navbar-dark">
        <a class="navbar-brand" href="index.html">
            <span class="fa fa-shield"></span> Captivate
        </a>
        <button class="navbar-toggler bg-gradient" type="button" data-toggle="collapse"
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
                    <nuxt-link class="nav-link" to="about">About</nuxt-link>
                </li>
                <li class="nav-item">
                    <nuxt-link class="nav-link" to="services">Services</nuxt-link>
                </li>
                <li class="nav-item">
                  <nuxt-link class="nav-link" to="project">portfolio</nuxt-link>
              </li>
                <li class="nav-item">
                    <nuxt-link class="nav-link" to="contact">Contact</nuxt-link>
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
        <div class="container my-md-5 my-4">
          <div class="row">
            <div class="col-lg-4">
              <div class="footer-logo mb-3">
                <a href="index.html">
                  <span class="fa fa-shield"></span> Captivate
                </a>
              </div>
              <div>
                <p class="">Lorem ipsum dolor, sit amet consectet et adipis icing elit. Ab commodi iure minus
                  laboriosam
                  placeat quia, dolorem animi. Eveniet repudiandae, perferendis nesciunt deserunt iure et, consequatur
                  optio!</p>
              </div>
            </div>
            <!-- Quick Links -->
            <div class="col-lg-3 col-md-4 mt-lg-0 mt-5">
              <h4 class="footer-title">Quick Links</h4>
              <ul class="footer-list">
                <li><a href="about.html"> About company</a></li>
                <li><a href="services.html"> Explore services</a></li>
                <li><a href="#work"> How does we Work?</a></li>
                <li><a href="#projects"> View projects</a></li>
              </ul>
            </div>
            <!-- Newsletter -->
            <div class="col-lg-5 col-md-8 mt-lg-0 mt-5">
              <h4 class="footer-title">Newsletter</h4>
              <p class="mb-4">By subscribing to our mailing list you will always be updated with the latest news from us.
              </p>
              <form class="newsletter-form">
                <input class="input-rounded" type="text" required="" placeholder="Enter Email Address">
                <button type="submit" title="Subscribe" class="btn btn-primary btn-style" name="submit" value="Submit">
                  Subscribe
                </button>
              </form>
            </div>
          </div>
        </div>
      </div>
      <div class="bottom-footer">
        <div class="container">
          <div class="row">
            <div class="col-lg-8 text-lg-left text-center mb-lg-0 mb-3">
              <p class="copyright">© 2020 Captivate. All Rights Reserved. Design by <a
                href="https://w3layouts.com/">W3Layouts</a></p>
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
      script: [
      { src: 'js/jquery-3.3.1.min.js' },
      { src: 'https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js' },
      { src: 'js/particles.min.js' },
      { src: 'js/script.js' },
      { src: 'js/lightbox-plus-jquery.min.js' },
      { src: 'js/custom.js' },
      { src: 'js/owl.carousel.js' },
      ]
    }
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
