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
                                get in touch with us or call our technical lead directly: <b> <a href='tel:+2348074247448' style='text-decoration:underline;'> Oghogho Airhunde</a></b> </p>
                        </div>
                        <div class="column2">
                            <div class="contact-para contact-info-align">
                                <div class="icon">
                                    <span class="fa fa-map-marker"></span>
                                </div>
                               <div>
                                    <strong class="info">Address:</strong>
                                         No 17 A. Ozumba Mbadiwe. Victoria Island
                                </div>
                            </div>
                            <div class="contact-info-align">
                                <div class="icon">
                                    <span class="fa fa-phone"></span>
                                </div>
                                <div>
                                    <strong class="info">Phone:</strong>
                                        <a href="tel:+2348035562231"> +2348035562231</a> ,
                                    <a href="tel:+2347069685282"> +2347069685282</a>
                                </div>
                            </div>
                            <div class="contact-info-align">
                                <div class="icon">
                                    <span class="fa fa-envelope-open-o"> </span>
                                </div>
                                <div>
                                    <strong class="info">Email:</strong> 
                                    <a href="mailto:henryonyemaobi@gmail.com">
                                        henryonyemaobi@gmail.com</a>
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
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3964.6589273286695!2d3.4100281147702547!3d6.437831895342325!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103b8ad63435c713%3A0xe1a93bf07adefdb6!2sThe%20Wings%20Complex!5e0!3m2!1sen!2sng!4v1586457537768!5m2!1sen!2sng"
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
                    <h4 class="section-title">we want to hear from you</h4>
                </div>
                <!-- contact form -->
                <form action="#" method="post">
                    <div class="main-input">
                        <div>
                            <input type="text" name="name" id="w3lName" placeholder="Your Name" class="contact-input"
                                required v-model='name' v-validate='"required|max:49"'/>
                                <transition  name="fadeLeft">
                 <span class='custom-alert' v-show="errors.has('name')">{{ errors.first('name') }}</span>
                                </transition> 
                        </div>
                        <div>
                            <input type="email" name="email" v-validate='"required|email"' id="w3lSender" placeholder="Your Email"
                                class="contact-input" required v-model='email' />
                                <transition  name="fadeLeft">
                                        <span class='custom-alert' v-show="errors.has('email')">{{ errors.first('email') }}</span>
                                       </transition> 
                        </div>
                        <div>
                            <input type="text" name="subject" v-validate='"required|max:50"' id="w3lSubject" placeholder="Subject" class="contact-input"
                            v-model='subject' required />
                            <transition name="fadeLeft">
                                    <span class='custom-alert' v-show="errors.has('subject')">{{ errors.first('subject') }}</span>
                                   </transition> 
                        </div>
                    </div>
                    <textarea class="contact-textarea" v-validate='"required|max:254"' name="message" id="w3lMessage" v-model='message'
                        placeholder="Type your message here" required></textarea>
                        <transition name="fadeLeft">
                                <span class='custom-alert' v-show="errors.has('message')">{{ errors.first('message') }}</span>
                               </transition> 	
                    <div class="text-right">
                        <button class="btn btn-style btn-primary" @click.prevent='contact()'>Submit</button>
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

       import axios from 'axios'
        export default {
          
            head(){
            return {
            title: "Contact Us for Web Development projects",
            meta:[
                
                { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
                { name: 'keywords', content: 'digital marketing, seo, web development in lagos, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },
                
            ]
            }
        },

            data(){
			return{
				name: '',
				email: '',
				subject: '',
				message: '',
			}
		},
        
          methods: {

            contact(){

			 //validate
             this.$validator.validateAll().then(() => {
           
           if (!this.errors.any()) {
                  //if no error
                  this.$nuxt.$loading.start()
     
                 // instantiant formdata object
            const formdata  = new FormData();
         //append form data to formdata
         formdata.append('name',  this.name);
         formdata.append('email', this.email);
         formdata.append('subject', this.subject);
         formdata.append('message', this.message);
         
         //send to database with axios
         console.log(formdata)
     
         axios.post('https://cohotekapi.getfoods.ng/api/contact',formdata)
         .then(res=>{
       if(res.data == 'ok'){
         this.$nuxt.$loading.finish()
         alert("Thank you! You will be contacted shortly.");
         
          //clear form
          this.name = '';
         this.email ='';
         this.subject= '';
         this.message= '';
         //clear form and errorbag
         setTimeout(func=>{
             this.errors.clear()
         },1) 
      
       }else{
         this.$nuxt.$loading.finish()
         alert("An Error Occured, Please call +2348035562231 or send an email to support@cohotek.tech");
       }
     
       })
       .catch(err=>{
           console.log(err)
           this.$nuxt.$loading.finish()
       })
     
        
          }else{
            //error occured and was shown
          }
         
         }); //validator

        }//method end

          },

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
        