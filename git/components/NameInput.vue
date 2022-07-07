<template>
  <div>
    <form>
      <label for="name">Name:</label>
      <input type="text" id="name" />
      <button>Submit</button>
    </form>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
form {
  width: 15%;
  display: flex;
  flex-direction: column;
  margin-top: 50px;
}

label {
  font-weight: 700;
}

input {
  padding: 5px 5px;
  margin: 6px 0 20px;
  border: 1px solid rgb(175, 175, 175);
  border-radius: 6px;
}

button {
  width: 50%;
  padding: 8px 20px;
  background-color: rgb(134, 134, 134);
  border: 1px solid rgb(134, 134, 134);
  color: white;
  border-radius: 6px;
  cursor: pointer;
}

button:hover {
  background-color: rgb(150, 150, 150);
  border: 1px solid rgb(150, 150, 150);
}
</style>
