<template>
  <div>
    <p>Hello World! Hello World! Hello World! Hello World! Hello World! Hello World!</p>
    <p>{{ message }}</p>
    <!-- <input v-model="message"> -->
    <ul>
      <li v-for="item in items" :key="item.id">
        {{ item.text }}
      </li>
    </ul>
    <button @click="clickEvent()">click</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: ['message'],
  data: () => ({
    // message: 'hello world',
    items: [
      { id: 1, text: 'アイテム1' },
      { id: 2, text: 'アイテム2' },
      { id: 3, text: 'アイテム3' },
    ],
  }),
  methods: {
    clickEvent() {
      console.log('clicked!');
    },
  },
};
</script>
