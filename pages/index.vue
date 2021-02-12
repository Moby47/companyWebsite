<template>
  

<div>

  
  <!-- banner section -->
  <section id="home" class="banner">
      <div id="banner-bg-effect" class="banner-effect"></div>
      <div class="container">
          <div class="row align-items-center">
              <div class="col-lg-7 col-md-12 col-sm-12 order-lg-first mt-lg-0 custom-margin">
                  <h1 class="mb-4 title title-size">

                    <strong>We Make </strong>Technology, <br>work <strong>for you.</strong>
                  </h1>
                  <p>We live in a digital era where
                      everything can be done on the Internet. Modern users value their time.
                       They go online to shop and book services, and if they cannot locate your 
                    company or struggle to find their 
                    way around your website – you are losing money.</p>
                  <div class="mt-5">
             <nuxt-link class="btn btn-primary btn-style mr-2 text-white" to="/about">Read More </nuxt-link>
          <nuxt-link class="btn btn-outline btn-outline-style text-white custom-hover" to="/services">Our Services </nuxt-link>
                  </div>
              </div>
              <div class="col-lg-5 col-md-12 col-sm-12 order-first text-lg-left text-center">
                  <div>
                      <img src="@/assets/images/cohotek-it-company.png" alt="cohotek IT company"
                       class="rounded-circle img-fluid hide-mobile">
                  </div>
              </div>
          </div>
      </div>
  </section>
  <!-- //banner section -->
  
  <!-- home page about -->
  <section class="w3l-about section-bg-color text-white">
      <div class="container">
          <div class="row about-content">
              <div class="col-lg-6 info mb-lg-0 mb-sm-5 mb-4 align-center">
                  <h3 class="title">Experience IT</h3>
                  <h6>Do you have trouble reaching your clients and customers online? Poor
                      web presence might be the reason why!</h6>
                  <p class="mt-md-4 mt-3 mb-0"> Our staff comprises of experienced specialists in the field of<strong> Microsoft product support, web development, SEO promotion,
                      web design, and IT training. </strong>
                     Your website is your online business card. Develop your brand with CohoTek to stay 
                     ahead of the competition!</p>
              </div>
              <div class="col-lg-6">
                  <img src="@/assets/images/cohotek-web-search.png" class="img-fluid img-shadow" 
                  alt="cohotek IT web development company">
              </div>
          </div>
      </div>
  </section>
  <!-- //home page about -->
  
  <!-- home page service grids -->
  <section id="services" class="bg-light">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
          <h4 class="section-title">IT Problems Begone</h4>
          <p class="text-center">We are a full-stack web development company offering a full 
            spectrum of services linked to the internet. 
              Hire us, and in a short period of time, you will notice a significant boost in your revenue and number of clients.</p>
        </div>
      </div>
      <div class="row mt-lg-5">
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="box-wrap">
            <div class="icon">
              <span class="fa fa-briefcase"></span>
            </div>
            <h4><a href="#url">Business Services</a></h4>
            <p>We are a one-stop IT solutions company with a difference,
              we want to change the world by the way we do business.</p>
          </div>
        </div>
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="box-wrap">
            <div class="icon">
              <span class="fa fa-shield"></span>
            </div>
            <h4><a href="#url">Product Consulting</a></h4>
            <p>A team of dedicated Product Consulting Services experts
               provides solutions to meet your management challenges.</p>
          </div>
        </div>
       
        <div class="col-lg-4 col-md-6 col-sm-12">
          <div class="box-wrap">
            <div class="icon">
              <span class="fa fa-globe"></span>
            </div>
            <h4><a href="#url">Projects Worldwide</a></h4>
            <p>We are opened to a market of vast populations that could be interested all around the world.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- //home page service grids -->
  
  <!-- testimonials section -->
  <section id="slider" class="testimonials">
      <div class="container">
          <div class="row align-items-center">
              <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
                  <h4 class="section-title">Building the Future with Tech</h4>
                  <p class="text-center">
                      Testimonies from satisfied clients.</p>
              </div>
          </div>
          <div class="large-12 columns mt-5">
              <div class="owl-carousel owl-theme">
                  <div class="item">
                      <div class="w3l-customers-7">
                          <div class="customers_sur">
                              <div class="customers-left_sur">
                                  <div class="customers_grid">
                                      <div class="ratings my-4 my-4">
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                      </div>
                                      <p>Fantastic job! i will surely refer a friend to your company.</p>
                                      <div class="customers-bottom_sur">
                                          <div class="custo_grid">
                                              <h5>Joe</h5>
                                              <span><a href='https://carspar.com.ng' target='_blank'>
                                                carspar.com.ng</a></span>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>

                  <div class="item">
                      <div class="w3l-customers-7">
                          <div class="customers_sur">
                              <div class="customers-left_sur">
                                  <div class="customers_grid">
                                      <div class="ratings my-4">
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                      </div>
                                      <p>I love my online shop, thanks Cohotek! keep up the good work.</p>
                                      <div class="customers-bottom_sur">
                                          <div class="custo_grid">
                                              <h5>Eweje</h5>
                                              <span><a href='https://habitat.com.ng' target='_blank'>
                                                habitat.com.ng</a></span>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>

                  <div class="item">
                      <div class="w3l-customers-7">
                          <div class="customers_sur">
                              <div class="customers-left_sur">
                                  <div class="customers_grid">
                                      <div class="ratings my-4">
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                      </div>
                                      <p>great job! i hope to work with you in the future.</p>
                                      <div class="customers-bottom_sur">
                                          <div class="custo_grid">
                                              <h5>Henry</h5>
                                              <span><a href='https://getfoods.ng' target='_blank'>
                                                getfoods.ng</a></span>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              
                  <div class="item" >
                      <div class="w3l-customers-7" >
                          <div class="customers_sur">
                              <div class="customers-left_sur">
                                  <div class="customers_grid">
                                      <div class="ratings my-4">
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                          <span class="fa fa-star"></span>
                                      </div>
                                      <p>Amazing customer service! thanks Cohotek.</p>
                                      <div class="customers-bottom_sur">
                                          <div class="custo_grid">
                                              <h5>Ebele</h5>
                                              <span><a href='https://mylingualink.com' target='_blank'>
                                                mylingualink.com</a></span>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
                 
              </div>
          </div>
      </div>
  </section>
  <!--//testimonials section -->
  
  <!-- stats section -->
  <section id="stats" class="stats">
      <div class="container">
          <div class="row">
              <div class="col-lg-5 margin-md-60">
                  <h2 class="left-title">Behind the scenes.</h2>
                  <p class="white">Some of Our Company Real Facts</p>
              </div>
              <div class="col-lg-7 mt-lg-0 mt-5">
                  <div class="d-sm-flex justify-content-lg-around justify-content-between counter-main">
                      <div class="counter">
                          <div class="icon">
                              <span class="fa fa-folder-open-o"></span>
                          </div>
                          <p class="value">{{projectCount}}</p>
                          <p class="title white">Projects</p>
                      </div>
                      <div class="counter">
                          <div class="icon">
                              <span class="fa fa-headphones"></span>
                          </div>
                          <p class="value">32</p>
                          <p class="title white">Consultant</p>
                      </div>
                      <div class="counter">
                          <div class="icon">
                              <span class="fa fa-trophy"></span>
                          </div>
                          <p class="value">11</p>
                          <p class="title white">Awards</p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </section>
  <!-- //stats section -->
  
  <!-- homepage blog grids -->
  <section id="blog">
      <div class="container">
          <div class="row align-items-center">
              <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
                  <h4 class="section-title">Our Blog</h4>
                  <p class="text-center">Stay informed. Technology made simple.</p>
              </div>
              
          </div>

          <div class="text-center" v-show='loading'>
          <v-progress-circular
            indeterminate
            color="primary"
          ></v-progress-circular>
                </div>

                <div class="text-center" v-show='err'>
                  Network error. Please reload.
                </div>
          
          <div class="blog-grids row mt-5">
              <div class="col-lg-4 col-md-6 col-sm-12 blog-grid" id="zoomIn" v-for='post in posts' v-bind:key='post.id'>
                  <nuxt-link :to="'/blog/'+post.id+'/'+post.title_slug">
   <figure><img :src="'https://henrymoby.website/storage/blog/pwa_1559904166.png'"
    class="img-fluid custom-height" :alt="post.title"></figure>
                  </nuxt-link>
                  <div class="blog-info">
                      <h3><nuxt-link :to="'/blog/'+post.id+'/'+post.title_slug">
                        {{post.title}}
                      </nuxt-link> </h3>
                      <ul>
                       <li><span class="fa fa-calendar mr-2"></span>{{post.created_at}}</li>
                      </ul>
                  </div>
              </div>
              

              
          </div>

          <p class='text-center'>
              <nuxt-link to='blog' class="btn btn-primary btn-style mt-2 text-center">View More</nuxt-link>
                        </p>
      </div>
  </section>
  <!-- //homepage blog grids -->
  
  
