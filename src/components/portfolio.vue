<template>
  <div id="port">
        <div class="container">
      <div class="row">
        <div class="col-lg-12 text-center">
          <h2 class="section-heading text-uppercase">Portfolio</h2>
          <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
        </div>
      </div>
      <div class="row">
        <div v-for="(obj, key) in jsonw" :key="key" class="col-md-4 col-sm-6 portfolio-item"  >
          <a class="portfolio-link" data-toggle="modal" href="#portfolioModal1">
            <div class="portfolio-hover">
              <div class="portfolio-hover-content">
                <i class="fas fa-plus fa-3x"></i>
              </div>
            </div>
            <img  v-bind:src="obj.image"  alt="">
          </a>
          <div class="portfolio-caption">
            <h4>{{obj.name}}</h4>
            <p class="text-muted">{{obj.title}}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    jsonw: [
      {
      name: 'Threads',
      title: 'Illustration',
      image: 'assets/img/portfolio/01-thumbnail.jpg'
    },
     {
      name: 'come',
      title: 'Website Design',
      image: 'img/portfolio/05-thumbnail.jpg'
    },
     {
      name: 'Window',
      title: 'Photography',
      image: 'img/portfolio/06-thumbnail.jpg'
    },
    {
      name: '2009-2011',
      title: 'Our Humble Beginning',
      image: 'hdhdhdhdhdhd'
    },
     {
      name: 'come',
      title: 'Website Design',
      image: 'img/portfolio/05-thumbnail.jpg'
    },
     {
      name: 'Window',
      title: 'Photography',
      image: 'img/portfolio/06-thumbnail.jpg'
    }

  ]
  })
 

}
</script>
