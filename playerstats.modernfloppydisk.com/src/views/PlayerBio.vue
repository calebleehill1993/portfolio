<template>
<div>
<div>
  <PlayerBio :player="player" />
</div>
<div class="github">
  <a href="https://github.com/BYU-CS-260-Winter-2020/lab-3b-grocery-store-calebleehill1993">Github Classroom</a>
</div>
</div>
</template>

<script>
import PlayerBio from "../components/PlayerBio.vue"
export default {
  name: 'Cart',
  components: {
    PlayerBio
  },
  data() {
    return {
    }
  },
  computed: {
    player() {
      return this.$root.$data.currentPlayer;
    },
    notEmpty() {
      return this.$root.$data.notEmpty;
    }
  },
  methods: {
  }
}
</script>
