<template>
  <div id="Footer">
    <div class="content">
      {{confName}} | Fork on
      <a href="https://github.com/CCIP-App/CCIP-Puzzle-Bueno/" target="_blank" alt="Source code on GitHub">GitHub</a>
    </div>
  </div>
</template>

<script>
import config from '../../config/project.json'
export default {
  name: 'Footer',
  data () {
    return {
      confName: config.confName,
      chip: true
    }
  }
}
</script>

<style lang="stylus">
#Footer
  display: flex
  justify-content: center
  align-items: flex-end
  flex-grow: 1
  // background-size: cover
  // background-repeat: no-repeat
  // background-image: url('../assets/footer.png')
  // background-position: center top
  .content
    padding: 2em
    color: #3b097a
    font-size: 12px
  a
    color: #3b097a
  .fillet-label
    background-color: rgba(0, 0, 0, .5)
</style>
