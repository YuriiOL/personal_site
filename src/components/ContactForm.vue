<template>
  <div class="maillBox">
    <h1>Contact me</h1>
    <form action="https://formspree.io/oleksovskyi@gmail.com" method="POST">
      <label>
        <input class="name" type="text" name="name" placeholder="Name" />
      </label>
      <label>
        <input class="email" type="email" name="_replyto" placeholder="Email" />
      </label>

      <textarea name="message" placeholder="Message"></textarea>

      <button type="submit" value="Send">
        <b>Send</b>
      </button>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.maillBox {
  height: 500px;
  width: 300px;
  position: relative;
  margin-left: -200px;
}
h1 {
  margin-left: 23%;
}

label {
  display: block;
  float: left;
}

textarea {
  display: block;
  height: 50%;
  width: 70%;
  position: absolute;
  left: 13%;
  top: 33%;
  resize: none;
  background-color: rgb(43, 43, 43);
  border: 1px solid white;
  color: white;
  font-size: 13px;
}

button {
  position: absolute;
  left: 13%;
  top: 87%;
  width: 72%;
  background-color: white;
  color: black;
  height: 30px;
}
button:hover {
  color: orangered;
}
.name {
  position: absolute;
  left: 13%;
  width: 33%;
  top: 20%;
  height: 30px;
  color: white;
  font-size: 10px;
}
.email {
  position: absolute;
  left: 50%;
  width: 33%;
  top: 20%;
  height: 30px;
  color: white;
  font-size: 10px;
}
input {
  background-color: rgb(43, 43, 43);
  border: 1px solid white;
}
@media (max-width: 1000px) {
  .maillBox {
    margin-left: -160px;
  }
}
@media (max-width: 800px) {
  .maillBox {
    margin-left: 0px;
    font-size: 15px;
  }
}
@media (max-width: 480px) {
  .maillBox {
    margin-left: -50px;
    font-size: 15px;
  }
}
</style>