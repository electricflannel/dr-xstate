<script>
export default {};
</script>

<template>
  <button :class="$style.button"></button>
</template>

<style module>
.button {
  width: 0;
  height: 75px;
  padding-left: 75px;
  overflow: hidden;
  position: relative;
  float: left;
  box-sizing: border-box;
  border-radius: 10px;
  margin: 1px;
  box-shadow: inset 0 2px 2px #fff, inset 0 -1px 2px #aeaba4;
  background: #e9e4da;
  background: -moz-linear-gradient(top, #e9e4da 0%, #e9e5db 100%);
  background: -webkit-linear-gradient(top, #e9e4da 0%, #e9e5db 100%);
  background: linear-gradient(to bottom, #e9e4da 0%, #e9e5db 100%);
  transition: all 0.2s ease;
}

.button:after {
  content: "";
  display: block;
  box-sizing: border-box;
  position: absolute;
  top: 11px;
  left: 11px;
  width: 50px;
  height: 50px;
  border-radius: 50px;
  box-shadow: inset 0 0 3px #fff, 0 0 10px #fff,
    inset 0 5px 10px rgba(0, 0, 0, 0.03);
  color: black;
  background: -moz-linear-gradient(top, #d7d0c0 0%, #fefefe 100%);
  background: -webkit-linear-gradient(top, #d7d0c0 0%, #fefefe 100%);
  background: linear-gradient(to bottom, #d7d0c0 0%, #fefefe 100%);
}
</style>
