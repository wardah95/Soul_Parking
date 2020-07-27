<template>
<div class="dashboard">
<h1><b>{{ msg }}</b></h1>
  <br>
  <b-container class="bv-example-row">
  <row :gutter="12">
        <column :xs="12" :lg="3">
        <b-card 
      footer="Card Footer"
      footer-tag="footer"
      footer-bg-variant="light"
      no-body class="overflow-hidden" style="max-width: 540px;">
      <b-row no-gutters>
        <b-col md="9">
        <b-card-body title="Kedatangan">
          <b-card-text>
            2.500
          </b-card-text>
        </b-card-body>
      </b-col>
        <b-col md="3">
        <b-card-img src="https://images.glints.com/unsafe/1024x0/glints-dashboard.s3.amazonaws.com/company-logo/6363072f79453b741343a12f915ea3c7.png" alt="Image" class="rounded-0"></b-card-img>
      </b-col>
      </b-row>
      </b-card>
        </column>
        <column :xs="12" :lg="3">
        <b-card 
      footer="Card Footer"
      footer-tag="footer"
      footer-bg-variant="light"
      no-body class="overflow-hidden" style="max-width: 540px;">
      <b-row no-gutters>
        <b-col md="8">
        <b-card-body title="PJP Lama">
          <b-card-text>
            2.000
          </b-card-text>
        </b-card-body>
      </b-col>
        <b-col md="3">
        <b-card-img src="https://images.glints.com/unsafe/1024x0/glints-dashboard.s3.amazonaws.com/company-logo/6363072f79453b741343a12f915ea3c7.png" alt="Image" class="rounded-0"></b-card-img>
      </b-col>
      </b-row>
      </b-card>
        </column>
        <column :xs="12" :lg="3">
        <b-card 
      footer="Card Footer"
      footer-tag="footer"
      footer-bg-variant="light"
      no-body class="overflow-hidden" style="max-width: 540px;">
      <b-row no-gutters>
        <b-col md="9">
        <b-card-body title="PJP Baru">
          <b-card-text>
           500  
          </b-card-text>
        </b-card-body>
      </b-col>
        <b-col md="3">
        <b-card-img src="https://images.glints.com/unsafe/1024x0/glints-dashboard.s3.amazonaws.com/company-logo/6363072f79453b741343a12f915ea3c7.png" alt="Image" class="rounded-0"></b-card-img>
      </b-col>
      </b-row>
      </b-card>
        </column>
        <column :xs="12" :lg="3">
          <b-card 
      footer="Card Footer"
      footer-tag="footer"
      footer-bg-variant="light"
      no-body class="overflow-hidden" style="max-width: 540px;">
      <b-row no-gutters>
        <b-col md="9">
        <b-card-body title="Keluar">
          <b-card-text>
            1.500
          </b-card-text>
        </b-card-body>
      </b-col>
        <b-col md="3">
        <b-card-img src="https://images.glints.com/unsafe/1024x0/glints-dashboard.s3.amazonaws.com/company-logo/6363072f79453b741343a12f915ea3c7.png" alt="Image" class="rounded-0"></b-card-img>
      </b-col>
      </b-row>
      </b-card>
        </column>
  
        <column :xs="12" :lg="6">
      <b-card img-src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRZsogzzNV_yPdoabnf39gNMNBYs3lIFfhNhw&usqp=CAU" img-alt="Card image" img-bottom class="mb-3">
      <b-card-text>
        <h2>Total Pemasukan</h2> <h2><b>Rp 1.500.000</b></h2>
      </b-card-text>
      </b-card>
        </column>
        <column :xs="12" :lg="6">
      <b-card img-src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRtVffM1-dMYB5SAzN8oMKHeXnZT8OyQPjT2Q&usqp=CAU" img-alt="Card image" img-bottom class="mb-3">
      <b-card-text>
        <h2>Membership</h2> <h2><b>1.200</b></h2>
      </b-card-text>
      </b-card>
        </column>
        <column :xs="12" :lg="6">
      <b-card img-src="https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSURyE4ZNP7cYnaqME5K7arOCR6jbRigb8kEw&usqp=CAU" img-alt="Card image" img-bottom class="mb-3">
      <b-card-text>
        <h2>Tarif Situs</h2>
      </b-card-text>
      </b-card>
        </column>
        <column :xs="12" :lg="6">
      <b-card img-src="https://static.sederet.com/images/2018/11/pie-chart.png" img-alt="Card image" img-bottom class="mb-3">
      <b-card-text>
        <h2>Metode Pembayaran</h2>
      </b-card-text>
      </b-card>
        </column>  
      </row>
</b-container>
</div>
</template>

<script>
export default {
  name: 'dashboard',
  data () {
    return {
      msg: 'Dashboard'
    }
  }
}
</script>

