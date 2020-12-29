<template>
  <div class="list-user">
    <p>List User Component</p>
    <!-- <user />
    <user />
    <user />
    <user /> -->
    {{ titleHeader }}
    <!-- {{ listUser }} -->
    <user v-for="user in listUserT" v-bind:key="user.email" />
  </div>
</template>

<script>
import User from "./User.vue";
export default {
  name: "List User",
  props: {
    titleHeader: String,
    listUserT: {
      type: Array,
    },
  },
  data() {
    return {};
  },
  components: {
    User,
  },
};
</script>
