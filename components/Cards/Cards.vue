<template>
  <div :class="$style.cards_main">
    <div :class="$style.cards_box">
      <img :class="$style.three_arrow" src="@/assets/imgs/icon.png">
      <div :class="$style.cards_image">
        <img src="@/assets/imgs/women.png">
      </div>
      <div :class="$style.year_text">
        2021
      </div>
      <div :class="$style.text">
        FREE TICKET EVENT
      </div>
    </div>
    <div :class="$style.cards_box">
      <img :class="$style.three_arrow2" src="@/assets/imgs/icon.png">
      <div :class="$style.cards_image">
        <img src="@/assets/imgs/men6.png">
      </div>
      <div :class="$style.text">
        <span>PARTY ROCK </span>FREE TICKET EVENT
      </div>
      <a href="#">
        RIGESTER
        <img src="@/assets/imgs/right_arrow_black.png">
      </a>
    </div>
    <div :class="[$style.cards_box , $style.box_3]">
      <div :class="$style.cycle" />
      <div :class="$style.cycle2" />
      <p>Upcoming Event <br><span>150+</span></p>
      <div :class="$style.btn">
        View More Event
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" module>

.cards_main{
    display: flex;
    justify-content: space-between;
    padding-bottom: 10%;
}

.cards_box{
    width: 30%;
    background: #fff;
    border-radius: 20px;
    position: relative;

    a{
      margin: 12% 14% 0;
      display: block;
      cursor: pointer;
      color: #000;
      transition: all 0.3s ease;
        &:hover{
          opacity: 0.7;
  }
  img{
    padding-left: 2%;
  }
}
}

.year_text{
position: relative;
color: #1b2635;
text-shadow: 8px 0px 2px #27ffe6;
font-size: 82px;
text-align: center;
font-family: Sanchez;
margin-top: 6%;
font-weight: 600;
letter-spacing: 4px;
z-index: 1;
}

.text{
  font-family: Corbel;
  font-size: 15px;
  text-align: center;
  margin-top: 18%;
  font-weight: 200;
  span{
  font-size: 69px;
font-weight: bold;
font-family: Corbel;
position: relative;
line-height: 0.8;
margin: -46.5% 15% 0;
display: block;
padding-bottom: 7%;
text-align: left;
  }
}

.box_3{
    background: #27ffe6;
    position: relative;
    overflow: hidden;
    p{
      position: relative;
    padding: 16% 12%;
      span{
        font-size: 70px;
        font-weight: bold;
      }
    }
}

.btn{
  position: relative;
background: #1d2635;
color: #27ffe6;
padding: 4%;
border-radius: 50px;
// margin: 29% 45% 10% 12%; --> asli
margin: 29% 35% 10% 12%;
cursor: pointer;
transition: all 0.3s ease;
text-align: center;
  &:hover{
    opacity: 0.9;
  }
}

.three_arrow{
position: absolute;
top: 13%;
left: -25%;
z-index: 1;
width: 48%;
}

.three_arrow2{
position: absolute;
bottom: 98%;
right: 4%;
width: 46%;
}

.cycle{
 position: absolute;
width: 45%;
height: 40%;
background: #28edd8;
border-radius: 50%;
opacity: 0.4;
top: 23%;
left: 51%;
}

.cycle2{
 position: absolute;
width: 80%;
height: 80%;
background: #28edd8;
border-radius: 50%;
opacity: 0.5;
top: 50%;
left: 34%;
}

.cards_image{
    position: relative;
    margin: -25% 12%;
    &:before{
        display: block;
        content: '';
        padding-bottom: 130%;
    }
    img{
        position: absolute;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        width: 100%;
    }
}
@media(max-width: 1215px){
  .year_text{
      font-size: 60px;

  }
    .text span{
  font-size: 56px;
}
}

@media(max-width: 1000px){
  .text span{
  font-size: 45px;
}

.btn{
  margin: 29% 20% 10% 12%;
}
}

@media(max-width: 800px){
  .cards_main{
    flex-direction: column;
  }

.cards_box{
width: 80%;
margin: 11% auto;
}

.cards_image{
width: 80%;
margin: -25% auto 0;
}
.year_text{
  font-size: 86px;
  margin-top: -19%;
}
.text{
padding-bottom: 10%;
margin-top: 6%;
span{
font-size: 70px;
margin: -28.5% 21% 0;
}
}

.three_arrow2{
  bottom: 68%;
}

.cards_box{
  a{
    margin: 7% 14% 10%;
  }
}
}

@media(max-width: 500px){
.year_text{
  font-size: 53px;
margin-top: -17%;
}

.text span{
  font-size: 45px;
}
}
</style>
