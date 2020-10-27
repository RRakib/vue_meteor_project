<template>
  <div className="container">
    <header>
      <h1>Todo List</h1>
    </header>
    <form>
      <div>
        <label>Student Name</label>
        <p>
          <input type="text" placeholder="Enter student name" />
        </p>
      </div>
      <div>
        <label>Student Email</label>
        <p>
          <input type="email" placeholder="Enter student email" />
        </p>
      </div>
      <div>
        <label>Student Phone</label>
        <p>
          <input type="email" placeholder="Enter student phone" />
        </p>
      </div>
      <div>
        <button type="submit">Submit</button>
      </div>
    </form>
  </div>
</template>

<script>
import Vue from "vue";
import Task from "./Task.vue";

export default {
  components: {
    Task
  },
  data() {
    return {};
  },
  methods: {
    getTasks() {
      return [
        { _id: 1, text: "This is task 1" },
        { _id: 2, text: "This is task 2" },
        { _id: 3, text: "This is task 3" }
      ];
    }
  }
};
</script>
