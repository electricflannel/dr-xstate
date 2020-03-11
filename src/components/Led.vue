<script>
export default {
  name: "Led",
  props: {
    on: Boolean
  },
  data: function() {
    return {
      toggled: false
    };
  },
  computed: {
    ledOn() {
      return this.on || this.toggled;
    }
  }
};
</script>

<template>
  <button
    :class="[$style.led, { [$style.ledOn]: ledOn }]"
    @click="toggled = !toggled"
  >
    Led
  </button>
</template>

<style module>
.led {
  position: relative;
  float: left;
  width: 20px;
  height: 20px;
  margin-right: 20px;
  border: 0;
  border-radius: 50%;
  outline: 0;
  background-color: #900;
  text-indent: -9999px;
  box-shadow: inset 0 0 0 1px rgba(0, 0, 0, 0.5),
    inset 0 0 0 2px rgba(255, 255, 255, 0.25),
    inset 0 5px 3px -2px rgba(255, 255, 255, 0.25),
    inset 0 -5px 3px -2px rgba(0, 0, 0, 0.1), 0 2px 5px 0px rgba(0, 0, 0, 0.5);
}

.led::before {
  content: "";
  position: absolute;
  display: block;
  top: 30%;
  left: 40%;
  left: 50%;
  width: 10%;
  width: 2px;
  height: 10%;
  height: 2px;
  margin-left: -1px;
  border-radius: 50%;
  background-color: #fff;
  box-shadow: 0 0 2px 2px rgba(255, 255, 255, 0.5),
    0 0 5px 5px rgba(255, 255, 255, 0.5);
}

.ledOn {
  background-color: #f00;
}
</style>
