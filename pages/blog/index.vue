<template>

        <div>
          
        
      
<!-- blog page breadcrumns -->
<section class="inner-banner">

    </section>
    <nav aria-label="breadcrumb">
        <ol class="breadcrumb breadcrumb-padding">
                <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
            <li class="breadcrumb-item active" aria-current="page">Blog</li>
        </ol>
    </nav>
    <!-- blog page breadcrumns -->
    
    <div class="display-ad" style="margin: 8px auto; display: block; text-align:center;">
    <!---728x90--->
    
    </div>
        
    <!-- blog page blog grids -->
    <section id="blog">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
                    <h4 class="section-title">Latest Blog Posts</h4>
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

            <div class="blog-grids row mt-md-5 mt-4">
                <div class="col-lg-4 col-md-6 col-sm-12 blog-grid" id="zoomIn"
                v-for='post in posts' v-bind:key='post.id'
                >
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
            <nav aria-label="Page navigation example">
                    <ul class="pagination justify-content-center mt-5 mb-0">
                        <li class="page-item">
                   <button class='page-link'
                      @click.prevent="getPosts(pagination.prev_page_url)" :disabled="!pagination.prev_page_url">
                    Previous
                    </button>
                        </li>
                        <li class="page-item"><span class="page-link">{{pagination.current_page}}</span></li>
                        <li class="page-item active"><span class="page-link" >of</span></li>
                        <li class="page-item"><span class="page-link">{{pagination.last_page}}</span></li>
                        <li class="page-item">
                  <button class='page-link'
                   @click.prevent="getPosts(pagination.next_page_url)" :disabled="!pagination.next_page_url">
                     Next
                 </button>
                        </li>
                    </ul>
                </nav>
        </div>
    </section>
    <!-- blog page blog grids -->
    
    <div class="display-ad" style="margin: 8px auto; display: block; text-align:center;">
    <!---728x90--->
    </div>
     
      
        </div>
        
        </template>
        
        <script>
     
        
        export default {
          
            head(){
        return {
        title: "IT Comapny Blog in Lagos",
        meta:[
            
            { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
            { name: 'keywords', content: 'digital marketing, seo, web development in lagos, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },
            
        ]
        }
        },

        data () {

        return {
        posts:[],
        loading: true,
        err: false,
        pagination: [],
        }

        },

        methods:{

  getPosts(page_url){

if(page_url){
 this.$nuxt.$loading.start()
}
var   page_url = page_url || 'https://cohotekapi.getfoods.ng/api/posts';

fetch(page_url, {
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
this.$nuxt.$loading.finish()
this.makePagination(res.meta, res.links);
})
.catch(error =>{
console.log(error)  
this.loading = false    
this.$nuxt.$loading.finish()
this.err = true
  })
},
//method end

makePagination(meta, links){
        var pagination = {
                        current_page: meta.current_page,
                        last_page: meta.last_page,
                        next_page_url: links.next,
                        prev_page_url: links.prev
                         }
           document.body.scrollTop = 0;
            document.documentElement.scrollTop = 0;
        this.pagination = pagination;
            },

        },

          mounted(){
            //collapse nav on component load
            $('#navbarNav').hide('fade');

             //get projects
             this.getPosts()
          },
          
          components: {
          //  Logo,
          //  VuetifyLogo
          }
        }
        </script>
        