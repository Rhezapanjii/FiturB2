<template>
  <div class="article-page d-flex">
    <ArticleNavbar></ArticleNavbar>
    <div class="col col-xl article">
      <ArticleTab></ArticleTab>
      <div class="right-bar">
        <div class="container side-bar">
         <!-- <h5 class="mt-5 "  > Pilih Cover </h5>
         <select v-model="pilih.cover">
            <option disabled value="">Please select one</option>
            <option>Sisipkan</option>
            <option>Import </option>
          </select> 
  <span>Selected: {{ selected }}</span> -->
  <div class="p-4">
    <p class ="side-font" >Pilih Cover</p>
    <select v-model="Selected ">
            <option disabled value="">Please select one </option>
            <option>Sisipkan</option>
            <option>Import </option>
            
          </select> 
          <div> 
        </div>
        <hr>
        <p class ="side-font" >Deskripsi Artikel</p>

        <div class="form-floating">
        <textarea class="side-font" placeholder="Lorem ipsum dolor sit amet consectetur adipisicing elit." id="floatingTextarea2" style="height: 100px"></textarea>
        </div>
    <p style="white-space: pre-line">
        {{ about }}
    </p>
        <p class ="side-font" >Pilih Kategori</p>
        <select v-model="kategori ">
            <option disabled value="">Please select one </option>
            <option>Makanan</option>
            <option>Restoran</option>
            <option>Tempat Wisata</option>
            <option>Taman</option>
            
          </select> 
          <hr />
          <p class ="side-font" >Tag</p>
          <div class="form-floating">
        <textarea class="side-font" placeholder="Lorem ipsum dolor sit amet consectetur adipisicing elit." id="floatingTextarea2" style="height: 100px"></textarea>
        </div>
        <hr />
          
        </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ArticleNavbar from './ArticleNavbar.vue'
import ArticleTab from './ArticleTab.vue'
export default {
  name: 'App',
  components: {
    ArticleNavbar,
    ArticleTab
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.article-page {
  background-color: #309C9F;
  height: 200vh;
  margin: 0;
}

.article {
  border-radius: 50px 0 0 0;
  background: #E5E5E5;
  display: flex;
}

.right-bar {

  border-radius: 50px 0 0 0;
  background: #fff;
  position: relative;
  width: 354px;
height: 1083px;
}

.button-group {
  position: relative;
  top: 10%;
  transform: translateY(50%);
  padding: 20px;
}

.btn {
  padding: 1px 4px;
  margin: 5px;
  border-radius: 100px;
}

.card-side {
  position: absolute;
  width: 340px;
  height: 106px;
  border-radius: 0;
  border: 0 0 1px 1px;
  box-shadow: rgba(0, 0, 0, 0.16) 0px 3px 6px 0px, rgba(0, 0, 0, 0.23) 0px 3px 6px 0px;
}

.card-side-body {
  height: inherit;
}

.preview-pict-side {
position: absolute;
width: 57px;
height: 29px;
margin-right: 5%;
transform: matrix(1, 0, 0, -1, 0, 0);
}


.side-font {
font-family: 'Inter';
font-style: normal;
font-weight: 400;
font-size: 18px;
line-height: 22px;
color : #727272;
}

.floatingTextarea2{
border: 1px solid #727272;
border-radius: 5px;
width: max-width ;
height: 185px;
}

</style>

