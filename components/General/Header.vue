<template>
<nav class="header-layout">
    <div class="header-container">
        <div class="header-container__logo">
            <nuxt-link to="/">YUTPA</nuxt-link>
        </div>   
        <b-navbar style="flex:8;">
            <template slot="end">
                <b-navbar-item tag="router-link" to="/inspire">
                    Home
                </b-navbar-item>
                <b-navbar-item href="#">
                    Projects
                </b-navbar-item>
                <b-navbar-item href="#">
                    About
                </b-navbar-item>
            </template>
        </b-navbar>
    </div>
    <div class="header-right">
        <b-icon
                icon="instagram">
            </b-icon>
            <b-icon
                icon="linkedin">
            </b-icon>
            <b-icon
                icon="twitter">
            </b-icon>
            <b-icon
                icon="github">
            </b-icon>
            <b-icon
                icon="facebook">
            </b-icon>
    </div>
</nav>
</template>

<style scoped>
.header-layout{
    position: relative;
    display: flex;
    flex-direction: row-reverse;
    width: 100%;
}
.header-container{
    position: relative;
    display: flex;
    align-items: center;
    flex:8;
    margin-right: 4rem;
    margin-left: 4rem;
    max-width: 1024px;
}
.header-container__logo{
    flex:2;
    padding: 2rem 1rem 1rem 1.5rem;
}
.header-container__logo a {
    font-family: "Sansation_Bold", sans-serif;
    color: #222222;
    line-height: 1;
    font-size: 2.5rem;
}
.header-right{
    flex:2;
    background: #222222;
    color: #ffffff;
    display: flex;
    align-items: center;
    justify-content: center;
}
.header-right .icon{
    margin-left: 1rem;
}
@media screen and (max-width:1024px) {
    .header-layout{
        flex-direction: column-reverse;
    }
    .header-container{
        margin: 0 1rem;
    }
    .header-right{
        padding: 1rem;
        background: url("~assets/particle.png");
        background-color: #222222;
    }
    .navbar{
        position: absolute;
        top:25%;
        right:0;
    }
}
</style>