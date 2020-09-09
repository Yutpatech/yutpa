<template>
<section class="side">
<vue-particles class="side-particle" style="background:#222222;" 
    color="#ffffff" 
    linesColor="#ffffff"	
    :particlesNumber="200"
    :clickEffect="false"
    :hoverEffect="false">
    </vue-particles>
</section>
</template>

<style scoped>
.side{
    min-height: 100vh;
    background: #222222;
    color: #ffffff;
    flex:2;
}
.side-particle{
    height:100%;
}
@media screen and (max-width:1024px) {
    .side{
        display: none;
    }
}
</style>