</div>

  

</template>

<script>
//import Logo from '~/components/Logo.vue'
//import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {

  head(){
    return {
      title: "Web Development IT Company in Lagos Nigeria",
      meta:[
        
          { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
          { name: 'keywords', content: 'web development in lagos, digital marketing, seo, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },
        
      ]
    }
  },
  
  data () {

    return {
    projectCount: '-',
    posts:[],
    loading: true,
    err: false,
    }
    
  },

  methods: {

  getProjectCount(){
      fetch('https://cohotekapi.getfoods.ng/api/project-count', {
      method: 'GET',
      headers: {
        'Content-Type': 'application/json',
        'X-Authorization': 'w69D58JnTvtUCH3KHcfhSGNIO7NtLuJEAF7ixJDwSHCGiTpdLUWdhvROVWt8TaUf'
      }
    })
      .then(res => res.json())
      .then(res=>{
        this.projectCount = res;
        console.log(res)
      })
      .catch(error =>{
        console.log(error)
        this.projectCount = '-';      
          })
  },
  //method end


  getPosts(){
      fetch('https://cohotekapi.getfoods.ng/api/posts', {
      method: 'GET',
      headers: {
        'Content-Type': 'application/json',
        'X-Authorization': 'w69D58JnTvtUCH3KHcfhSGNIO7NtLuJEAF7ixJDwSHCGiTpdLUWdhvROVWt8TaUf'
      }
    })
      .then(res => res.json())
      .then(res=>{
        this.posts = res.data;
        console.log(this.posts)
        this.loading = false
      })
      .catch(error =>{
        console.log(error)  
        this.loading = false    
        this.err = true
          })
  },
  //method end

  },

  mounted() {
  
  // get project count
  this.getProjectCount()

  //get blog posts
  this.getPosts()

      /*===================================*
	02. BACKGROUND ANIMATION JS
	*===================================*/
  
  var $particles_js = $("#banner-bg-effect");
  if ($particles_js.length > 0) {
    particlesJS(
      "banner-bg-effect",
      // Update your personal code.
      {
        particles: {
          number: {
            value: 80,
            density: {
              enable: true,
              value_area: 800
            }
          },
          color: {
            value: "#ffffff"
          },
          shape: {
            type: "circle",
            stroke: {
              width: 0,
              color: "#ffffff"
            },
            polygon: {
              nb_sides: 5
            },
            image: {
              src: "img/github.svg",
              width: 100,
              height: 100
            }
          },
          opacity: {
            value: 0.4,
            random: false,
            anim: {
              enable: false,
              speed: 1,
              opacity_min: 0.5,
              sync: false
            }
          },
          size: {
            value: 3,
            random: true,
            anim: {
              enable: false,
              speed: 20,
              size_min: 0.2,
              sync: false
            }
          },
          line_linked: {
            enable: true,
            distance: 150,
            color: "#ffffff",
            opacity: 0.2,
            width: 1
          },
          move: {
            enable: true,
            speed: 6,
            direction: "none",
            random: false,
            straight: false,
            out_mode: "out",
            bounce: false,
            attract: {
              enable: false,
              rotateX: 600,
              rotateY: 1200
            }
          }
        },
        interactivity: {
          detect_on: "canvas",
          events: {
            onhover: {
              enable: false,
              mode: "repulse"
            },
            onclick: {
              enable: false,
              mode: "push"
            },
            resize: true
          },
          modes: {
            grab: {
              distance: 400,
              line_linked: {
                opacity: 1
              }
            },
            bubble: {
              distance: 400,
              size: 20,
              duration: 2,
              opacity: 1,
              speed: 3
            },
            repulse: {
              distance: 200,
              duration: 0.4
            },
            push: {
              particles_nb: 4
            },
            remove: {
              particles_nb: 2
            }
          }
        },
        retina_detect: true
      }
    );
  }
    /*===================================*
	02. BACKGROUND ANIMATION JS
  *===================================*/
  
     /*===================================*
	Owl carousel
	*===================================*/
  
  $(document).ready(function () {
    var owl = $('.owl-carousel');
    owl.owlCarousel({
      margin: 10,
      nav: true,
      loop: false,
      responsive: {
        0: {
          items: 1
        },
        767: {
          items: 2
        },
        1000: {
          items: 3
        }
      }
    })
  })

   /*===================================*
	Owl carousel
  *===================================*/
  
  //collapse nav on component load
  $('#navbarNav').hide('fade');
  
},

  components: {
  //  Logo,
  //  VuetifyLogo
  }
}
</script>
