<template>
  <div class="container">
    <global-header :user="user"></global-header>
    <column-list :list="list"></column-list>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
import 'bootstrap/dist/css/bootstrap.min.css'
import GlobalHeader, { UserProps } from './components/GlobalHeader.vue'
import ColumnList, { ColumnProps } from './components/ColumnList.vue'

const userData: UserProps = {
  isLogin: false,
  name: 'devin'
}
const testData: ColumnProps[] = [
  {
    id: 1,
    title: 'test1',
    description: '这是专栏',
    avatar: ''
  },
  {
    id: 1,
    title: 'test1',
    description: '这是专栏',
    avatar: ''
  },
  {
    id: 1,
    title: 'test1',
    description: '这是专栏',
    avatar: ''
  },

  {
    id: 1,
    title: 'test1',
    description: '这是专栏',
    avatar: ''
  }
]
export default defineComponent({
  components: {
    GlobalHeader,
    ColumnList
  },
  setup () {
    return {
      list: testData,
      user: userData
    }
  }
})
</script>
<style></style>
