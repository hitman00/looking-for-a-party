<template>
  <div :class="$style.main">
    <div :class="$style.profile">
      <div :class="$style.avatar">
        YP
      </div>
      <div :class="$style.user">
        Yu party
      </div>
    </div>
    <div :class="$style.pages">
      <a href="#">Home</a>
      <a href="#">About Us</a>
      <a href="#">Contact Us</a>
      <a href="#">Category</a>
    </div>
    <div :class="$style.icon_page">
      <img src="@/assets/imgs/meno_icon.png">
    </div>
    <div :class="$style.registry">
      REGISTER
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" module>
.main{
    display: flex;
    padding-top: 4.5%;

}

.profile{
    width: 20%;
    display: flex;
}

.avatar{
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: #29ffe8;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    transition: all 0.3s ease;
    &:hover{
      background:#a8ff0d;
    }
}

.user{
    display: flex;
    align-items: center;
    padding-left: 5%;
    color: #fff;

}

.pages{
    width:60% ;
    display: flex;
    padding: 0 10%;
    align-items: center;
    justify-content: space-evenly;
    a{
    color: #fff;
    display: block;
    transition: all 0.3s ease;
    font-family: tahoma;

    &:hover{
        opacity: 0.8;
    }
    }
}

.icon_page{
display: none;
align-items: center;
justify-content: center;
width: 8%;
cursor: pointer;
transition: all 0.3s ease;
&:hover{
  opacity: 0.7;
}
}

.registry{
    display: flex;
    align-items: center;
    justify-content: end;
    width: 20%;
    color: #3cefdb;
    cursor: pointer;
       transition: all 0.3s ease;
    &:hover{
      opacity: 0.8;
    }
}

@media(max-width: 800px){
.pages{
   display: none;
}
.registry{
  display: none;
}

.icon_page{
  display: flex;
}
.main{
  justify-content: space-between;
}
.profile{
    width: 50%;}
}
</style>
