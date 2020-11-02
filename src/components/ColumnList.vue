<template>
  <ul></ul>
</template>

<script lang="ts">
import { defineComponent, PropType } from 'vue'
export interface ColumnProps{
  id: number;
  title: string;
  avatar: string;
  description: string;
}
export default defineComponent({
  props: {
    list: {
      type: Array as PropType<ColumnProps[]>,
      required: true
    }
  },
  setup (props) {
    console.log(props)
  }
})
</script>

<style lang="scss" scoped></style>
