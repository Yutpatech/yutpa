<template>
    <div class="side-button" @mouseover="hover = true" @mouseleave="hover = false">
        <div style="display:flex">
            <slot></slot>
            <div class="side-button__line" :class="{ lineactive : hover}"></div>
        </div>
        <b-icon
            icon="home">
        </b-icon>
    </div>
</template>

<script>
export default {
    data(){
        return{
            hover:false,
        }
    },
    methods:{
    }
}
</script>

<style scoped>
.side-button{
    background: #2365A4;
    color: white;
    border: solid 1px #2365A4;
    margin-right: 3rem;
    margin-top: 2rem;
    padding: .8rem;
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
}
.side-button:hover{
    background: white;
    color: #2365A4;
}
.side-button__line{
    width: 5px;
    height: 25px;
    background: white;
    margin-left: .8rem;
}
.lineactive{
    background: #2365A4;
}
</style>