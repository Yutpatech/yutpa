<template>
  <section class="section indexpage">
    <div class="homebox">
      <vue-typed-js class="typedjs" :strings="['have vanished.', 'are coming back.']" :typeSpeed="100" :backSpeed="100">
        <h1>Dragons <span class="typing"></span></h1>
      </vue-typed-js>
      <p style="margin-top: 2rem;max-width:600px;">
        Efsanelerde adı geçen ejderhalardan ilham alarak yola çıktık.
        Kodlarımızı ejderhaları hayal eden insanların hayal güçleriyle süsledik.
        Ve projelerimizi mühendislik teknikleriyle, güncel teknolojileri kullanarak özenle geliştiriyoruz. 
        Eğer projeniz varsa ve hayata geçirmek için birilerini arıyorsanız, doğru yerdesiniz!
      </p>
      <div class="columns is-mobile" style="max-width: 600px;margin-top: 1.5rem;">
        <a href="mailto:hi@yutpa.net" target="_blank" class="test noselect"><span>Teklif Al</span></a>
      </div>
     <!-- <img src="~/assets/programing.png" width="200" /> -->
    </div>
    <h1 style="font-size:1.8rem;color:#222;margin-bottom:28px;">Neler kullanıyoruz?</h1>
    <h3>Back-end</h3>
    <div class="buttons columns is-mobile">
      <Bracket>Php</Bracket>
     <Bracket>Node.js</Bracket>
     <Bracket>Python</Bracket>
     <Bracket>Firebase</Bracket>
    </div>
    <h3>Front-end</h3>
    <div class="buttons columns is-mobile">
      <Bracket>Html5</Bracket>
      <Bracket>Css3</Bracket>
     <Bracket>Javascript</Bracket>
     <Bracket>Vue.js</Bracket>
     <Bracket>Nuxt.js</Bracket>
    </div>
  </section>
</template>

<script>
//import Card from '~/components/Card'
import Bracket from '~/components/Showcases/Bracket.vue'

export default {
  name: 'HomePage',

  components: {
    Bracket
  }
}
</script>
<style scoped>
.main-container, .indexpage{
  background: url('../assets/yut.png');
  background-size: 500px;
  background-size: 40%;
  background-position-x: right;
  background-position-y: top;
  background-repeat: no-repeat;
}
.homebox{
  margin-bottom: 9.5rem;
}
.buttons{
  display: flex;
}
.typedjs{
  font-size: 2.85rem;
  color: #222222;
}

@media screen and (max-width: 480px) {
  .homebox{
    padding-top: 3.5rem;
  }
}

@media screen and (min-width: 480px) and (max-width:768px) {
  .homebox{
    max-width: 415px;
  }
  .typedjs{
    font-size: 2rem;
  }
}


.test {
  border: none;
  display: block;
  text-align: center;
  cursor: pointer;
  outline: none;
  overflow: hidden;
  position: relative;
  color: #fff;
  font-weight: 700;
  font-size: 15px;
  background-color: #222;
  padding: 17px 60px;
  margin: 0 auto;
  box-shadow: 0 5px 15px rgba(0,0,0,0.20);
  width: 220px;
}

.test span {
  position: relative; 
  z-index: 1;
}
.test:after {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 490%;
  width: 140%;
  background: #2365A4;
  -webkit-transition: all .5s ease-in-out;
  transition: all .5s ease-in-out;
  -webkit-transform: translateX(-98%) translateY(-25%) rotate(45deg);
  transform: translateX(-98%) translateY(-25%) rotate(45deg);
}

.test:hover:after {
  -webkit-transform: translateX(-30%) translateY(-25%) rotate(45deg);
  transform: translateX(-30%) translateY(-25%) rotate(45deg);
}
.noselect {
  -webkit-touch-callout: none; /* iOS Safari */
    -webkit-user-select: none; /* Safari */
     -khtml-user-select: none; /* Konqueror HTML */
       -moz-user-select: none; /* Old versions of Firefox */
        -ms-user-select: none; /* Internet Explorer/Edge */
            user-select: none; /* Non-prefixed version, currently supported by Chrome, Edge, Opera and Firefox */
            cursor: pointer;
}
</style>