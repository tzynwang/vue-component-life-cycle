<template>
  <nav id="nav" ref="nav">
    nav count: {{ count }}
    <button @click.stop="addCount">nav count +1</button>
  </nav>
</template>

<script>
export default {
  name: 'navComponent',
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
    console.group('beforeCreate nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  created () {
    console.group('created nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  beforeMount () {
    console.group('beforeMount nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  mounted () {
    console.group('mounted nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  beforeUpdate () {
    console.group('beforeUpdate nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  updated () {
    console.group('updated nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  beforeDestroy () {
    console.group('beforeDestroy nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  },
  destroyed () {
    console.group('destroyed nav ===============')
    console.log(this.$data)
    console.log(this.$el)
    console.log(this.$refs.nav)
  }
}
</script>
