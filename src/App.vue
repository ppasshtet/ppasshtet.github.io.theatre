<template>
  <div id="app">
    <div id="nav">
      <div id="boxlogo">
        <div id="navLogo">
          Открой мир
       <div class="mainLine"></div>
        Открытый мир
        </div>
      </div>
      <div id="boxnav">
        <router-link  to="/">Главная</router-link> 
        <router-link to="/activity">Мероприятия</router-link> 
        <router-link to = "/about">О нас</router-link> 
        <router-link to = "/contact">Контакты</router-link> 
        <router-link to = "/news">Мы в сми</router-link> 
      </div>
      <div id="boximg">
        <img src="../src/assets/111.svg" alt="">
      </div>
    </div>
    
    <div id="nav1">
      <div class="container">
        <div class="row">
      <div class="col">
        <div id="positionNavText">
        Открой мир
       <div class="mainLine"></div>
        Открытый мир
        </div>
       
      </div>
      </div>
      <div class="row">
          <div class="col">
            <div class="line">
            </div>
          </div>
      </div>

    </div>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  text-align: center;
}
@media (min-width: 800px) and (max-width: 1980px) {
  #boximg{
    width: 384px;
    height: 100%;
    margin-left: 74.7%;
    margin-top: -100px;
  }
  #boxlogo{
    width: 201px;
    height: 100%;
      #navLogo{
            font-family: Montserrat;
            font-style: normal;
                font-weight: 800;
                font-size: 18px;
                padding-top: 25px;
                  .mainLine{
                    background:  #323232;
                    width: 121px;
                    height: 4px;
                    margin-left: 40px;
                    top: 45px;
                  }
      }
      
  }
  #nav1{
    display: none;
  }
  #nav {
position: absolute;
width: 100%;
height: 100px;
top: 0px;
left: 0px;
background: #F8F8F8;
z-index: 0;
  #boxnav{
    margin-left: 201px;
    width: 583.63px;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: -100px;
    z-index: 1;
    font-family: a_AntiqueGr;
font-size: 22px;
line-height: 27px;
  }
}
}

@media screen and (max-width: 320px) {
  #nav{
      display: none;
  }
  #nav1{
    background: #fff;
    height: 93px;
      #positionNavText{
        font-family: Montserrat;
        font-style: normal;
        font-weight: 800;
        font-size: 18px;
        margin-top: 30px;
        

          .mainLine{
            background:  #323232;
            width: 121px;
            height: 4px;
            margin-left: 83px;
            top: 45px;
          }
      }
  }
  .line{
  position: absolute;
width: 290px;
height: 1px;
left: 15px;
top: 18px;
opacity: 1;
background: #323232;
  }
}


</style>


