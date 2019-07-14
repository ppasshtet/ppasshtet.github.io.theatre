<template>
  <div class="about">
    <div class="linebase">
          </div>
        <div class="container">
          <div class="row">
            <div class="mainName">
              {{MainNameAbout}}
            </div>
          </div>
          <div class="Content-1">
          <div class="row">
              <div class="col-xl-6">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea, enim rerum obcaecati neque deleniti sed tempore voluptas dolores adipisci quod eum architecto officiis totam placeat autem eaque. Pariatur, at natus?
              </div>
              <div class="col-xl-6">
                <img src="../assets/image.png" alt="">
              </div>
          </div>
          </div>
              <hr/>
              <div class="Content-2">
          <div class="row">
              <div class="col-xl-6">
                <img src="../assets/image.png" alt="">
              </div>
              <div class="col-xl-6">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea, enim rerum obcaecati neque deleniti sed tempore voluptas dolores adipisci quod eum architecto officiis totam placeat autem eaque. Pariatur, at natus?
              </div>
          </div>
          </div>
          <hr/>
          <div class="Content-3">
          <div class="row">
              <div class="col-xl-6">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea, enim rerum obcaecati neque deleniti sed tempore voluptas dolores adipisci quod eum architecto officiis totam placeat autem eaque. Pariatur, at natus?
              </div>
              <div class="col-xl-6">
                <img src="../assets/image.png" alt="">
              </div>
          </div>
          </div>
          </div>
              
            <div class="linebottom">

            </div>

        </div>
</template>


<script>
// @ is an alias to /src
import {mapState} from '@/store.js'
export default {
  name: 'home',
  data:{
  },
  computed:{
    MainNameAbout () {
      return this.$store.state.MainNameAbout
    },

  },
  components: {
    
}
}
</script>
<style>
.about{
  background: #E5E5E5;
}
.linebase{
  position: absolute;
  height: 20px;
  width: 100%;
  left: 0;
  margin-top: 100px;
  transform: matrix(1, 0, 0, -1, 0, 0);
   background: url(../assets/image2.jpg); 
}
@font-face {
  font-family: a_AntiqueGr;
  src: url(../assets/type/2285.ttf);
}
.mainName{
  position: absolute;
width: 1440px;
height: 44px;
left: 0px;
top: 149px;

font-family: a_AntiqueGr;
font-size: 48px;
line-height: 60px;
text-align: center;
}
.Content-1{
  margin-top: 259px;
}
.Content-2, .Content-3{
  margin-top: 20px;
}
hr{
  background: #A9A9A9;
  margin-top: 20px;
}
.Content-3{
  margin-bottom: 20px;
}
.linebottom{
position: absolute;
width: 100%;
height: 20px;
left: 0px;
margin-bottom: 0px;
background: url(../assets/image2.jpg)
}
</style>

