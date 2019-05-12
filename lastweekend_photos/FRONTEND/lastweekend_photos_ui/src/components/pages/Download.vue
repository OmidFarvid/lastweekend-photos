<style>
  .text-black {
    color: #000000;
  }


  .cover-row {
    position: absolute;
    width: 96%;
    z-index: 2;
    opacity: 0.8;
    color: #000000;
    background-color: #cccccc;
    bottom: 0px;
    margin-left: 10px;
    left: 0px;
  }

  .la {
    cursor: pointer;
  }

  .thumbnail {
    padding: 4px;
    line-height: 1.42857;
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 4px;
    -webkit-transition: border .2s ease-in-out;
    -o-transition: border .2s ease-in-out;
    transition: border .2s ease-in-out;
  }

  .image-size {
    border: 2px solid black;
    -webkit-box-shadow: 5px 5px 0px 0px rgba(0, 0, 0, 0.75);
    -moz-box-shadow: 5px 5px 0px 0px rgba(0, 0, 0, 0.75);
    box-shadow: 5px 5px 0px 0px rgba(0, 0, 0, 0.75);
    height: 50px;
    width: 50px;
    text-align: center;
    font-size: x-large;
    color: #000000;
    margin-right: 10px;
  }

  .image-size.active {
    background: rgba(71, 142, 222, 0.46);
  }
</style>
<template>
  <div class="container">
    <div class="row">
      <div class="col-md-6">
        <div class="row">
          <div class="thumbnail">
            <div class="col-12 image-box">
              <img src='resources/images/img2.jpg'
                   style="width: 100%;height: auto;">
              <span class="cover-row">man in laps</span>
            </div>

            <div class="row h4">
              <div class="col-md-1 offset-2 h3">
                <span class="la la-mail-forward"></span>
              </div>

              <div class="col-md-1 h3">
                <span class="la la-star-o"></span>
              </div>

              <div class="col-md-1 h3">
                <span class="la la-thumbs-o-up"></span>
              </div>

              <div class="col-md-2 text-center offset-2">
                <span class="la la-comment-o"></span>
                35
              </div>
              <div class="col-md-3 text-center">
                <span class="la la-heart-o"></span>
                443
              </div>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-2 text-center">
            <span class="la la-user h2"></span>
          </div>
          <div class="col-md-10">
            <div class="row">
              <div class="col-md-12 text-left h3 text-black">
                albert nic
              </div>
            </div>
            <div class="row">
              <div class="col-md-12 text-left h3">
                london
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="row">
          <div class="col-md-2 offset-3 image-size">S</div>
          <div class="col-md-2 image-size">M</div>
          <div class="col-md-2 image-size">L</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "Download"
  }
</script>

<style scoped>

</style>