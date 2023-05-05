<template>
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col-md-6">
            <div class="card-body">
              <form>
                <div class="form-group mb-2">
                  <label for="id">{{ idLabel }}</label>
                  <input type="id" class="form-control" id="id" v-model="id">
                </div>
                <div class="d-grid gap-2 d-md-flex justify-content-md-end">
                <button class="btn btn-outline-primary btn-sm" id="sm-btn" type="button">ID중복체크</button>
                </div>
                <div class="form-group mb-2">
                  <label for="password">{{ passwordLabel }}</label>
                  <input type="password" class="form-control" id="password" v-model="password">
                </div>
                <div class="form-group mb-5">
                  <label for="password_chk">{{ passwordChkLabel }}</label>
                  <input type="password_chk" class="form-control" id="passwordChk" v-model="passwordChk">
                </div>
                
                <div class="d-grid gap-2 mb-4">
                <button type="submit" class="btn btn-primary btn-lg" id="bg-btn"  v-on:click.prevent="join">{{ joinButton }}</button>
                </div>
                <div class="d-grid gap-2 d-md-block mx-auto">
                  <button class="btn btn-outline-primary btn-sm" id="sm-btn"  type="button">공지사항</button>
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
        idLabel: 'ID',
        passwordLabel: 'Password',
        passwordChkLabel: 'Password 확인',
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
  #bg-btn:hover{
      transform: translateY(-5px); 
  }
  .btn{
            transition: .4s all;
        }
   
  #sm-btn:hover{
      transform: scale(1.2); 
  }
  </style>
  