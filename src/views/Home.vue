<template>
    <div id="home">
       <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="0"
      controls
      indicators
      background="#fff"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #333;"
      data-touch="false"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
    
      <b-carousel-slide>
        <h1>WELCOME,</h1>
        <p class="desc">North Central American Youth Soccer League is a Youth, Female and Men soccer league that has dedicated it self and it’s members to promote and improve soccer for everyone in the city of Los Angeles and it’s surrounding communities. </p>
      </b-carousel-slide>


      <b-carousel-slide>
        <h1>UPCOMING EVENTS</h1>
        <p class="desc">Every match is on saturdays. Tap on the buttom below and find out all the information about the full schedule of our multiple teams. </p>
        
        <router-link to="/Schedule">
          <b-icon icon="plus-circle-fill" class="circulito" animation="throb"></b-icon>
        </router-link>
      </b-carousel-slide>
      
      <b-carousel-slide>
        <h1 class="message">CONTACT</h1>
        <p class="desc">
        Los Angeles, CA. 90037
        <br>Phone: 323-233-9850
        <br>Email: nyslcontact@nysl.com</p>
      </b-carousel-slide>

      


    </b-carousel>

    </div>
</template>

<script>

export default {
    name: 'home',
    }

</script>
 
 <style>


h1{
  font-family: arial black;
  font-weight: bold;
  color: #000;
  text-align: right;
}


p.desc{
  font-family: Sans-Serif;
  position: relative;
  font-size: 15px;
  margin: 1em;
  margin-top: 0;
  color: black;
  text-align: right;
}

.circulito{
  color: #b0c8f3;
  font-size: 4rem;
}

.div{
  height: 100%;
}

 </style>