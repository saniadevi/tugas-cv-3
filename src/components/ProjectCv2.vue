<template>
<div class="all row">
    <div class="nme">
    <fieldset class="line"><legend>&ensp;RESUME&ensp;</legend></fieldset>
    <h1   v-for="user in dataList" :key="user">{{user.nma0}}<br>{{user.nma1}}</h1>
    </div><br>
    <div class="true">
     <img  src="https://www.drodd.com/images15/1-15.jpg" > 
    <h2 class="app"> BOOTCAMP PARTICIPANTS<hr></h2>
    </div>
<div class="one">
<br>
    
    <h2>PROFILE<hr style="border-top: 1px dashed black;"></h2>
    <p v-for="user in dataList" :key="user"><b>NAME</b><br>{{user.nama}}</p>
    <p v-for="user in dataList" :key="user"><b>DATE OF BIRTH</b><br>{{user.date }}</p>
    <p v-for="user in dataList" :key="user"><b>ADDRESS</b><br>{{user.adres}}</p>
    <p v-for="user in dataList" :key="user"><b>WEBSITE</b><br>{{user.website}}</p><br>
    <h2>AWARDS<hr style="border-top: 1px dashed black;"></h2>
    <p v-for="user in dataList" :key="user"><b>CHARTER AWARD 2012 </b><br> {{user.charter}}</p>
    <p v-for="user in dataList" :key="user"><b>INTERFACE DESIGN 2013 </b><br> {{user.inter}}</p><br>
<h2>CONTACT<hr style="border-top: 1px dashed black;"></h2>
    <p v-for="user in dataList" :key="user"><b>HOME NUMBER&#x260E;&#xFE0F; </b><br> {{user.home}}</p>
    <p v-for="user in dataList" :key="user"><b>PHONE NUMBER&#x1F4DE; </b><br>{{user.phone}}</p>
    <p v-for="user in dataList" :key="user"><b>EMAIL&#x1F4E7; </b><br> {{user.email}}</p><br>
    <div>
<h2>SOCIAL<hr style="border-top: 1px dashed black;"></h2>
    <p><b>TWITTER</b><br>@Azafnia</p>
    <p><b>FACEBOOOK </b><br>Azafnia</p>

 
     </div>
     </div>
     <div class="two">
    
     <div class="satu">
        <h2>&#x1F4BC;WORK EXPERIENCE<hr style="border-top: 1px dashed black;"></h2>

        <div class="row">
  <div class="column1" >
    <h2  v-for="user in dataList" :key="user"><b>{{user.creat0}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.creat1}}</p><br>
    <h2  v-for="user in dataList" :key="user"><b>{{user.creat0}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.creat1}}</p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.creat0}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.creat1}}</p>
  </div>
  
  <div class="column2" >
    <h2  v-for="user in dataList" :key="user"><b>{{user.senior0}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.senior1}}</p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.senior0}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.senior1}}</p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.senior0}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.senior1}}</p>
  </div>
</div>
     </div>
 <br>
<div class="dua">
<h2 >&#x1F4D3;EDUCATION<hr style="border-top: 1px dashed black;"></h2>
  <div class="wor">
  <div class="kolom1" >
    <h2  v-for="user in dataList" :key="user"><b>{{user.educa0}}</b></h2>
        <p  v-for="user in dataList" :key="user">{{user.educa1}}<br></p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.educa0}}</b></h2>
        <p  v-for="user in dataList" :key="user">{{user.educa1}}<br></p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.educa0}}</b></h2>
        <p  v-for="user in dataList" :key="user">{{user.educa1}}<br></p>
  </div>
  
  <div class="kolom2" >
    <h2  v-for="user in dataList" :key="user"><b>{{user.educa2}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.educa3}}</p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.educa2}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.educa3}}</p>
    <h2  v-for="user in dataList" :key="user"><b>{{user.educa2}}</b></h2>
    <p  v-for="user in dataList" :key="user">{{user.educa3}}</p>
  </div>
</div>
     </div>
