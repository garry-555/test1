<template>
  <section>
    <h2>my friends</h2>
    <ul>
      <friend-contact> </friend-contact>
      <friend-contact> </friend-contact>
    </ul>
  </section>
</template>

<script>
import FriendContact from "./components/FriendContact.vue";
export default {
  components: { FriendContact },
  data() {
    return {
      friends: [
        {
          id: "garry",
          name: "gaurav",
          phone: "89998",
          emailId: "krgmail.com",
        },
        {
          id: "saf",
          name: "safder",
          phone: "77675",
          emailId: "safgmail.com",
        },
      ],
    };
  },
};
</script>


