<template>
  <div class="block-container">
    <div class="block">
      <form action="/api/register">
        <div class="block-inner">
          <div class="input-group">
            <label for="login">Login</label><br/>
            <input type="text" name="login" id="login">
          </div>
          <div class="input-group">
            <label for="Email">Email</label><br/>
            <input type="email" name="email" id="email">
          </div>
          <div class="input-group">
            <label for="password">Password</label><br/>
            <input type="password" name="password" id="password">
          </div>
          <div class="input-group">
            <label for="password-confirm">Password confirmation</label><br/>
            <input type="password" name="password-confirm" id="password-confirm">
          </div>
        </div>
        <button type="submit" class="button big bottom enlarged">Register</button>
      </form>
    </div>
  </div>
</template>

<style lang="scss">
.register {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {}
})
export default class Register extends Vue {}
</script>
