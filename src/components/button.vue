<template>
<div class="button-container">
  <button class="button">Home</button>
  <button class="button">About</button>
  <button class="button">Skill</button>
</div>

</template>

<style scoped>
@import url('https://fonts.cdnfonts.com/css/common-pixel');

.button-container {
  text-align: center;
  margin-top: 50px; 
  
}

.button {
  background-color: transparent;
  border: none;
  outline: none;
  padding: 10px 20px;
  margin: 0 10px;
  position: relative;
  font-family: 'Common Pixel', sans-serif;
  color: wheat;
}

.button::before,
.button::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  background-color: palevioletred;
  transition: width 0.3s;
}

.button::before {
  top: 0;
  left: 0;
}

.button::after {
  bottom: 0;
  right: 0;
}

.button:hover::before,
.button:hover::after {
  width: calc(100% - 10px); 
}


</style>