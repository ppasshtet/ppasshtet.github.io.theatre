<template>
    <div class="contact">
         <div class="lineBase">
          </div>
          
            <div class="container">
                <div class="boxNameContact">
                        <div class="row">
                            <div class="col-xl">
                                <div class="MainName">
                                    Автономная некоммерческая организация социально-культурных программ и проектов
                                </div>
                            </div>
                        </div>
                    <div class="blockContact">
                    <div class="row">
                        <div class="col-xl-6">
                            <div id="contact-1">

                            </div>
                        </div>
                        <div class="col-xl-6">
                             <div id="contact-2">
                                 
                             </div>
                        </div>
                    </div>
                </div>
                </div>
            </div>

                
            <div class="ContactName">
                {{MainNameContact}}
                <div class="position">
                {{positionContact}}
                </div>
              
            </div>
            <div class="container">
                <div class="boxPhoneEmail">
                    <div class="row">
                        <div class="col-xl-6">
                            <div class="Phone">
                                <div class="phoneNum">
                                    Тел: {{phone}}
                                </div>
                            </div>
                        </div>
                        <div class="col-xl-6">
                            <div class="E-mail">
                                <div class="nameMail">
                                     {{Mail}}
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="linebottom">

            </div>
            </div>
</template>

<script>
import {mapState} from '@/store.js'
export default {
    computed:{
    phone () {
      return this.$store.state.phone
    },
    Mail () {
        return this.$store.state.Mail
    },
    MainNameContact () {
        return this.$store.state.MainNameContact
    },
    positionContact () {
        return this.$store.state.positionContact
    },
},
}
</script>


<style>

.lineBase{
  height: 20px;
  width: 100%;
  left: 0;
  margin-top: 100px;
    background: url(../assets/image22.png); 
}
.boxNameContact{
    top: 38px;
    height: 412px;
    /* background: #000; */
    margin-top: 38px;
}
@font-face {
  font-family: a_AntiqueGr;
  src: url(../assets/type/2285.ttf);
}
.MainName{
font-family: a_AntiqueGr;
font-size: 48px;
line-height: 60px;
display: flex;
align-items: center;
text-align: center;
padding-top: 20px;
}
#contact-1, #contact-2{
width: 310px;
height: 210px;
margin-top: 50px;
background: #FFFFFF;
/* Темно-Серый */

border: 1px solid #A9A9A9;
box-sizing: border-box;
border-radius: 8px;
}
#contact-1{
    margin-left: 210px;
}
.ContactName{
    margin-top: 50px;
    width: 100%;
    height: 174px;
    background: url(../assets/image22.png);

font-family: a_AntiqueGr;
font-size: 36px;
line-height: 45px;
padding-top: 42px;
color: #FFFFFF;

}
.boxPhoneEmail{
    margin-top: 30px;
    /* background: red; */
    height: 46px;
    margin-bottom: 20px;
}
.Phone{
width: 300px;
height: 46px;
margin-left: 0px;
background: #FFFFFF;
display: flex;
align-items: center;
justify-content: center;
/* Темно-Серый */

border: 1px solid #A9A9A9;
box-sizing: border-box;
border-radius: 8px;
font-family: Times New Roman;
font-size: 24px;
line-height: 28px;

}
.E-mail{
width: 468px;
height: 46px;
margin-left: 71.5px;
background: #FFFFFF;
font-family: Times New Roman;
font-size: 24px;
line-height: 28px;
/* Темно-Серый */

border: 1px solid #A9A9A9;
box-sizing: border-box;
border-radius: 8px;
display: flex;
align-items: center;
justify-content: center;
}
.nameMail{
    display: flex;
    align-items: center;
    justify-content: center;
}
.phoneNum{
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>

