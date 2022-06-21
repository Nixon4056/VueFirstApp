<template>
  <section>
    <h2>Nikodem Wicon</h2>
    <ul>
      <friend-contact></friend-contact>
      <friend-contact></friend-contact>
    </ul>
  </section>
</template>

<script>
export default {
  data() {
    return {
      friends: [
        {
          id: 'Nikodem',
          name: 'Nikodem Wicon',
          phone: '+48 696 787 013',
          email: 'nikodem@nicode.pl'
        },
        {
          id: 'Marta',
          name: 'Marta Rybicka',
          phone: '+48 668 246 135',
          email: 'nikodem@nesperta.com'
        }
      ],
    };
  },
}
</script>