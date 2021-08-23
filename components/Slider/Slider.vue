<template>
  <div :class="$style.slider_main">
    <div :class="$style.boxs">
      <div :class="$style.title">Looking for a party ?</div>
      <div :class="$style.description">
        Vulputate odio nulla sit vel duis eget in suspendisse a posuere non duis
        eget in eget in suspendisse a posurer non duis eget in
      </div>
      <div :class="$style.search_box">
        <img src="@/assets/imgs/search_icon.png" />
        <input type="text" placeholder="Search party" />
        <div :class="$style.find_box">Find Party</div>
      </div>
    </div>
    <div :class="$style.boxs">
      <div :class="$style.iphone_image">
        <img src="@/assets/imgs/iphone11.png" />
      </div>
      <div :class="$style.download_app">
        <svg viewBox="0 0 120 120">
          <circle id="MyPath" cx="60" cy="60" r="45" fill="none" />

          <text fill="#FFFFFf">
            <textPath href="#MyPath">DOWNLOAD THE APP</textPath>
          </text>
        </svg>
        <img src="@/assets/imgs/down_arrow_white.png" />
      </div>
    </div>
    <div :class="$style.search_box2">
      <input type="text" placeholder="Search party" />
      <div :class="$style.find_box">Find Party</div>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'Iphone'
  };
</script>

<style lang="scss" module>
  .slider_main {
    display: flex;
    margin-top: 6.2%;
  }

  .boxs {
    width: 50%;
    position: relative;
  }

  .title {
    color: #fff;
    font-size: 120px;
    font-weight: bold;
  }

  .description {
    color: #fff;
    width: 76%;
    font-size: 20px;
    font-family: tahoma;
    margin-top: 6%;
    margin-bottom: 10%;
  }

  .iphone_image {
    width: 110%;
    position: relative;
    &:before {
      display: block;
      content: '';
      padding-bottom: 100%;
    }
    img {
      position: absolute;
      bottom: 0;
      top: 0;
      left: 0;
      right: 0;
      width: 100%;
    }
  }

  .search_box {
    width: 70.7%;
    padding: 1%;
    border-radius: 50px;
    background: #323c48;
    display: flex;
    align-items: center;
    margin-bottom: 18.2%;
    input {
      background: none;
      color: #fff;
      border: none;
      align-self: normal;
      flex-grow: 1;
    }
    img {
      padding: 0 6% 0 8%;
      transition: all 0.3s ease;
    }
    &:hover img {
      transform: rotate(90deg) scale(1.2);
      padding-left: 8%;
    }
  }

  .download_app {
    position: absolute;
    right: 14%;
    bottom: 13%;
    width: 200px;
    height: 200px;
    opacity: 0.7;
    background: #000;
    color: #fff;
    border-radius: 50%;
    transform: rotate(180deg);
    font-size: 14px;
    cursor: pointer;
    transition: all 0.3s ease;
    &:hover {
      opacity: 0.8;
    }
    svg {
      position: absolute;
      transition: all 0.5s ease;
    }
    &:hover svg {
      transform: rotate(360deg);
    }
    img {
      margin: 37% auto 0;
      display: block;
      transition: all 0.5s ease;
    }
    &:hover img {
      transform: rotate(-180deg);
    }
  }

  .search_box2 {
    width: 100%;
    display: none;
    flex-direction: column;
    text-align: center;
    input {
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

  .find_box {
    padding: 4.6%;
    border-radius: 50px;
    background: #27ffe6;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    transition: all 0.3s ease;
    &:hover {
      opacity: 0.8;
    }
  }
  @media (max-width: 1215px) {
    .iphone_image {
      width: 130%;
    }
  }

  @media (max-width: 1000px) {
    .title {
      font-size: 90px;
    }

    .description {
      font-size: 13px;
    }

    .find_box {
      font-size: 10px;
    }

    .download_app {
      display: none;
    }
  }

  @media (max-width: 800px) {
    .boxs {
      width: 100%;
    }

    .slider_main {
      flex-direction: column;
      margin-top: 10%;
      margin-bottom: 10%;
    }

    .description {
      width: 100%;
      font-size: 15px;
    }

    .search_box {
      display: none;
    }

    .iphone_image {
      width: 100%;
      margin: 0 auto;
    }

    .search_box2 {
      display: flex;
    }

    .iphone_image {
      z-index: -1;
    }
  }
</style>
