<template>
    <div class="slider_wrap">
<div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
  <ol class="carousel-indicators">
    <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="3"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="4"></li>
    <li data-target="#carouselExampleIndicators" data-slide-to="5"></li>
  </ol>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img class="d-block w-100" src="../assets/bba35b173b8225cda4d866f137586d9c66a538c8.png" alt="First slide">
        <div class="carousel-caption d-none d-md-block">
            <a href="#"><h5>Anselm Kiefer: Walhalla</h5></a>
            <p>Until 12 February 2017, London</p>
        </div>
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="https://miro.medium.com/max/1200/1*mk1-6aYaf_Bes1E3Imhc0A.jpeg" alt="Second slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="https://media.istockphoto.com/photos/woman-using-her-laptop-picture-id643897728?k=20&m=643897728&s=170667a&w=0&h=VR_wNxm1xT3y_45RJX8GRW7EQbOxu7l1unV2EzlKDb0=" alt="Third slide">
          <div class="carousel-caption d-none d-md-block">
            <a href="#"><h5>Anselm Kiefer: Walhalla</h5></a>
            <p>Until 12 February 2017, London</p>
        </div>
    </div>
    <div class="carousel-item ">
      <img class="d-block w-100" src="https://thumbs.dreamstime.com/b/alligator-apple-19928485.jpg" alt="First slide">
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="https://miro.medium.com/max/1200/1*mk1-6aYaf_Bes1E3Imhc0A.jpeg" alt="Second slide">
        <div class="carousel-caption d-none d-md-block">
            <a href="#"><h5>Anselm Kiefer: Walhalla</h5></a>
            <p>Until 12 February 2017, London</p>
        </div>
    </div>
    <div class="carousel-item">
      <img class="d-block w-100" src="https://media.istockphoto.com/photos/woman-using-her-laptop-picture-id643897728?k=20&m=643897728&s=170667a&w=0&h=VR_wNxm1xT3y_45RJX8GRW7EQbOxu7l1unV2EzlKDb0=" alt="Third slide">
    </div>
  </div>
  <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>
    <div class="slider_info">
        <a href="#"><p>Anselm Kiefer: Walhalla</p></a>
        <p>Until 12 February 2017, London</p>
    </div>
    </div>
    
</template>

<script>
export default {
    
}
</script>
<style scoped>

.slider_wrap{
    width: 100%;
    height: 602px;
   /*background-color: rebeccapurple;*/
    margin-top: 10px;
}
.slider_info a{
    text-decoration: none;
    color: #222222;
    font-family: "DINPro-Bold";
    font-size: 24px;
}
.slider_info p{
   font-family: "DINPro-Medium";
   font-size: 24px;
}
img.d-block.w-100 {
    height: 600px;
}
ol.carousel-indicators {
    height: 20px;
    z-index: 9999;
    right: 0px !important;
    width: 200px;
    position: absolute;
    left: 67%;
    bottom: -52px;
}
.carousel-indicators li{
    cursor: pointer;
    border-radius: 50%;
    height: 15px;
    width: 15px;
    margin-right: 8px;
    background-color: #B0B0B0;
}
.carousel-indicators li.active{
    background-color: #FF5C5C;
}
.slider_info {
    float: left;
    width: 100%;
    text-align: left;
    margin-top: 10px;
    font-size: 24px;
    letter-spacing: 0.05em;
}
.carousel-caption.d-none.d-md-block {
    float: left;
    text-align: left;
}
.carousel-caption.d-none.d-md-block a{
  font-family: "DINPro-Bold";
  color: #222222;
    text-decoration: none;
}
.carousel-caption.d-none.d-md-block p{
  font-family: "DINPro-Medium";
  color: #222222;
    text-decoration: none;
}
.carousel-caption{
  left:5% !important;
}
.slider_info p{
    margin-bottom: 5px;
}
@media (max-width: 768px) {
  img.d-block.w-100 {
    height: 200px;
}
.slider_wrap{
  height: 200px;
}
ol.carousel-indicators[data-v-2dedc691]{
  display: none !important;
}
}
</style>