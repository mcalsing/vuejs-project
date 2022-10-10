<template>
  <div class="box column is-4 is-offset-one-third">
    <div class="field">
      <p class="control has-icons-left">
        <input class="input" placeholder="Email" />
        <span class="icon is-small is-left">
          <i class="fas fa-envelope" />
        </span>
      </p>
    </div>
    <div class="field">
      <p class="control has-icons-left">
        <input class="input" type="password" placeholder="Senha" />
        <span class="icon is-small is-left">
          <i class="fas fa-lock" />
        </span>
      </p>
    </div>
      <button class="button is-primary" @click="handleClick">Exemplo 2</button>
  </div>
</template>

<script>
// @ is an alias to /src
/* import HelloWorld from '@/components/HelloWorld.vue' */

export default {
  name: 'Login',
  data() {
    return {

    }
  },
  methods: {
    handleClick() {
      this.$router.push('/form');
    }
  }
}
</script>
