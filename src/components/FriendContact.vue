<template>
  <li>
    <h2>{{ friend.name }}</h2>
    <button @click="toggleDetails">Show Details</button>
    <ul v-if="detailsAreVisible">
      <li><strong>Phone: </strong>{{ friend.phone }}</li>
      <li><strong>Email: </strong>{{ friend.email }}</li>
    </ul>
  </li>
</template>

<script>

export default{
  data() {
    return{
      detailsAreVisible: false,
      friend: {
        id: 'Nikodem',
        name: 'Nikodem Wicon',
        phone: '+48 696 787 013',
        email: 'nikodem@nicode.pl'
      },
    };
  },
  methods: {
    toggleDetails(){
      this.detailsAreVisible = !this.detailsAreVisible;
    },
  },
};
</script>
