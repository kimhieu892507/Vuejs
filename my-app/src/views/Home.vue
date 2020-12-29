<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <!-- <hello-world /> -->
    <ListUser v-bind:titleHeader="title" v-bind:listUser="listUser" />
    <!-- <ListUser titleHeader="title" /> -->
    <!-- <ListUser v-bind:listUserT="listUserT" /> -->
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import ListUser from "@/components/ListUser.vue";
export default {
  name: "Home",
  data() {
    return {
      title: "Good morning",
      listUserT: [
        { email: "test@gmail.com", active: true },
        { email: "test1@gmail.com", active: false },
        { email: "test2@gmail.com", active: false },
        { email: "test3@gmail.com", active: false },
        { email: "test4@gmail.com", active: false },
        { email: "test5@gmail.com", active: false },
      ],
    };
  },
  components: {
    HelloWorld,
    ListUser,
    // HelloWorld
  },
};
</script>
