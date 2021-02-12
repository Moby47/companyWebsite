<template>

        <div>
          
        
      
<!-- blog single page breadcrumns -->
<section class="inner-banner">

    </section>
    <nav aria-label="breadcrumb">
        <ol class="breadcrumb breadcrumb-padding">
           <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
            <li class="breadcrumb-item active" aria-current="page">Blog single post</li>
        </ol>
    </nav>
    <!-- blog single page breadcrumns -->
    
    <div class="display-ad" style="margin: 8px auto; display: block; text-align:center;">
    <!---728x90--->
    
    </div>
        
    <!-- single post -->
    <section class="text-11">
        <div class="text11">

                <div class="text-center" v-show='loading'>
                        <v-progress-circular
                          indeterminate
                          color="primary"
                        ></v-progress-circular>
                              </div>
              
                <div class="text-center" v-show='err'>
                        Network error. Please reload.
                      </div>
                      
            <div class="container">
                <div class="row">
                    <div class="col-lg-8 text11-content">
               <img :src="'https://henrymoby.website/storage/blog/pwa_1559904166.png'"
               class="img-fluid custom-height2" :alt="post.title" />
               <div class="blog-info">
                    <h3>
                      {{post.title}}
                  </h3>
                    <ul>
                     <li><span class="fa fa-calendar mr-2"></span>{{post.created_at}}</li>
                            </ul>
                        </div>

                        <p class="mt-4 mb-3 jumbotron" v-html='post.description'>
                    
                        </p>
                      
                      <!--  <h5 class="quote">Lorem faucibus ante vitae justo efficitur elementum. Donec ipsum faucibus arcu
                            elementum nec purus quis tempor.</h5>
                   -->
                      
                      <!--  <div class="new-posts clearfix">
                            <a class="prev-post pull-left" href="#prev"><span class="fa fa-angle-double-left"></span>
                                Previous
                                Post</a>
                            <a class="next-post pull-right" href="#next">Next Post <span
                                    class="fa fa-angle-double-right"></span></a>
                        </div>
                      -->


                      <!--  <div class="leave-comment-form" id="comment">
                            <h3 class="aside-title">Leave a reply</h3>
                            <form action="#" method="post">
                                <div class="input-grids">
                                    <div class="form-group">
                                        <input type="text" name="Name" class="form-control" placeholder="Your Name"
                                            required="">
                                    </div>
                                    <div class="form-group">
                                        <input type="email" name="Email" class="form-control" placeholder="Email"
                                            required="">
                                    </div>
                                    <div class="form-group">
                                        <textarea name="Comment" class="form-control" placeholder="Your Comment"
                                            required=""></textarea>
                                    </div>
                                </div>
                                <div class="submit text-right">
                                    <button class="btn btn-style btn-primary">Post Comment</button>
                                </div>
                            </form>
                        </div>
                        -->
                    </div>

                    <!--
                    <div class="sidebar-side col-lg-4 col-md-12 col-sm-12 mt-lg-0 mt-5">
                        <aside class="sidebar">

                          
    
                            <!-Blog Category Widget->
                            <div class="sidebar-widget sidebar-blog-category">
                                <div class="sidebar-title">
                                    <h4>Categories</h4>
                                </div>
                                <ul class="blog-cat">
                                    <li><a href="#url">Marketing process <span>1</span></a></li>
                                    <li><a href="#url">Business partnership <span>5</span></a></li>
                                    <li><a href="#url">Development <span>8</span></a></li>
                                </ul>
                            </div>
    
                         
    
                      
                            <!- Tags Widget--
                            <div class="sidebar-widget popular-tags">
                                <div class="sidebar-title">
                                    <h4>Tags</h4>
                                </div>
                                <a href="#url">Business</a>
                                <a href="#url">Cloud</a>
                                <a href="#url">Tax</a>
                                <a href="#url">Invest</a>
                                <a href="#url">Market</a>
                            </div>
    
                           
                        </aside>
                    </div>
                -->

                </div>
            </div>
        </div>
    </section>
    <!-- //single post -->
    
    <div class="display-ad" style="margin: 8px auto; display: block; text-align:center;">
    <!---728x90--->
    </div>
     
      
        </div>
        
        </template>
        
        <script>
      
        export default {
          
            head(){
            return {
            title: this.post.title,
            meta:[
                
                { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
                { name: 'keywords', content: 'digital marketing, seo, web development in lagos, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },
                
            ]
            }
        },
            data () {
                return {
                post:[],
                err: false,
                loading: true,
                }
              },
              
            methods:{

              //fetch post
              getPost(){
               // this.$nuxt.$loading.start()
             var  page = 'https://cohotekapi.getfoods.ng/api/posts/'+this.$route.params.id+'/'+this.$route.params.slug;
          
                    fetch(page, {
                    method: 'GET',
                    headers: {
                    'Content-Type': 'application/json',
                    'X-Authorization': 'w69D58JnTvtUCH3KHcfhSGNIO7NtLuJEAF7ixJDwSHCGiTpdLUWdhvROVWt8TaUf'
                    }
                    })
                    .then(res => res.json())
                    .then(res=>{
                      this.post = res.data;
                      console.log(this.post)
                      //  this.$nuxt.$loading.finish()
                      this.loading = false
                    })
                    .catch(error =>{
                        console.log(error)  
                  //  this.$nuxt.$loading.finish()
                  this.loading = false
                    this.err = true
                    })
                  },

            },

          mounted(){
            //collapse nav on component load
            $('#navbarNav').hide('fade');

            //get post
            this.getPost()
          },
          
         
        }
        </script>
        