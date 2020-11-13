<template>
  <div id="profile">
    <div class="full">
    <b-avatar variant="dark" size="7rem"></b-avatar>
    <h2 class="first-text">Hey,</h2>
    <p>nice to see you again!</p> 
      <input type="text" class="form-control" placeholder="Your Email *" value="" />

      <input type="password" class="form-control" placeholder="Your Password *" value="" />

      <input type="submit" class="btnSubmit" value="Login" /> | 

      <a href="#" class="btnForgetPwd" value="Login">Forgot password?</a>
      <router-link to="/">
      <p><b-icon icon="arrow-left-circle-fill" class="flecha"></b-icon></p>
      </router-link>
    </div>
  </div>
</template>

  



<script>
export default {
  name: 'Profile'

}
</script>

<style>


  .full{  
    z-index: 999;
    margin-top:30%;
    height: 100%;
}

.first-text{
  font-family: arial black;
  font-weight: bold;
  color: #b0c8f3;
}

.login-form-2{
    background: #f05837;
    box-shadow: 0 5px 8px 0 rgba(0, 0, 0, 0.2), 0 9px 26px 0 rgba(0, 0, 0, 0.19);
}
.btnSubmit{
    font-weight: 600;
    color: #282726;
    background-color: #fff;
    margin-top: 4vh;
    border: none;
    border-radius: 1.5rem;
}
.btnForgetPwd{
    color: #000;
    font-weight: 600;
    margin-top: 4vh;
    text-decoration: none;
    border-radius: 1.5rem;
}
.btnForgetPwd:hover{
    text-decoration: none;
    color: #000;
}
.flecha{
  font-size: 4rem;
  color: #b0c8f3; 
  margin-top: 7vh;
}
</style>