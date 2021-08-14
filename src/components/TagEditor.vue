<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="First slide"
        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
        img-src="@/assets/Port_2_Background.jpg"
      ></b-carousel-slide>


      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <template #img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="480"
            src="https://picsum.photos/1024/480/?image=55"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>
    </b-carousel>

    <b-container>
      <b-col>

        <img src="@/assets/Layer 1.png" />
      </b-col>

      <b-col>
        hhh
        <img src="@/assets/blue-watercolor-texture-with-copyspace-right.jpg" />

      </b-col>
    </b-container>

    <b-container fluid class="counters">
      <b-row>
        <b-col class="counter" data-count="150">{{ count }}</b-col>
        <b-col class="counter" data-count="150">{{ count }}</b-col>
        <b-col class="counter" data-count="150">{{ count }}</b-col>
      </b-row>
    </b-container>

    <b-container>
      <b-row>
        <b-col class="portfolio-box shadow">
          <b-card
            class="border-0"
            overlay
            img-src="https://img.demo.persina.com/unsafe/720x720/https://static.demo.persina.com/Products/Image/4583cdf554e1427c9b68f31513128765.jpg"
            img-alt="Card Image"
            text-variant="white"
          >
          </b-card>

          <div class="portfolio-info">
            <h4>project name goes here 6</h4>
            <p>category project</p>
          </div>
        </b-col>
        <b-col class="portfolio-box shadow">
          <b-card
            class="border-0"
            overlay
            img-src="https://img.demo.persina.com/unsafe/720x720/https://static.demo.persina.com/Products/Image/4583cdf554e1427c9b68f31513128765.jpg"
            img-alt="Card Image"
            text-variant="white"
          >
          </b-card>

          <div class="portfolio-info">
            <h4>project name goes here 6</h4>
            <p>category project</p>
          </div>
        </b-col>
        <b-col class="portfolio-box shadow">
          <b-card
            class="border-0"
            overlay
            img-src="https://img.demo.persina.com/unsafe/720x720/https://static.demo.persina.com/Products/Image/4583cdf554e1427c9b68f31513128765.jpg"
            img-alt="Card Image"
            text-variant="white"
          >
          </b-card>

          <div class="portfolio-info">
            <h4>project name goes here 6</h4>
            <p>category project</p>
          </div>
        </b-col>
        <b-col class="portfolio-box shadow">
          <b-card
            class="border-0"
            overlay
            img-src="https://img.demo.persina.com/unsafe/720x720/https://static.demo.persina.com/Products/Image/4583cdf554e1427c9b68f31513128765.jpg"
            img-alt="Card Image"
            text-variant="white"
          >
          </b-card>

          <div class="portfolio-info">
            <h4>project name goes here 6</h4>
            <p>category project</p>
          </div>
        </b-col>
      </b-row>
    </b-container>
    {{ counter}}

    <b-container>
      <b-row>
        <b-col>
          <b-card border-variant="info" header="Info" align="center">
            <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</b-card-text>
          </b-card>
        </b-col>

        <b-col>
          <b-card border-variant="info" header="Info" align="center">
            <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</b-card-text>
          </b-card>
        </b-col>

        <b-col>
          <b-card border-variant="info" header="Info" align="center">
            <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</b-card-text>
          </b-card>
        </b-col>

        <b-col>
          <b-card border-variant="info" header="Info" align="center">
            <img src="@/assets/photo-camera.png" alt="">
            <b-card-text>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</b-card-text>
          </b-card>
        </b-col>
      </b-row>
    </b-container>

    <div class="container">
        <div class="row">

            <div id="carousel-example-generic" class="carousel slide carousel-fade carousel-animate carousel-bg" data-ride="carousel">
                <!-- Indicators -->
                <ol class="carousel-indicators">
                    <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
                    <li data-target="#carousel-example-generic" data-slide-to="1"></li>
                    <li data-target="#carousel-example-generic" data-slide-to="2"></li>
                </ol>
                <!-- Wrapper for slides -->
                <div class="carousel-inner" role="listbox">
                    <div class="item active" style="background-image: url(https://unsplash.it/1240/530?image=697);">
                        <div class="carousel-caption">
                           <div class="hero">
                                <hgroup class="zoomInDown animated">
                                    <h1 class="fadeInLeft animated">One</h1>
                                    <h3 class="slideInRight animated">Get start your next awesome project</h3>
                                </hgroup>
                                <button class="btn btn-hero btn-lg bounceInUp animated" role="button">See all features</button>
                            </div>
                        </div>
                    </div>
                    <div class="item" style="background-image: url(https://unsplash.it/1240/530?image=545);">
                        <div class="carousel-caption">
                            <div class="hero fadeInUp animated">
                                <hgroup>
                                    <h1>Two</h1>
                                    <h3>Get start your next awesome project</h3>
                                </hgroup>
                                <button class="btn btn-hero btn-lg zoomIn animated" role="button">See all features</button>
                            </div>
                        </div>
                    </div>
                    <div class="item" style="background-image: url(https://unsplash.it/1240/530?image=673);">
                        <div class="carousel-caption">
                            <div class="hero rollIn animated">
                                <hgroup class="rotateInDownRight animated">
                                    <h1>Three</h1>
                                    <h3>Get start your next awesome project</h3>
                                </hgroup>
                                <button class="btn btn-hero btn-lg" role="button">See all features</button>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Controls -->
                <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev">
                    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
                    <span class="sr-only">Previous</span>
                </a>
                <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next">
                    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
                    <span class="sr-only">Next</span>
                </a>
            </div>

            <section class="details">
                <h1>Animation in Bootstrap Slider</h1>
                <br>
            </section>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      counter: 8,
      sett:'',
    }
  },
