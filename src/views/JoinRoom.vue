<template>
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col-md-6">
            <div class="card-body">
              <form>
                <div class="form-group  mb-4">
                  <label for="code">{{ codeLabel }}</label>
                  <input type="code" class="form-control" id="code" v-model="code">
                </div>
                <div class="d-grid gap-2 mb-4">
                    <button type="submit" class="btn btn-primary" v-on:click.prevent="join">{{ joinButton }}</button>
                </div>
                <div class="d-grid gap-2 mb-5">
                    <button type="submit" class="btn btn-primary" v-on:click.prevent="returnButton">{{ returnButton }}</button>
                </div>
                <div class="d-grid gap-2 d-md-block mx-auto">
                  <button class="btn btn-outline-primary  btn-sm" type="button">공지사항</button>
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
        codeLabel: '방코드',
        returnButton: '이전으로',
        joinButton: '방입장',
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
  