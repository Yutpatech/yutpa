<template>
<section>
  <Header/>
  <div class="main-layout">
    <div class="main-container">
      <nuxt />
    </div>
    <Side/>
  </div>
</section>
</template>

<script>
import Header from '~/components/General/Header.vue';
import Side from '~/components/General/Side.vue';
import Sidebutton from '~/components/Parts/Sidebutton.vue';

export default {
  components: {
    Header,
    Side,
    Sidebutton
  },
  data () {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Inspire',
          icon: 'lightbulb',
          to: { name: 'inspire' }
        }
      ]
    }
  }
}
</script>

<style scoped>
*{
  font-family: 'Work Sans', sans-serif;
}
.main-layout{
  display: flex;
  flex-direction: row-reverse;
  max-width: 100%;
}
.main-container{
  height: 100%;
  max-width: 1024px;
  margin:auto;
  margin-right: 4rem;
  margin-left: 4rem;
  flex:8;
}
@media screen and (max-width: 1024px){
  .main-container{
    max-width: 100vw;
    margin: 1rem;
  }
}
</style>
