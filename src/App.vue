<template>
  <div class="container">
    <Header title="Task Tracker" />
    <Tasks :tasks="tasks" />
  </div>
</template>

<script>
import Header from "./components/Header";
import Tasks from "./components/Tasks";
export default {
  name: "App",
  components: {
    Header,
    Tasks,
  },
  data() {
    return {
      tasks: [],
    };
  },
  created() {
    this.tasks = [
      {
        id: 1,
        text: "Pick up laundry at the aircraft carrier",
        day: "Monday",
        reminder: true,
      },
      {
        id: 2,
        text: "Go on date at aircraft carrier",
        day: "Tuesday",
        reminder: false,
      },
      {
        id: 3,
        text: "Wipe up vomit on aircraft carrier",
        day: "Monday",
        reminder: true,
      },
    ];
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 40px;
}

body {
  background-color: #ccb;
  padding: 0px 20px 30px 20px;
}

.container {
  /* margin: 10px; */
  /* padding: 10px; */
  height: 100vh;
  background-color: #deefee;
  box-shadow: 0 0 15px rgba(0, 80, 0, 0.4);
}

button {
}

button:hover {
}
</style>
