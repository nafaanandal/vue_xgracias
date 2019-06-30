<template>
  <div class="dashboard">
    <!-- navbar -->
    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <!-- Brand/logo -->
      <a class="navbar-brand" href="#">
        <img src="images/logo_xgracias.jpeg" alt="Logo" style="width:180px;">
      </a>
      <!-- Links -->
      <ul class="nav navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#">19/20/1</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">NOTIFICATION</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">ACCOUNT</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">LANGUAGE</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">LOGOUT</a>
        </li>
      </ul>
    </nav>

    <!-- The sidebar -->
    <div class="sidebar">
      <img src="images/user.jpg" alt="Cinque Terre" style="width:200px;height:170px;">
      <h3 style="text-align: center">NAMA USER</h3>
      <div class="dropdown">
        <button
          type="button"
          class="btn btn-primary dropdown-toggle"
          data-toggle="dropdown"
        >1301154559(NIM)</button>
        <div class="dropdown-menu">
          <span class="dropdown-item-text">kelas :</span>
          <span class="dropdown-item-text">dosen wali :</span>
          <span class="dropdown-item-text">program studi:</span>
        </div>
      </div>
      <div class="dropdown">
        <button
          type="button"
          class="btn btn-primary dropdown-toggle"
          data-toggle="dropdown"
        >GROUP PENGGUNA (ROLE 1)</button>
        <div class="dropdown-menu">
          <a class="dropdown-item" href="#">ROLE 2</a>
        </div>
      </div>
      <form class="form-inline" action="/action_page.php">
        <input class="form-control mr-sm-2" type="text" placeholder="Search">
        <button class="btn btn-success" type="submit">Search</button>
      </form>
      <a href="#home">Akun</a>
      <a href="#news">Asrama Mahasiswa</a>
      <a href="#contact">Bimbingan Konseling</a>
      <a href="#about">CeLOE</a>
      <a href="#about">Dispensasi</a>
      <a href="#about">Ekuivalensi</a>
      <a href="#about">Elearning(Idea)</a>
    </div>

    <!-- Page content -->
    <div class="content">
      <h1>Selamat datang #namauser</h1>
    </div>
  </div>
</template>

<style>
.Dashboard {
  /* background-image: url("images/background_telyu.jpg"); */
  background-position-x: center;
}

.navbar-brang {
  display: inline-block;
  padding-top: 0.3125rem;
  padding-bottom: 0.3125rem;
  /* margin-right: 1rem; */
  font-size: 1.25rem;
  line-height: inherit;
  white-space: nowrap;
}

/* The side navigation menu */
.sidebar {
  margin: 0;
  padding: 0;
  width: 200px;
  background-color: #f1f1f1;
  position: fixed;
  height: 100%;
  overflow: auto;
}

/* Sidebar links */
.sidebar a {
  display: block;
  color: black;
  padding: 16px;
  text-decoration: none;
}

/* Active/current link */
.sidebar a.active {
  background-color: #4caf50;
  color: white;
}

/* Links on mouse-over */
.sidebar a:hover:not(.active) {
  background-color: #555;
  color: white;
}

/* Page content. The value of the margin-left property should match the value of the sidebar's width property */
div.content {
  margin-left: 200px;
  padding: 1px 16px;
  height: 1000px;
}

/* On screens that are less than 700px wide, make the sidebar into a topbar */
@media screen and (max-width: 700px) {
  .sidebar {
    width: 100%;
    height: auto;
    position: relative;
  }
  .sidebar a {
    float: left;
  }
  div.content {
    margin-left: 0;
  }
}

/* On screens that are less than 400px, display the bar vertically, instead of horizontally */
@media screen and (max-width: 400px) {
  .sidebar a {
    text-align: center;
    float: none;
  }
}
</style>

