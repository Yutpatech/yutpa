<template>
  <div class="bracket noselect column">
    <slot></slot>
  </div>
</template>


<style scoped>
.bracket{
  font-weight: 700;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  min-height: 100px;
  padding: 1rem;
  margin: 1rem;
  background: #222222;
  color: #ffffff;
}
.bracket:hover{
  background: #2365A4;
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