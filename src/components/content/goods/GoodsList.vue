<template>
  <div class="goods">
    <goods-list-item v-for="item in goods" :key="item.acm" :goods-item="item"/>
  </div>
</template>

<script>
import GoodsListItem from './GoodsListItem'

export default {
  data () {
    return {
    };
  },
  props: {
    goods: {
      type: Array,
      default() {
        return []
      }
    }
  },

  components: {
    GoodsListItem
  },

  computed: {},

  methods: {}
}

</script>

<style scoped>
  .goods {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 2px;
  }
</style>
