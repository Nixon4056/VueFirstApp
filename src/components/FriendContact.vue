<template>
  <li>
    <h2>{{ name }}</h2>
    <button @click="toggleDetails">{{ detailsAreVisible ? 'Hide' : 'Show'}} Details</button>
    <ul v-if="detailsAreVisible">
      <li><strong>Phone: </strong>{{ phoneNumber }}</li>
      <li><strong>Email: </strong>{{ emailAddress }}</li>
    </ul>
  </li>
</template>

<script>

export default{
  props: [
    'name',
    'phoneNumber',
    'emailAddress'
  ],
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
