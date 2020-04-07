<template>

        <div>
          
        
      
<!-- about page breadcrumns -->
<section class="inner-banner">

    </section>
    <nav aria-label="breadcrumb">
        <ol class="breadcrumb breadcrumb-padding">
            <li class="breadcrumb-item"><a href="index.html">Home</a></li>
            <li class="breadcrumb-item active" aria-current="page">Portfolio</li>
        </ol>
    </nav>
    <!-- //about page breadcrumns -->
    
    <!-- homepage blog grids -->
    <section id="blog">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
                    <h4 class="section-title">Company Portfolio</h4>
                    <p class="text-center">There are many variations of passages of Lorem Ipsum available, but the majority
                        have
                        suffered alteration in some form, by injected humour</p>
                </div>
            </div>
            <div class="blog-grids row mt-5">
                <div class="col-lg-4 col-md-6 col-sm-12 blog-grid" id="zoomIn">
                    <a href="#blog-single.html">
                        <figure><img src="@/assets/images/blog.jpg" class="img-fluid" alt=""></figure>
                    </a>
                    <div class="blog-info">
                        <h3><a href="#blog-single.html">4 Steps To Consider Before You Start</a> </h3>
                        <ul>
    <!--<li><a href="#author"><span class="fa fa-user-o mr-2"></span>Johnson smith</a></li>-->
                            <li><span class="fa fa-calendar mr-2"></span>Jan 16, 2020</li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12 mt-md-0 mt-4 blog-grid" id="zoomIn">
                    <a href="#blog-single.html">
                        <figure><img src="@/assets/images/blog1.jpg" class="img-fluid" alt=""></figure>
                    </a>
                    <div class="blog-info">
                        <h3><a href="#blog-single.html">Strategic Plan Execution Management</a> </h3>
                        <ul>
                       <!--     <li><a href="#author"><span class="fa fa-user-o mr-2"></span>Alexander</a></li>-->
                            <li><span class="fa fa-calendar mr-2"></span>Jan 19, 2020</li>
                        </ul>
                    </div>
                </div>
                <div class="col-lg-4 col-md-6 col-sm-12 mt-lg-0 mt-4 blog-grid" id="zoomIn">
                    <a href="#blog-single.html">
                        <figure><img src="@/assets/images/blog2.jpg" class="img-fluid" alt=""></figure>
                    </a>
                    <div class="blog-info">
                        <h3><a href="#blog-single.html">Business planning, strategy and execution</a> </h3>
                        <ul>
                        <!--   <li><a href="#author"><span class="fa fa-user-o mr-2"></span>Elizabeth ker</a></li>-->
                            <li><span class="fa fa-calendar mr-2"></span>Jan 21, 2020</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <!-- //homepage blog grids -->
     
      
        </div>
        
        </template>
        
        <script>
        //import Logo from '~/components/Logo.vue'
        //import VuetifyLogo from '~/components/VuetifyLogo.vue'
        
        export default {
          
          mounted(){
            //collapse nav on component load
            $('#navbarNav').hide('fade');
          },
          
          components: {
          //  Logo,
          //  VuetifyLogo
          }
        }
        </script>
        