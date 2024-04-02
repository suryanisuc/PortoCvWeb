<template>
   <div class="profile">
  <profile />
 </div>

  <div class="hedder">
    <h1>Portofolio</h1>
  </div>

  <div class="Paragraf">
    <h3>Hai Saya suci ,</h3>
    <p>Saya seorang Mahasiswa Universitas Islam Riau.</p>
    <p>Skill yang saya punya dalam IT adalah <br>Pengembangan Web. Saya menguasai beberapa<br>bahasa pemrograman dasar.</p>
  </div>

  <div class="hobby">
    <p>Hobby saya manjat tebing, daki gunung,dan rafting .</p>
  </div>
  <div class="Sosial">
    <Social />
  </div>

  <div class="Cat">
    <Cat />
  </div>

  <div class="girl">
    <girl />
  </div>

  <div class="hub">
    <hub />
  </div>

  <div class="button">
    <but />
  </div>

</template>

<script>
import Social from './components/icons/Sosial.vue';
import Cat from './components/Cat.vue';
import girl from './components/girl.vue';
import hub from './components/icons/git.vue';
import but from './components/button.vue';
import profile from './components/profile.vue';

export default {
  name: 'App',
  components: {
    Social,
    Cat,
    girl,
    hub,
    but,
    profile
  }
}
</script>

<style>
@import url('https://fonts.cdnfonts.com/css/chilling-nightime');
@import url('https://fonts.cdnfonts.com/css/diary-santa');

body {
  background: rgb(88,1,97);
  background: linear-gradient(90deg, rgba(88,1,97,1) 0%, rgba(121,9,119,1) 35%, rgba(213,0,255,1) 100%);
  overflow: hidden;
}


.profile >*{
  z-index: -1;
  position: fixed;
}

.Paragraf{
  font-weight: bold;
  position: fixed;
  right: 700px;
  top: 300px;
  font-family: 'Diary Santa', sans-serif;
  color: thistle;
  text-shadow: 0 0 10px purple;
}

.hobby{
  font-weight: bold;
  position: fixed;
  display: block;
  right: 700px;
  top: 470px;
  left: 600px;
  font-family: 'Diary Santa', sans-serif;
  color: thistle;
  text-shadow: 0 0 10px purple;
  
}

.hedder{
  font-weight: bold;
  color: violet;
  position: fixed;
  z-index: 99;
  top: 80px;
  margin-top: -80px;
  margin-left: -700px;
  overflow: hidden;
  font-family: 'Chilling Nightime', sans-serif;
  font-size: 30px;
}
.button {
  z-index: 99;
  position: fixed;
  font-size: 24px;
  overflow: hidden;
  margin-top: -390px;
  margin-left: -200px;
}
.Sosial {
  display: flex;
  align-items: center; 
  justify-content: center; 
  position: fixed;
  bottom: 50%;
  right: 0;
  top: 50%;
  padding: 0 400px;
  z-index: 3;
}

.Sosial > * {
  margin-left: 10px; 
  width: 40px; 
  height: auto; 
  filter: drop-shadow(0 0 10px #000);
}

.Cat {
  position: fixed;
  bottom: 50%;
  right: 0;
  top: 150px;
  z-index: 4;
  size: 10px; 
  padding: 0 100px;
}

.Cat > * {
  margin-left: 10px; 
  width: 20px; 
  height: auto; 
  transform: scaleX(-1);
}

.girl{
  z-index: 1;
  margin-top: -100px;
  margin-left: -800px;
  overflow: hidden;
}

.hub{
  display: flex;
  align-items: center; 
  justify-content: center; 
  position: fixed;
  bottom: 250px;
  right: 0;
  top: 50%;
  padding: 0 430px;
  z-index: 3;
}
.hub >*{
  margin-left: 10px; 
  width: 30px; 
  height: auto; 
}

</style>
