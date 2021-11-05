<template>
  <div>
    <ul v-for="user in users" :key="user.id">
      <li>
        <span>{{ user.name }}</span
        >&#160;
      </li>
    </ul>
    <form @submit.prevent="add">
        <input type="hidden" v-model="form.id">
        <input type="text" v-model="form.name">
        <button type="submit" v-show="!updateSubmit">add</button>
        <button type="button" v-show="updateSubmit" @click="update(form)">Update</button>
    </form>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      users: [],
      form: {
        id: '',
        name: ''
      },
      users: '',
      updateSubmit: false
    };
  },
  mounted() {
    this.load();
  },
  methods: {
    load() {
      axios
        .get(" http://localhost:3000/users")
        .then((res) => {
          this.users = res.data;
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
};


</script>