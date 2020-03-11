<script>
import DoomsDayClock from "./DoomsDayClock";
import NuclearCodes from "./NuclearCodes";
import Led from "./Led";
import BraunButton from "./BraunButton";

export default {
  name: "Dashboard",
  components: {
    DoomsDayClock,
    NuclearCodes,
    Led,
    BraunButton
  }
};
</script>

<template>
  <div>
    <header>
      <h1>Doomsday Dashboard</h1>
    </header>
    <main style="padding: 5px;">
      <led />
      <braun-button></braun-button>
      <dooms-day-clock />
      <nuclear-codes />
    </main>
  </div>
</template>
