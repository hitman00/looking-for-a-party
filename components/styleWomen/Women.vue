<template>
  <div :class="$style.main">
    <div :class="$style.boxs">
      <div :class="$style.image">
        <img src="@/assets/imgs/women.png">
      </div>
      <img :class="$style.year" src="@/assets/imgs/20214.png">
      <div :class="$style.text">
        FREE TICKET EVENT
      </div>
    </div>
    <div :class="$style.boxs">
      <div :class="$style.image">
        <img src="@/assets/imgs/men6.png">
      </div>
      <div :class="$style.text2">
        PARTY ROCK <span>FREE TICKET EVENT</span>
      </div>
      <a href="#">
        RIGESTER
      </a>
    </div>
    <div :class="[$style.boxs , $style.bc]">
      <div :class="$style.cycle" />
      <div :class="$style.cycle2" />
      <p>Upcoming Event <br><span>150+</span></p>
      <div :class="$style.bct">
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
.main{
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding-bottom: 10%;
}

.boxs{
    width: 30%;
    background: #fff;
    border-radius: 20px;

    a{
      margin: 35% 14% 0;
      display: block;
      cursor: pointer;
      color: #000;
      transition: all 0.3s ease;
        &:hover{
          opacity: 0.7;
  }
}
}

.year{
 position: relative;
 margin: -14% auto;
 display: block;
 width: 55.5%;
}

.text{
  font-family: Corbel;
  font-size: 15px;
  text-align: center;
  margin-top: 18%;
  font-weight: 200;
}

.text2{
font-size: 69px;
font-weight: bold;
font-family: Corbel;
position: relative;
line-height: 0.8;
margin: -28.5% 15%;
    span{
        font-size: 15px;
        font-weight: 200;
        display: block;
        line-height: 3;
    }
}

.bc{
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

.bct{
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

.image{
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

@media(max-width: 1000px){
  .text2{
  font-size: 45px;
}
.bct{
  margin: 29% 20% 10% 12%;
}
}

@media(max-width: 800px){
  .main{
    flex-direction: column;
  }
.boxs{
width: 80%;
margin: 11% auto;
}

.image{
width: 80%;
margin: -25% auto 0;
}
.text{
padding-bottom: 10%;
}
.text2{
  font-size: 55px;
  margin: -18.5% 21%;
}
.boxs{
  a{
    margin: 28% 14% 10%;
  }
}
}
</style>
