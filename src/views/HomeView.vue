<template>
  <div id="app">
    <p class="user-id">User ID: {{ userId }}</p>
    <div class="chat-container">
      <input v-model="message" @keyup.enter="sendMessage" placeholder="Type a message" class="chat-input" />
      <button @click="sendMessage" class="send-button">Send</button>
      <ul class="messages">
        <li v-for="message in messages" :key="message.id" :class="{'my-message': message.userId === userId}">
          <strong>{{ message.userId }}:</strong> {{ message.content }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
export default {

}
</script>

<style scoped>
#app {
  font-family: Arial, sans-serif;
  text-align: center;
  margin-top: 100px;
  background-color: rgb(161, 230, 165);
}

input {
  padding: 10px;
  width: 300px;
  margin-right: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  padding: 10px 20px;
  background-color: #4caf50;
  color: white;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

ul {
  list-style-type: none;
  padding: 0;
  margin: 20px 0;
}

li {
  padding: 10px;
  margin: 5px 0;
  border: 1px solid #ccc;
  border-radius: 4px;
  text-align: left;
}

p {
  margin-top: 20px;
  font-weight: bold;
}
</style>

