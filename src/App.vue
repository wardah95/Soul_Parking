<template>
<div id="app">
  <b-navbar toggleable="lg" type="dark" variant="dark">
  <b-button v-b-toggle.Menu>Menu</b-button>
  <b-navbar-nav class="ml-auto">
    <b-dropdown split text="DKI Jakarta" variant="light" class="m-2" >
      <b-dropdown-item href="#">Jakarta Pusar</b-dropdown-item>
      <b-dropdown-item href="#">Jakarta Utara</b-dropdown-item>
      <b-dropdown-item href="#">Jakarta Selatan</b-dropdown-item>
      <b-dropdown-item href="#">Jakarta Barat</b-dropdown-item>
      <b-dropdown-item href="#">Jakarta Timur</b-dropdown-item>
    </b-dropdown>
  </b-navbar-nav> 
  <b-navbar-nav class="ml-auto">
    <b-list-group-item variant="dark">
      <b-avatar variant="info" src="https://placekitten.com/300/300" class="mr-3"></b-avatar>
    Wardatul Jannah
    </b-list-group-item>
  </b-navbar-nav>
  </b-navbar>

<b-sidebar id="Menu" shadow>
    <div class="px-3 py-2">
    <b-img src="https://res-3.cloudinary.com/crunchbase-production/image/upload/c_lpad,h_256,w_256,f_auto,q_auto:eco/tjlw9bptmczkeccr3vn0" fluid-grow alt="Fluid-grow image"></b-img>
    <div>
    <div>
      <b-icon-grid1x2-fill></b-icon-grid1x2-fill><b-button href="#" variant="light"><router-link to="dashboard">Dashboard</router-link></b-button> <br>
      <b-icon-files></b-icon-files><b-button v-b-toggle.penagturan variant="light">Pelaporan</b-button>
        <b-collapse id="penagturan" class="mt-2">
        <b-card>
          <b-button href="#" variant="light">Laporan Tarif</b-button> <br>
          <b-button href="#" variant="light">Laporan Pendapatan</b-button> <br>
          <b-button href="#" variant="light">Pengaduan</b-button> <br>
          <b-button href="#" variant="light">Laporan Member</b-button> <br>
          <b-button href="#" variant="light">Laporan Gaskir</b-button> <br>
          <b-button href="#" variant="light">Laporan Aplikasi</b-button>
        </b-card>
        </b-collapse>
    </div>
    <div>
      <b-icon-gear-fill></b-icon-gear-fill><b-button v-b-toggle.lokasi variant="light">Pengaturan Lokasi</b-button>
      <b-collapse id="lokasi" class="mt-2">
      <b-card>
        <b-button href="#" variant="light">Info Lokir</b-button> <br>
        <b-button href="#" variant="light">Tarif </b-button> <br>
        <b-button href="#" variant="light"><router-link to="gaskir">Gaskir</router-link></b-button> <br>
        <b-button href="#" variant="light">Shift</b-button> <br>
        <b-button href="#" variant="light">Produk</b-button> <br>
        <b-button href="#" variant="light">Pemulihan Kendaraan</b-button> <br>
        <b-button href="#" variant="light">Aktivasi Member</b-button> <br>
        <b-button href="#" variant="light">Pengaturan Penguna</b-button>
      </b-card>
      </b-collapse>
    </div>
    <div>
      <b-icon-person></b-icon-person><b-button v-b-toggle.admin variant="light">Sistem Admin</b-button>
      <b-collapse id="admin" class="mt-2">
      <b-card>
        <b-button href="#" variant="light">Lokis</b-button> <br>
        <b-button href="#" variant="light">Penguna </b-button> <br>
        <b-button href="#" variant="light">Hardware</b-button> <br>
      </b-card>
      </b-collapse>
    </div>
      <b-icon-person-circle></b-icon-person-circle><b-button href="#" variant="light">Sistem Admin</b-button><br>
      <b-icon-files></b-icon-files><b-button href="#" variant="light">Keluar</b-button>
  </div>
  </div>
  </b-sidebar>
  <h1><b>{{ msg }}</b></h1> <br>
  <router-view/> 
</div> 

</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Selamat Data Di Halaman Soul Parking'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
