<template>
  <div class="block-container">
    <div class="block login">
      <form action="/api/login">
        <div class="block-inner">
          <div class="input-group">
            <label for="login">Login</label>
            <input type="text" name="login" id="login">
          </div>
          <div class="input-group">
            <label for="password">Password</label>
            <input type="password" name="password" id="password">
          </div>
        </div>
        <button class="button big bottom enlarged" type="submit">Login</button>
      </form>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  components: {}
})
export default class Login extends Vue {}
</script>
