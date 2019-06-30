<template>
  <div class="login">
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <!-- Brand/logo -->
      <a class="navbar-brand" href="#">
        <img src="../assets/logo_xgracias.jpeg" alt="Logo" style="width:180px;">
      </a>
      <!-- Links -->
      <ul class="nav navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#" data-toggle="modal" data-target="#myModal">LOGIN</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">ADMISSION</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">PARENTS LOGIN</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">DELA</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">SSO ACTIVATION</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">OTHERS</a>
        </li>
      </ul>
    </nav>

    <!-- The Modal -->
    <div
      class="modal"
      id="myModal"
      data-backdrop="static"
      data-keyboard="false"
      style="background: transparent"
    >
      <div class="modal-dialog">
        <div class="modal-content" style="margin-top: 100px">
          <!-- Modal Header -->
          <div class="modal-header">
            <h6 class="modal-title" style="margin-top: 13px;margin-left: 10px">SSO LOGIN</h6>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              style="text-align: right"
            >&times;</button>
          </div>

          <!-- Modal body -->
          <div class="modal-body">
            <form>
              <div class="form-group">
                <input
                  type="username"
                  class="form-control"
                  id="username"
                  placeholder="Enter username"
                  name="username"
                >
              </div>
              <div class="form-group">
                <input
                  type="password"
                  class="form-control"
                  id="pwd"
                  placeholder="Enter password"
                  name="pswd"
                >
              </div>
              <div class="form-group form-check">
                <label class="form-check-label">
                  <input class="form-check-input" type="checkbox" name="remember"> Remember me
                </label>
              </div>
              <button type="submit" class="btn btn-primary">LOGIN</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.login {
  background-image: url("../assets/bg.jpg");
  background-position: center;
  height: 100vh;
}
/* Bordered form */
/* form {
    border: 3px solid #f1f1f1;
  } */

/* Full-width inputs */
input[type="text"],
input[type="password"] {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

/* Set a style for all buttons */
button {
  background-color: #4caf50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
}

/* Add a hover effect for buttons */
button:hover {
  opacity: 0.8;
}

/* Extra style for the cancel button (red) */
.cancelbtn {
  width: auto;
  padding: 10px 18px;
  background-color: #f44336;
}

/* Center the avatar image inside this container */
.imgcontainer {
  text-align: center;
  margin: 24px 0 12px 0;
}

/* Avatar image */
img.avatar {
  width: 40%;
  border-radius: 50%;
}

/* Add padding to containers */
.container {
  padding: 16px;
}

/* The "Forgot password" text */
span.psw {
  float: right;
  padding-top: 16px;
}

/* Change styles for span and cancel button on extra small screens */
@media screen and (max-width: 300px) {
  span.psw {
    display: block;
    float: none;
  }
  .cancelbtn {
    width: 100%;
  }
}

.btn {
  border: none; /* Remove borders */
  color: white; /* Add a text color */
  padding: 14px 28px; /* Add some padding */
  cursor: pointer; /* Add a pointer cursor on mouse-over */
}

.success {
  background-color: #4caf50;
} /* Green */
.success:hover {
  background-color: #46a049;
}

* {
  box-sizing: border-box;
}
/* Full-width input fields */
input[type="text"],
input[type="password"] {
  width: 100%;
  padding: 15px;
  margin: 5px 0 22px 0;
  display: inline-block;
  border: none;
  background: #f1f1f1;
}

/* Add a background color when the inputs get focus */
input[type="text"]:focus,
input[type="password"]:focus {
  background-color: #ddd;
  outline: none;
}

/* Set a style for all buttons */
button {
  background-color: #4caf50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  cursor: pointer;
  width: 100%;
  opacity: 0.9;
}

button:hover {
  opacity: 1;
}

/* Extra styles for the cancel button */
.cancelbtn {
  padding: 14px 20px;
  background-color: #f44336;
}

/* Float cancel and signup buttons and add an equal width */
.cancelbtn,
.signupbtn {
  float: left;
  width: 50%;
}

/* Add padding to container elements */
.container {
  padding: 16px;
}

/* The Modal (background) */
.modal {
  display: none; /* Hidden by default */
  position: fixed; /* Stay in place */
  z-index: 1; /* Sit on top */
  left: 0;
  top: 0;
  width: 100%; /* Full width */
  height: 100%; /* Full height */
  overflow: auto; /* Enable scroll if needed */
  background-color: #474e5d;
  padding-top: 50px;
}

/* Modal Content/Box */
.modal-content {
  background-color: #fefefe;
  margin: 5% auto 15% auto; /* 5% from the top, 15% from the bottom and centered */
  border: 1px solid #888;
  width: 80%; /* Could be more or less, depending on screen size */
}

/* Style the horizontal ruler */
hr {
  border: 1px solid #f1f1f1;
  margin-bottom: 25px;
}

/* The Close Button (x) */
.close {
  position: absolute;
  right: 35px;
  top: 15px;
  font-size: 40px;
  font-weight: bold;
  color: #f1f1f1;
}

.close:hover,
.close:focus {
  color: #f44336;
  cursor: pointer;
}

/* Clear floats */
.clearfix::after {
  content: "";
  clear: both;
  display: table;
}

/* Change styles for cancel button and signup button on extra small screens */
@media screen and (max-width: 300px) {
  .cancelbtn,
  .signupbtn {
    width: 100%;
  }
}
.modal-backdrop {
  z-index: -1;
}
.close {
  color: grey;
}
</style>

