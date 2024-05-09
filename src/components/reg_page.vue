<template>
    <div class= "root">
            <p className = "paste-bin">PasteBin</p>
            <input className ="login" type="text" name="username" v-model="userName" placeholder="login">
      <input className ="password" type="password" name="password" v-model="userPass" placeholder="password">
            <input className = "repeat_password" type="password" name="secPpassword" placeholder="password">
            <button className ="sign-up" type="submit" name="signUp">Sign Up</button>
    </div> 
</template>

<script>
</script>

<style scoped>
.root {
  background-color: white;
  border-radius: 20px;
  border: 1px solid grey;
  height: 400px;
  width: 300px;
  display: flex;
  flex-direction: column;
  margin-top: 15%;
  margin-left: auto;
  margin-right: auto;
  align-items: center;
  }
  .paste-bin {
    font-family: "Limelight";
    font-size: 36px;
    font-weight: 400;
    color: #5F5F5F;
  }

  input {
    margin: 10px;
    border: 1px solid grey;
    height: 30px;
    box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.25);
    border-radius: 20px;
    text-align: center;
    flex: auto;
  }
  .login {
    margin-top: 0px;
  }

  button {
    font-family: "Libre Franklin";
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    color: white;
    width: 175px;
    height:50px; 
    background-color: #5F5F5F;
    margin: 10px;
    box-shadow: 0 4px 4px 0 rgba(0, 0, 0, 0.25);
    border-radius: 20px;
    margin-bottom: 20px;
    flex: auto;
    transition: transform 500ms ease;
  }

  button:hover {
    transform: scale(1.1) translateY(-1px);
}
</style>

<script>

</script>