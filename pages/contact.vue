<template>

        <div>
          
        
      
<!-- contact page breadcrumns -->
<section class="inner-banner">

    </section>
    <nav aria-label="breadcrumb">
        <ol class="breadcrumb breadcrumb-padding">
                <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
            <li class="breadcrumb-item active" aria-current="page">Contact</li>
        </ol>
    </nav>
    <!-- contact page breadcrumns -->
    
    <!-- contact section -->
    <section class="w3l-contact3">
        <div class="contact1-bg section-gap">
            <div class="container">
                <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12 px-lg-3 px-0">
                    <h4 class="section-title">Get in touch with us</h4>
                    <p class="text-center">Your vision, our Tech. Let us take you online.</p>
                </div>
                <div class="row contact-main mt-5">
                    <div class="col-md-6 ">
                        <div class="column">
                            <h3 class="header">We are here for you</h3>
                            <p class="head-main">For more information or inquiry
                                 about our services, projects and pricing
                                please feel free to
                                get in touch with us.</p>
                        </div>
                        <div class="column2">
                            <div class="contact-para contact-info-align">
                                <div class="icon">
                                    <span class="fa fa-map-marker"></span>
                                </div>
                               <div>
                                    <strong class="info">Address:</strong class="info">
                                         No 00. Ozumba Mbadiwe. Victoria Island
                                </div>
                            </div>
                            <div class="contact-info-align">
                                <div class="icon">
                                    <span class="fa fa-phone"></span>
                                </div>
                                <div>
                                    <strong class="info">Phone:</strong class="info">
                                        <a href="tel:+2348035562231"> Phone Number 1</a> ,
                                    <a href="tel:+2348035000000"> Phone Number 2</a>
                                </div>
                            </div>
                            <div class="contact-info-align">
                                <div class="icon">
                                    <span class="fa fa-envelope-open-o"> </span>
                                </div>
                                <div>
                                    <strong class="info">Email:</strong> 
                                    <a href="mailto:support@cohotek.tech">
                                        support@cohotek.tech</a>
                                </div>
                            </div>
                        </div>
                        <div class="column3">
                            <h3 class="header follow">Follow us </h3>
                            <a href="#facebook" class="facebook" title="facebook"><span class="fa fa-facebook"></span></a>
                            <a href="#twitter" class="twitter" title="twitter"><span class="fa fa-twitter"></span></a>
                            <a href="#linkedin" class="linkedin" title="linkedin"><span class="fa fa-linkedin"></span></a>
                            <a href="#instagram" class="instagram" title="instagram"><span
                                    class="fa fa-instagram"></span></a>
                        </div>
                    </div>
                    <!-- map iframe-->
                    <div class="col-md-6 map mt-lg-0 mt-4">
                        <iframe
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d387190.2895687731!2d-74.26055986835598!3d40.697668402590374!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c24fa5d33f083b%3A0xc80b8f06e177fe62!2sNew+York%2C+NY%2C+USA!5e0!3m2!1sen!2sin!4v1562582305883!5m2!1sen!2sin"
                            frameborder="0" style="border:0" allowfullscreen=""></iframe>
                    </div>
                    <!-- //map iframe -->
                </div>
            </div>
        </div>
    </section>
    
    <section class="contact-form">
        <div class="container">
            <div class="contacts12-main">
                <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12 mb-md-5 mb-3">
                    <h4 class="section-title">we want to here from you</h4>
                </div>
                <!-- contact form -->
                <form action="https://sendmail.w3layouts.com/submitForm" method="post">
                    <div class="main-input">
                        <div>
                            <input type="text" name="w3lName" id="w3lName" placeholder="Your Name" class="contact-input"
                                required />
                        </div>
                        <div>
                            <input type="email" name="w3lSender" id="w3lSender" placeholder="Your Email"
                                class="contact-input" required />
                        </div>
                        <div>
                            <input type="text" name="w3lSubject" id="w3lSubject" placeholder="Subject" class="contact-input"
                                required />
                        </div>
                    </div>
                    <textarea class="contact-textarea" name="w3lMessage" id="w3lMessage"
                        placeholder="Type your message here" required></textarea>
                    <div class="text-right">
                        <button class="btn btn-style btn-primary">Submit</button>
                    </div>
                </form>
                <!-- //contact form -->
            </div>
        </div>
    </section>
    <!-- //contact section -->
     
      
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
        