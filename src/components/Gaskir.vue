<template>
  <div class="gaskir">    
  <h1><b>{{ msg }}</b></h1>
  <br>
  <b-container class="bv-example-row">
  <row :gutter="12">
    <column :xs="12" :lg="6">
    <b-card>
    <template v-slot:header>
      <h4 class="mb-0">List Petugas parkir</h4>
    </template>
    <b-list-group flush>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar variant="success" class="mr-3"></b-avatar>
        <span class="mr-auto">Malika</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar class="mr-3"></b-avatar>
        <span class="mr-auto">J. Circlehead</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar variant="primary" text="BV" class="mr-3">BM</b-avatar>
        <span class="mr-auto">Bambang</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar variant="info" src="https://placekitten.com/300/300" class="mr-3"></b-avatar>
        <span class="mr-auto">Dita Mila</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar variant="success" icon="people-fill" class="mr-3">BK</b-avatar>
        <span class="mr-auto">Vijay</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar class="mr-3">JN</b-avatar>
        <span class="mr-auto">Junaydi</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar variant="primary" src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQFD8weP2uC1l_7K7EnMlHKHJEG4WN9eej8nw&usqp=CAU" text="BV" class="mr-3"></b-avatar>
        <span class="mr-auto">Taka</span>
      </b-list-group-item>
      <b-list-group-item class="d-flex align-items-center">
        <b-avatar variant="info" src="https://i.mydramalist.com/WBZrWc.jpg" class="mr-3"></b-avatar>
        <span class="mr-auto">Andrea</span>
      </b-list-group-item>
    </b-list-group>
  </b-card>
        </column>
        <column :xs="12" :lg="6">
        <b-card
    title="Tambah Petugas"
    img-src="https://cms.dailysocial.id/wp-content/uploads/2020/06/235d46031c0fb7da02e2c6c64f9f77ef_Soul-Parking-2.png"
    img-alt="Image"
    img-top
    tag="article"
    class="mb-2">
    <b-card-text>
      Silahkan Klik Tambah Untuk Menambah Petugas Parkir
    </b-card-text>
    <b-button v-b-toggle.tambah class="m-1">Tambah</b-button>
    <b-collapse id="tambah">
    <b-form>
    <label class="sr-only" for="inline-form-input-name">Name</label>
    <b-input
      id="inline-form-input-name"
      class="mb-2 mr-sm-2 mb-sm-0"
      placeholder="Name"></b-input>

    <label class="sr-only" for="inline-form-input-username">Username</label>
    <b-input-group prepend="@" class="mb-2 mr-sm-2 mb-sm-0">
      <b-input id="inline-form-input-username" placeholder="Username"></b-input>
    </b-input-group>
    <b-button variant="primary">Save</b-button>
    </b-form>
  </b-collapse>
  </b-card>
      </column>
      </row>
</b-container>
  </div>


</template>

<script>
export default {
  name: 'gaskir',
  data () {
    return {
      msg: 'Tambah Petugas Parkir'
    }
  }
}
</script>

