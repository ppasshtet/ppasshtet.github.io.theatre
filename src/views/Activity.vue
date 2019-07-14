<template>
    <div class="activity">
         <div class="lineBone">

            </div>
        <div class="container">
            <div class="box">
            <div class="row">
                Тип мероприятия:
                <button class="all">
                    Все
                </button>
                <button class="SoActivity">
                    Социальные мероприятия
                </button>
                <button class="Patriot">
                    Патриотическое воспитание
                </button>
                <button class="Street">
                    Уличные мероприятия
                </button>
                <button class="tales">
                    Сказки
                </button>
            </div>
        </div>
        <div class="box-1">
        <div class="row">
            <div class="col-xl-4">
                <router-link to="/description">
                <div class="card-1">
                    
                </div>
                </router-link>
            </div>
            <div class="col-xl-4">
                <div class="card-2">

                </div>
            </div>
            <div class="col-xl-4">
                <div class="card-3">

                </div>
            </div>
        </div>
</div>
<div class="box-1">
        <div class="row">
            <div class="col-xl-4">
                <div class="card-1">

                </div>
            </div>
            <div class="col-xl-4">
                <div class="card-2">

                </div>
            </div>
            <div class="col-xl-4">
                <div class="card-3">

                </div>
            </div>
        </div>
</div>
<div class="box-1">
        <div class="row">
            <div class="col-xl-4">
                <div class="card-1">

                </div>
            </div>
            <div class="col-xl-4">
                <div class="card-2">

                </div>
            </div>
            <div class="col-xl-4">
                <div class="card-3">

                </div>
            </div>
        </div>
</div>
        </div>
        <div class="linebottom"></div>


        <router-view></router-view>    
        </div>
</template>


<script>
export default {
    
}
</script>


<style>
@media (min-width: 800px) and (max-width: 1980px){
.box-1{
    margin-top: 41px;
}
.card-1, .card-2, .card-3{
width: 320px;
height: 180px;
background: url(../assets/image.png);
filter: blur(2px) opacity(100%);
box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.5);
backdrop-filter: blur(5px);
/* Note: backdrop-filter has minimal browser support */

border-radius: 8px;
}
.lineBone{
left: 0;
width: 100%;
height: 20px;
margin-top: 100px;
background: #E6D690;
transform: matrix(1, 0, 0, -1, 0, 0)
}
.box{
    margin-top: 27px;
}
.all{
    margin-left: 28px;
    background: url(../assets/image2.jpg)
}
.SoActivity{
    margin-left: 20px;
    background: #F28E13;
    border-radius: 4px;
}
.SoActivity:active,  button:active, button:focus{
box-shadow: inset 0px 4px 4px rgba(0, 0, 0, 0.35);
border-radius: 4px;
outline: none !important;
}
.Patriot{
    margin-left: 20px;
   background: #ED2424;
border-radius: 4px;

}
.Street{
    margin-left: 20px;
     background: #049DD9;
    border-radius: 4px;
}
.tales{
    margin-left: 20px;
    background: #E6D690;
    border-radius: 4px;
}
}
</style>
