<template>
  <div :class="$style.main">
    <div :class="$style.boxs">
      <div :class="$style.title">
        Looking for a party ?
      </div>
      <div :class="$style.description">
        Vulputate odio nulla sit vel duis eget in suspendisse a posuere non duis eget in eget in suspendisse a posurer non duis eget in
      </div>
      <div :class="$style.search_box">
        <img src="@/assets/imgs/search_icon.png">
        <input type="text" placeholder="Search party">
        <div :class="$style.find_box">
          Find Party
        </div>
      </div>
    </div>
    <div :class="$style.boxs">
      <div :class="$style.image">
        <img src="@/assets/imgs/iphone.png">
      </div>
    </div>
    <div :class="$style.search_box2">
      <input type="text" placeholder="Search party">
      <div :class="$style.find_box">
        Find Party
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
  margin-top: 6.2%;
}
.boxs{
    width: 50%;
}
.title{
    color: #fff;
    font-size: 120px;
    font-weight: bold;
}
.description{
  color: #fff;
  width: 76%;
  font-size: 20px;
  font-family: tahoma;
  margin-top: 6%;
  margin-bottom: 10%;
}

.image{
  position: relative;
  &:before{
    display: block;
    content: '';
    padding-bottom: 100%;
  }
  img{
    position: absolute;
    bottom: 0;
    top:0;
    left: 0;
    right: 0;
    width: 100%;
  }
}

.search_box{
  width: 70.7%;
 padding: 1%;
  border-radius: 50px;
  background: #323c48;
  display: flex;
  align-items: center;
  margin-bottom: 18.2%;
  input{
    background: none;
    color: #fff;
    border: none;
    width: 53%;
  }
  img{
    padding: 0 6% 0 8%;
  }
}

.search_box2{
  width: 100%;
  display: none;
  flex-direction: column;
  text-align: center;
  input{
    background: none;
    color: #fff;
    border: none;
    width: 100%;
    text-align: center;
    background: #323c48;
    padding: 4.6%;
    margin: 6% auto 2%;
    border-radius: 50px;

}
}

.find_box{
 padding: 4.6% ;
  border-radius: 50px;
  background: #27ffe6;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  transition: all 0.3s ease;
  &:hover{
    opacity: 0.8;
  }
}
@media(max-width: 1215px){
  .search_box input{
        width: 48%;

  }
}

@media(max-width: 1000px){

.title{
    font-size: 90px;
}

.description , .find_box{

  font-size: 13px;
}

 .search_box input{
        width: 46%;

  }
}

@media(max-width: 800px){
.boxs{
    width: 100%;
}

.main{
flex-direction: column;
  margin-top: 10%;
  margin-bottom: 10%;
}

.description{
  width: 100%;
  font-size: 15px;
}

.search_box{
  display: none;
}

.image{
width: 70%;
margin: 0 auto;
}

.search_box2{
  display: flex;
}

.image{
  img{
    height: 100%;
  }
}

}
</style>
