<template>

        <div>
          
        
      
<!-- about page breadcrumns -->
<section class="inner-banner">

    </section>
    <nav aria-label="breadcrumb">
        <ol class="breadcrumb breadcrumb-padding">
                <li class="breadcrumb-item"><nuxt-link to="/">Home</nuxt-link></li>
            <li class="breadcrumb-item active" aria-current="page">Portfolio</li>
        </ol>
    </nav>
    <!-- //about page breadcrumns -->
    
    <!-- homepage blog grids -->
    <section id="blog">
        <div class="container">
            <div class="row align-items-center" >
                <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
                    <h4 class="section-title">Company Portfolio</h4>
                    <p class="text-center">
             Cohotek is changing the way, we work, live, play and learn by connecting businesses
                            with their IT needs.</p>
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
               

                <div class="col-lg-4 col-md-6 col-sm-12 mt-lg-0 mt-4 blog-grid" id="zoomIn"
                v-for='proj in projects' v-bind:key='proj.id'>

                    <a :href="proj.url" target='_blank'>
                        <figure><img src="@/assets/images/cohotek-it-company.png"
                             class="img-fluid custom-height" :alt="proj.name"></figure>
                    </a>
                    <div class="blog-info">
                        <h3><a :href="proj.url" target='_blank'>{{proj.name}}</a> </h3>
                        
                    </div>
                </div>

                
              

            </div>
            <nav aria-label="Page navigation example">
                    <ul class="pagination justify-content-center mt-5 mb-0">
                        <li class="page-item">
                   <button class='page-link'
                      @click.prevent="getProjects(pagination.prev_page_url)" :disabled="!pagination.prev_page_url">
                    Previous
                    </button>
                        </li>
                        <li class="page-item"><span class="page-link">{{pagination.current_page}}</span></li>
                        <li class="page-item active"><span class="page-link" >of</span></li>
                        <li class="page-item"><span class="page-link">{{pagination.last_page}}</span></li>
                        <li class="page-item">
                  <button class='page-link'
                   @click.prevent="getProjects(pagination.next_page_url)" :disabled="!pagination.next_page_url">
                     Next
                 </button>
                        </li>
                    </ul>
                </nav>
         
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
      title: "Web Development Portfolio",
      meta:[
        
          { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
          { name: 'keywords', content: 'digital marketing, seo, web development in lagos, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },
        
      ]
    }
  },

  data () {

return {
projects:[],
loading: true,
err: false,
pagination: [],
}

},

methods: {

getProjects(page_url){

    if(page_url){
     this.$nuxt.$loading.start()
    }
    var   page_url = page_url || 'https://cohotekapi.getfoods.ng/api/projects';

  fetch(page_url, {
  method: 'GET',
  headers: {
    'Content-Type': 'application/json',
    'X-Authorization': 'w69D58JnTvtUCH3KHcfhSGNIO7NtLuJEAF7ixJDwSHCGiTpdLUWdhvROVWt8TaUf'
  }
})
  .then(res => res.json())
  .then(res=>{
    this.projects = res.data;
    console.log(this.projects)
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
            this.getProjects()
          },
          
          components: {
          //  Logo,
          //  VuetifyLogo
          }
        }
        </script>
        