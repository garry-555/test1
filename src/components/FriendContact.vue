<template>
  <li>
    <h2>{{ friend.name }}</h2>
    <button @click="toggleDetails">show details</button>
    <ul v-if="isVisible">
      <li><strong>phone: </strong> {{ friend.phone }}</li>
      <!-- <li><strong><strong> {{}}</li> -->
      <li><strong>email: </strong> {{ friend.emailId }}</li>
    </ul>
  </li>
</template>


<script>
export default {
  data() {
    return {
      isVisible: false,
      friend: {
        id: "garry",
        name: "gaurav",
        phone: "89998",
        emailId: "krgmail.com",
      },
    };
  },
  methods: {
    toggleDetails() {
      this.isVisible = !this.isVisible;
    },
  },
};
</script>
