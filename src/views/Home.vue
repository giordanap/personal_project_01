<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/cdz.jpg">
    <hr/>
    <Task :task="task" />
  </div>
</template>

<script>
import { mapState } from 'vuex'
import Task from '../components/Task'

export default {
  name: 'Home',
  components: {
    Task
  },
  computed: {
    ...mapState(['task'])
  },
}
</script>
