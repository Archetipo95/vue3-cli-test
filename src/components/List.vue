<template>
  <div>
    <article v-for="person in people" :key="person.id" className="person">
      <img :src="person.image" :alt="person.name" />
      <div>
        <h4>{{ person.name }}</h4>
        <p>{{ person.age }} years old</p>
      </div>
    </article>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    people: Array,
  },
};
</script>
