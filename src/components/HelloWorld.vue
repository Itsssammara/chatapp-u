

<script>
// import io from 'socket.io-client';
// import { ref } from 'vue';

// export default {
//   setup() {
//     const socket = io();
//     const userId = ref('');
//     const messages = ref([]);
//     const message = ref('');

//     socket.on('userId', (id) => {
//       userId.value = id;
//     });

//     const sendMessage = () => {
//       if (message.value.trim() !== '') {
//         const newMessage = { content: message.value, userId: userId.value, id: Date.now() };
//         socket.emit('chat message', newMessage);
//         messages.value.push(newMessage);
//         message.value = '';
//       }
//     };

//     return { socket, userId, messages, message, sendMessage };
//   },
// };
</script>

