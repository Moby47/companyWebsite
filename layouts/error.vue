<template>
 

    <div>
      
        <!-- about page breadcrumns -->
        <section class="inner-banner">
        
        </section>
       
      
        <!-- about page team section -->
        <section class="w3l-team-main-6">
            <!-- /team-grids -->
            <div class="team-content">
                <div class="container">
                    <div class="row align-items-center">
                        <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">
                            <h4 class="section-title" v-if="error.statusCode === 404">
                                {{ pageNotFound }}</h4>
                            <p class="text-center" v-else>
                                {{ otherError }} <br>
                                <a href='/'>Home</a>
                              </p>
                        </div>
                    </div>
                 
                </div>
            </div>
            <!-- /team-grids -->
        </section>
        <!-- //about page team section -->
        
      
       
        
          </div>
          

</template>

<script>
export default {

  head(){
    return {
      title: "",
      meta:[
        
          { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
          { name: 'keywords', content: 'digital marketing, seo, web development in lagos, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },
        
      ]
    }
  },

  layout: 'empty',
  props: {
    error: {
      type: Object,
      default: null
    }
  },
  data () {
    return {
      pageNotFound: '404! This Page Was Not Found',
      otherError: 'An error occurred, please try another page'
    }
  },
  head () {
    const title =
      this.error.statusCode === 404 ? this.pageNotFound : this.otherError
    return {
      title
    }
  }
}
</script>

<style scoped>
h1 {
  font-size: 20px;
}
</style>