<div class="tiga">
<div class="sow">
       <h2>SKILLS&#x1F4A1;<hr style="border-top: 1px dashed black;"></h2>
       <div class="san">
       <p><b>PROFESSIONAL SKILLS</b><br>Microsoft Windows&#x26AB;&#x26AB;&#x26AB;&#x26AA;
       <br>Windows&#x26AB;&#x26AB;&#x26AB;&#x26AA; <br>Mac OSX&#x26AB;&#x26AB;&#x26AB;&#x26AA; <br>Data Handling&#x26AB;&#x26AB;&#x26AB;&#x26AA; <br> Record Keeping&#x26AB;&#x26AB;&#x26AB;&#x26AA;<br>Web Skills&#x26AB;&#x26AB;&#x26AB;&#x26AA;</p>
       </div>
       <div class="nia">
       <p><b>PERSONAL SKILLS</b><br>Organisation&#x26AB;&#x26AB;&#x26AB;&#x26AA;&#x26AA;<br>Communication&#x26AB;&#x26AB;&#x26AB;&#x26AA;<br>Time Keeping &#x26AB;&#x26AB;&#x26AB;&#x26AA;<br>Team Player&#x26AB;&#x26AB;&#x26AB;&#x26AA;<br> Commitment&#x26AB;&#x26AB;&#x26AB;&#x26AA;<br>Multitasking&#x26AB;&#x26AB;&#x26AB;&#x26AA;</p>
       </div>

</div>
     </div>   
     </div>
</div>
</template>
<script>
import axios from "axios";
export default {
  data() {
    return {
      dataList: [],
      form: {
        id: '',
        name: ''
      },
      updateSubmit: false
    };
  },
  mounted() {
    this.load();
  },
  methods: {
    load() {
      axios
        .get("http://localhost:3000/dataList")
        .then((res) => {
          this.dataList = res.data;
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
};


</script>
<style scoped> 

.all{ 
    width: 100%;
    margin: auto;
} 
 
.one { 
    border: 1px solid none ; 
    padding: 20px; 
    width: 300px; 
    float: left; 
    height: 100%;
    text-align: right;
    margin-bottom: 100%;
} 
 
.two { 
    padding: 20px; 
    background-color: white; 
    float: left; 
    width: 50%; 
    height: auto; 
     margin-bottom: 30px;
} 
.app {
margin-left: 150px;
}
img {
    border: 8px solid white ;
    border-radius: 100%;
    margin-right: 50px;
    height:120px;
    width:120px;
    margin-top: -80px;
}
 
.satu{ 
  background-color: lightgrey; 
  padding: 15px; 
  height: 300px; 
  font-size: 13px;
} 
.dua {
    background-color: lightgrey; 
  padding: 15px; 
  height: 290px;      
  margin-bottom: 20px;
  font-size: 13px;
}
.tiga {
    background-color: lightgrey; 
  padding: 25px; 
  height: 230px; 
}
h1 {
    border: 1px solid none;
    color: white;
    margin-left: 27%;
    font-family: serif;
}
.line {
border-top: 10px solid white;
border-left: none;
border-right: none;
border-bottom: none;
color: white;
margin-bottom: 10px;

}
.nme {
    background-color: navy;
    padding: 20px;
}
h2 {
margin:auto;
}
.row {
  content: "";
  display: table;
  clear: both;
}
.true {
     border: 1px solid none; 
    width: 670px; 
     margin-left: 16%;
}
.column1 {
  float: left;
  width: 40%;
  padding: 10px;
  height: auto; 
}

.column2 {
  float: left;
  width: 50%;
  padding: 10px;
  height: auto; 
}
.kolom1 {
     float: left;
  width: 40%;
  padding: 10px;
  height: 300px; 
}
.kolom2 {
     float: left;
  width: 40%;
  padding: 10px;
  height: 300px; 
}
.san {
     float: left;
  width: 40%;
  padding: 10px;
  height: 300px; 
}

.nia {
     float: left;
  width: 40%;
  padding: 10px;
  height: 300px; 
}

.container {
    border: 1px solid none;
    padding-right:-20px ;
    height: auto;
}


   
 
</style>