<template>
  <div class="root">
    <div className="header">
      <p className="pasteBin">PasteBin</p>
        <p className="login">admin</p>
    </div>
      <div className="main">
        <form action="#">
          <div className="wrapper">
            <button name="paste" @click="PostMapping">Paste</button>
              <select name="expireIn" v-model="time">
                <option value="1">1 Hour</option>
                <option value="24">24 Hours</option>
                <option value="168">1 Week</option>
              </select>
          </div>
          <textarea name="text" v-model="snippet"></textarea>
          <p>{{ time }}</p>
          <p>{{ snippet }}</p>
        </form>
      </div>
  </div> 
</template>

<style scoped>
body {
  margin: 0;
}

.header {
  background-color: #5F5F5F;
  margin-bottom: 20px;
  border-radius: 0 0 20px 20px;
  padding: 38px 17px; 
  display: flex;
  align-items: center;
}

.pasteBin {
  font-family: "Limelight";
  font-size: 48px;
  font-weight: 400;
  color: rgba(232, 227, 227, 1);
}

.login {
  font-family: "Libre Franklin";
  font-size: 16px;
  font-weight: 700;
  color: rgba(232, 227, 227, 1);
  position: absolute;
  right: 10px;
}

textarea {
  border-radius: 20px;
  border: 1px solid grey;
  resize: none;
  width: 80%;
  height: 550px;
  margin: 0 auto; 
}

button {
  font-family: "Libre Franklin";
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  color: white;
  width: 100px;
  height: 50px;
  background-color: #5F5F5F;
  border-radius: 40px;
  border: none; 
  margin: 10px;
  margin-bottom: 20px; 
  transition: transform 500ms ease;
} 
button:hover {
  transform: scale(1.1) translateY(-1px);
}
.wrapper {
  display: flex;
  justify-content: flex-end;
  width: 80%;
  margin: auto;
}

select {
    height: 50px;
    background-color: #5F5F5F;
    color: white;
    border: none;
    border-radius: 40px;
    padding: 0 20px;
    font-family: "Libre Franklin";
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    margin: 10px;
}

select:focus {
    outline: none;
}
</style>

<script>
export default {
  data (){
    return {
      snippet: '',
      time: ''
    }
  },
  methods: {
    PostMapping () {

    },

    GetMapping () {

    },

    PutMapping () {

    },

    DeleteMapping () {

    }
}
}
</script>