<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/login">Login</router-link> |
    <router-link to="/register">Register</router-link> |
    <router-link to="/forgot">Forgot password</router-link>
  </div>
  <router-view/>
</template>

<style lang="scss">
body {
  background: #101010;
}

label, button {
  color: #E3E2D7;
  cursor: pointer;
}

input {
  display: flex;
  justify-content: center;
  align-items: center;
  line-height: 32px;
  background-color: transparent;
  color: #fff;
  font-size: 18px;
  border: none;
  border-bottom: 1px solid #E3E2D7;
  outline: none;
}

.input-group {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 20px;
  flex-direction: column;
  &:last-child {
    margin-bottom: 0;
  }
}

.block, .button {
  border: none;
  border-radius: 12px;
  background-color: rgba(48,48,48,.7);
  backdrop-filter: blur(20px);
}

.block {
  &-inner {
    padding: 20px;
  }
  &-container {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}

.button {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px;
  &.big {
    font-size: 20px;
    padding: 15px;
  }
  &.bottom {
    border-top-left-radius: 0;
    border-top-right-radius: 0;
  }
  &.enlarged {
    width: 100%;
  }
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
