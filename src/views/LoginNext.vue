<template>
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col-md-6">
            <div class="card-body">
              <form>
                <div class="d-grid gap-2 mb-4">
                <button type="submit" class="btn btn-primary btn-lg" v-on:click.prevent="create">{{ createButton }}</button>
                </div>
                <div class="d-grid gap-2 mb-5">
                <button type="submit" class="btn btn-primary btn-lg" v-on:click.prevent="join">{{ joinButton }}</button>
                </div>
                <div class="d-grid gap-2 d-md-block mx-auto">
                  <button class="btn btn-outline-primary btn-sm" type="button">공지사항</button>
                </div>
              </form>
            </div>
            
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Login',
    data() {
      return {
        createButton: '방생성',
        joinButton: '방참가',
        email: '',
        password: ''
      }
    },
    methods: {
      login() {
        // your login logic goes here
      }
    }
  }
  </script>
  
  <style scoped>
  .card-header {
    background-color: #007bff;
    color: #fff;
  }
  </style>
  