// methods: {
//     todo: function() {
//       console.log(this.counter);
//       var self = this;
//       self.sett = setInterval(function() {
//         self.counter += 1;
//       }, 200);
//     },
//   },
//   mounted() {
//     this.todo();
//     setTimeout(function() {
//         clearInterval(self.sett);
//       }, 3000);
//   }
}
</script>

<style>
body {
  background-color: #ebecec!important;
}
.portfolio-box {
  position: relative;
  width: 100%;
  height: 18.5rem;
  overflow: hidden;
}

.portfolio-box img {
  width: 100%;
  height: 100%;
}

.portfolio-box .portfolio-info{
  background-color: linear-gradient(45deg, rgba(71,201,229,0.9) 0%, rgba(102,252,233,0.9) 100%);
  opacity: 0;
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  text-align: center;
  z-index: 3;
  transition: all ease-in-out 0.3s;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: white;
}

.portfolio-box:hover img {
  transform: scale(1.5);
  transition-duration: 2s;
  transition-property: all;
}

.portfolio-box:hover .portfolio-info {
  opacity: 0.9;
  transition-duration: 1s;
  transition-property: all;
}


.portfolio-box .portfolio-info::after {
    display: block;
    content: "";
    width: 48px;
    height: 48px;
    position: absolute;
    bottom: 35px;
    right: 35px;
    border-bottom: 3px solid #d7dce1;
    border-right: 3px solid #d7dce1;
    transition: all 0.5s ease 0s;
    z-index: 9994;
}


.portfolio-box .portfolio-info::before {
    display: block;
    content: "";
    width: 48px;
    height: 48px;
    position: absolute;
    top: 35px;
    left: 35px;
    border-top: 3px solid #d7dce1;
    border-left: 3px solid #d7dce1;
    transition: all 0.5s ease 0s;
    z-index: 9994;
}
/* counter */
.counters {
  background-color: #000;
  color:#fff;
  margin: 100px auto 0;
  text-align: center;
  display: table;
}

.counter {
  display: table-cell;
  margin:1.5%;
  font-size:50px;
  background-color: grey;
  width:200px;
  border-radius: 50%;
  height:200px;
  vertical-align: middle;
}
/*
Animate Bootstrap Carousel
Element by thecodeblock.com
*/
/********************************/
/*       Coloring indicators    */
/********************************/
.carousel-animate .carousel-indicators > li {
  margin: 0 2px;
  background-color: #f39c12;
  border-color: #f39c12;
  opacity: 0.7;
}
.carousel-animate .carousel-indicators > li.active {
  width: 10px;
  height: 10px;
  opacity: 1;
}
/********************************/
/*          Hero Headers        */
/********************************/
.carousel-animate .hero {
  color: #fff;
  text-align: center;
  text-transform: uppercase;
  text-shadow: 1px 1px 0 rgba(0, 0, 0, 0.75);
}
/********************************/
/*          Custom Buttons      */
/********************************/
.btn.btn-lg {
  padding: 10px 40px;
}
.btn.btn-hero,
.btn.btn-hero:hover,
.btn.btn-hero:focus {
  color: #f5f5f5;
  background-color: #1abc9c;
  border-color: #1abc9c;
  outline: none;
  margin: 20px auto;
}
/********************************/
/*          Media Queries       */
/********************************/
@media screen and (max-width: 640px) {
  .hero h1 {
    font-size: 2em;
  }
}
/********************************/
/*          Fade Effect         */
/********************************/
.carousel-fade .carousel-inner .item {
  transition-property: opacity;
}
.carousel-fade .carousel-inner .item,
.carousel-fade .carousel-inner .active.left,
.carousel-fade .carousel-inner .active.right {
  opacity: 0;
}
.carousel-fade .carousel-inner .active,
.carousel-fade .carousel-inner .next.left,
.carousel-fade .carousel-inner .prev.right {
  opacity: 1;
}
.carousel-fade .carousel-inner .next,
.carousel-fade .carousel-inner .prev,
.carousel-fade .carousel-inner .active.left,
.carousel-fade .carousel-inner .active.right {
  left: 0;
  transform: translate3d(0, 0, 0);
}
/************************************/
/*       BS bacground Images       */
/**********************************/
.carousel-bg .carousel-inner .item {
  background-color: darkslategrey;
  background-size: cover;
  background-position: center;
  min-height: 480px;
}

</style>