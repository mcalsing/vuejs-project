<template>
 <!--  <Header />
  <router-view/> -->
  <div class="container">
    <p class="title">Fill the form</p>
    <div class="field">
      <label class="label">Name</label>
      <div class="control">
        <input class="input" type="text">
      </div>
    </div>

  <div class="field">
    <label class="label">Username</label>
    <div class="control has-icons-left">
      <input class="input" type="text" placeholder="User">
      <span class="icon is-small is-left">
        <i class="fas fa-user"></i>
      </span>
    </div>
  </div>

  <div class="field">
    <label class="label">Email</label>
    <div class="control has-icons-left">
      <input class="input" type="email" placeholder="Email">
      <span class="icon is-small is-left">
        <i class="fas fa-envelope"></i>
      </span>
    </div>
  </div>

  <div class="field">
    <label class="label">Subject</label>
    <div class="control">
      <div class="select">
        <select>
          <option>Select dropdown</option>
          <option>Student</option>
          <option>Professor</option>
          <option>Speaker</option>
        </select>
      </div>
    </div>
  </div>

  <div class="field">
    <label class="label">Message</label>
    <div class="control">
      <textarea class="textarea" placeholder="Textarea"></textarea>
    </div>
  </div>

  <div class="field is-grouped">
    <div class="control">
      <button class="button is-link" @click="handleClick">Exemplo 3</button>
    </div>
    <div class="control">
      <button class="button">Cancel</button>
    </div>
  </div>
</div>
</template>

<script>


export default {
  name: "Form",
  data() {
    return {};
  },
  methods: {
    handleClick() {
      this.$router.push("/pokemons");
    }
  },
}
</script>