<template>
  <div>
    <slot />
    <slot name="title" />
    <slot name="item" v-bind="{ value: 'vue' }" />
    <slot name="test" :slotData="subName" />
  </div>
</template>

<script>
export default {
  name: "SlotDemo",
  data () {
    return {
      subName: '子slot'
    }
  }
};
</script>
