<template>
  <div id="app">
    
    <div class="wrapper">
      <div class="blue">
      <b-row>
        <b-col>
        <router-link to="/Profile"><svg width= "60px" height="60px" class="circle" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 496 512"> <path d="M248 104c-53 0-96 43-96 96s43 96 96 96 96-43 96-96-43-96-96-96zm0 144c-26.5 0-48-21.5-48-48s21.5-48 48-48 48 21.5 48 48-21.5 48-48 48zm0-240C111 8 0 119 0 256s111 248 248 248 248-111 248-248S385 8 248 8zm0 448c-49.7 0-95.1-18.3-130.1-48.4 14.9-23 40.4-38.6 69.6-39.5 20.8 6.4 40.6 9.6 60.5 9.6s39.7-3.1 60.5-9.6c29.2 1 54.7 16.5 69.6 39.5-35 30.1-80.4 48.4-130.1 48.4zm162.7-84.1c-24.4-31.4-62.1-51.9-105.1-51.9-10.2 0-26 9.6-57.6 9.6-31.5 0-47.4-9.6-57.6-9.6-42.9 0-80.6 20.5-105.1 51.9C61.9 339.2 48 299.2 48 256c0-110.3 89.7-200 200-200s200 89.7 200 200c0 43.2-13.9 83.2-37.3 115.9z"/></svg></router-link>
        </b-col>
        <b-col>
        <div class="title">NYSL</div>
        </b-col>
      </b-row>
      </div>

      <div class="main-view">
        <router-view/>
      </div>
      
    </div>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@1,200&display=swap');



#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  height: 100vh;
}

.main-view{
  position: relative;
  z-index: 998;
  width: 100%;
  height: 80vh;
  text-align: center;
  margin-top: 10vh;
  max-height: 100vh;
  max-width: 100vw;
}

.wrapper{
  width: 100%;
  height: 70vh;
  display: row;

  div{
    height: 90%;

    &.blue {
    background: #b0c8f3;
    background-image: linear-gradient(150deg, #b0c8f3 0, #b0c8f3 281px, #ddd 282px, #b0c8f3 283px, #b0c8f3 566px);
    width: 100%;
    height: 22%;
    border-bottom: 7px solid #CEEDC7;
    
    .circle{
      position: relative;
      height: 100%;
      margin: 1em;
      color: #CEEDC7;
      }
    .title{
      font-size: 90px;
      color:  #CEEDC7;
      font-weight: 900;
      font-family: 'Poppins';
      left: 0px;
      -webkit-text-fill-color: transparent;
      -webkit-text-stroke-width: 1px;
      -webkit-text-stroke-color: #CEEDC7;
      font-style: italic;
      }
    }
  }

  .bottom-bar{
    text-align: center;
    height: 12%;
    margin-bottom: 0px;
  }
  .carousel-control-next-icon{
    background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='%23000' viewBox='0 0 8 8'%3E%3Cpath d='M2.75 0l-1.5 1.5 2.5 2.5-2.5 2.5 1.5 1.5 4-4-4-4z'/%3E%3C/svg%3E");
 }

   .carousel-control-prev-icon{
    background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' fill='%23000' viewBox='0 0 8 8'%3E%3Cpath d='M5.25 0l-4 4 4 4 1.5-1.5-2.5-2.5 2.5-2.5-1.5-1.5z'/%3E%3C/svg%3E") !important;
 }
}
</style>