<script>

  import SignIn from './sign-in'
  import SignUp from './sign-up'
  export default {
    components: {
      SignIn,
      SignUp
    },

    methods: {
      doSignIn (obj) {
      }
    }    
  }

</script>


<template>
  <div>
    <div class="login-wrap">
      <div class="login-html">
        <input id="tab-1" type="radio" name="tab" class="sign-in" checked><label for="tab-1" class="tab">Sign In</label>
        <input id="tab-2" type="radio" name="tab" class="sign-up"><label for="tab-2" class="tab">Sign Up</label>
        <div class="login-form">
					<sign-in @do-sign-in="doSignIn"/>
					<sign-up/>	
        </div>
      </div>
    </div>
  </div>
</template>

<style src="./style.css"></style>


