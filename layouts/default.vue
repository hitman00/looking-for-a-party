<template>
  <div>
    <Nuxt />
  </div>
</template>

<style lang="scss" module>
  *,
  *::before,
  *::after {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    background-image: url('~/assets/imgs/background55.png');
    background-color: #1d2635;
    background-position: right top;
    background-repeat: no-repeat;
    overflow-x: hidden;
  }

  a {
    text-decoration: none;
  }

  @font-face {
    font-family: 'Righteous';
    font-style: normal;
    font-weight: normal;
    src: url('@/assets/fonts/font/Righteous.woff') format('woff');
  }

  @font-face {
    font-family: 'Sanchez';
    font-style: normal;
    font-weight: normal;
    src: url('@/assets/fonts/font/Sanchez-Regular.woff') format('woff');
  }
</style>
