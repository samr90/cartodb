<template>
  <router-link :to="{ name: 'maps' }" class="action-link title is-small" :class="{ 'action-link--empty-state': isEmptyState }">
    {{ text }}
  </router-link>
</template>

<script>
export default {
  name: 'MapsLink',
  props: {
    text: String,
    isEmptyState: Boolean
  }
};
</script>

<style scoped lang="scss">
@import "stylesheets/new-dashboard/variables";

.action-link {
  display: block;
  margin-top: 28px;
  letter-spacing: 1px;
  text-align: center;
  text-transform: uppercase;

  &.action-link--empty-state {
    margin-top: 64px;
  }
}
</style>
