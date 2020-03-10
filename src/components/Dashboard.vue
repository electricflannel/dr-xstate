<script>
import DoomsDayClock from "./DoomsDayClock";
import NuclearCodes from "./NuclearCodes";
export default {
  name: "Dashboard",
  components: {
    DoomsDayClock,
    NuclearCodes
  }
};
</script>

<template>
  <div>
    <header>
      <h1>Doomsday Dashboard</h1>
    </header>
    <main>
      <dooms-day-clock />
      <nuclear-codes />
    </main>
  </div>
</template>
