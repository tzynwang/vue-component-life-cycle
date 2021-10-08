<template>
  <header id="header" ref="header">
    <navComponent />
    <hr>
    header count: {{ count }}
    <button @click.stop="addCount">header count +1</button>
  </header>
</template>

<script>
import navComponent from './navComponent.vue'

export default {
  name: 'headComponent',
  components: {
    navComponent
  },
  data () {
    return {
      count: 0
    }
  },
  methods: {
    addCount () {
      this.count += 1
    }
  },
  beforeCreate () {
    console.group('beforeCreate header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  created () {
    console.group('created header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  beforeMount () {
    console.group('beforeMount header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  mounted () {
    console.group('mounted header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  beforeUpdate () {
    console.group('beforeUpdate header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  updated () {
    console.group('updated header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  beforeDestroy () {
    console.group('beforeDestroy header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  },
  destroyed () {
    console.group('destroyed header ===============')
    console.log(this.$el)
    console.log(this.$refs.header)
    // console.log(this.$refs.nav)
  }
}
</script>
