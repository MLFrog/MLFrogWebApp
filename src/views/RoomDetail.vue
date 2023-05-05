<template>
    <div class="container">
      <div class="row justify-content-center mt-5">
        <div class="col-md-6">
            <div class="card-body">
              <form>
                <div class="row mb-5">
                  <div class="col-md-6">
                    <div class="form-group mb-2">
                      <label for="code">{{ code }}</label>
                      <input type="code" class="form-control" id="code" >
                    </div>
                  </div>
                  <div class="col-md-6">
                    <div class="form-group mb-2">
                      <label for="cnt">{{ cnt }}</label>
                      <input type="cnt" class="form-control" id="cnt" >
                    </div>
                  </div>
                </div>
                <div class="row mb-4">
                  <div class="col-md-6">
                    <div class="d-grid gap-2 mx-auto">
                      <button class="btn btn-outline-danger" id="bg-btn" type="button">파일업로드</button>
                    </div>                    
                  </div>
                  <div class="col-md-6 border-3">
                    <div class="col-md-12">
                      <div class="row">
                        <div class="col-md-4">
                          <div class="border border-top-5 p-3" >
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="d-grid gap-2 d-md-block mx-auto">
                  <button class="btn btn-outline-primary btn-sm" id="sm-btn" type="button">공지사항</button>
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
        code: '방 코드',
        cnt: '참가인원 수',
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
  

  
  