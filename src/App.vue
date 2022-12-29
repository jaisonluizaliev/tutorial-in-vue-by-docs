<script setup lang="ts">
import ChangeThingsDynamically from "./components/tutorial/ChangeThingsDynamically.vue";
import Conditional from "./components/tutorial/Conditional.vue";
import EventsListener from "./components/tutorial/EventsListener.vue";
import Forms from "./components/tutorial/Forms.vue";
import HelloWorldVue from "./components/tutorial/HelloWorld.vue";
import InterpolationVue from "./components/tutorial/Interpolation.vue";
import LifeCycle from "./components/tutorial/LifeCycle.vue";
import Lists from "./components/tutorial/Lists.vue";
import Props from "./components/tutorial/childs/Props/Props.vue";
import Watchers from "./components/tutorial/childs/Watchers/Watchers.vue";
import Emit from "./components/tutorial/childs/Emit/Emit.vue";
import SlotVue from "./components/tutorial/childs/Slot/Slot.vue";
</script>

<template>
  <InterpolationVue />
  <HelloWorldVue />
  <ChangeThingsDynamically />
  <EventsListener/>
  <Forms/>
  <Conditional/>
  <Lists/>
  <LifeCycle/>
  <Watchers/>
  <Props/>
  <Emit/>
  <SlotVue/>
</template>

<!-- <style scoped>

</style> -->
