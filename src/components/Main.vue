<template>
    <main class="hello">
        <div>
            <span>Notifications <b>{{ notifications }}</b></span>
            <button>Mark all as read</button>
        </div>
        <NotificationCard />
    </main>
  </template>
  
  <script>
import NotificationCard from '@/components/NotificationCard.vue'

  export default {
    name: 'HelloWorld',
    props: {
      msg: String
    },
    components: {
        NotificationCard
    },  
    data() {
        return {
            notifications: 3,
            cards: {}
        }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  h3 {
    margin: 40px 0 0;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
  </style>
  