<template>
    
<div id="login-box">
    <div class="left">
        <h1>Sign in</h1>
        <form action="/signin" method="post">
            <input type="text" v-model="userData.username" placeholder="Username" />
            <input type="password" name="password" placeholder="Password" value="" />
            <input type="submit" name="signup_submit" value="Sign me up" />
        </form>
    </div>
  
    <div class="right">
       <span class="loginwith">Sign in with<br />social network</span>
       <button class="social-signin facebook">Log in with facebook</button>
       <button class="social-signin twitter">Log in with Twitter</button>
       <button class="social-signin google">Log in with Google+</button>
    </div>
    <div class="or">OR</div>
</div>
  </template>
  
  <script>
  export default {
    name: 'signinPage',
    data() {
        return {
            userData: {
                username: '',
                password: '',
            }
        }
    }
  }
  </script>
  
  <style scoped>

  </style>