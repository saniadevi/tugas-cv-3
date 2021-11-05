<template>
<div class="all row">
<div class="one">
    <H1 v-for="row in agenda" :key="row" style="font-family:'Crimson Text';">{{row.name}} <br><span> {{row.name2}}</span> </H1><br>
    <img  src="https://4.bp.blogspot.com/-FOZ-RymNN8c/UQKamE83EGI/AAAAAAAARkk/zhuVK94iW1k/s1600/Lonely+Tree+Paography+Wallpapers+07.jpg" height="135px" width="255px ">
    <h2>Contact<hr></h2>
    <p v-for="row in agenda" :key="row"><b>Address:{{ row.addres }}</b><br<br></p>
    <p v-for="row in agenda" :key="row"><b>Phone:{{ row.phone }}</b><br></p>
    <p v-for="row in agenda" :key="row"><b>Email:{{ row.email }}</b><br><u></u></p><br>
    <h2>Languages</h2><hr>
    <p v-for="row in agenda" :key="row">{{row.bhs0}} <br>
    {{row.bhs1}} <br>
    {{row.bhs2}}</p>
    <h2>Hobbies<hr></h2>
    <ul>
        <li v-for="row in agenda" :key="row">{{row.hobi0}}</li>
        <li v-for="row in agenda" :key="row">{{row.hobi1}}</li>
        <li v-for="row in agenda" :key="row">{{row.hobi2}}</li>
    </ul>
    </div>
<div class="two">
    
  <h2>Summary<hr></h2>
  <p v-for="row in agenda" :key="row">{{row.summary0}}<br>{{row.summary1}}<br>{{row.summary2}} <br>{{row.summary3}}<br>{{row.summary4}}</p><br>
  
  <h2>Skill Highlights<hr></h2>
  <ul>
      <li v-for="row in agenda" :key="row">{{row.skil0}}</li>
      <li v-for="row in agenda" :key="row">{{row.skil1}}</li>
      <li v-for="row in agenda" :key="row">{{row.skil2}}</li>
  </ul>

<h2>Experince <hr></h2>
<p v-for="row in agenda" :key="row"><b>{{row.experince0}}</b>  {{row.experince1}} <br>
<b>{{row.experince2}}</b>{{row.experince3}}</p>
<ul>
    <li v-for="row in agenda" :key="row">{{row.experince4}}</li>
    <li v-for="row in agenda" :key="row">{{row.experince5}}</li>
    <li v-for="row in agenda" :key="row">{{row.experince6}}</li>
</ul>

<h2>Education<hr></h2>
<ul>
    <li v-for="row in agenda" :key="row">{{row.education0}}</li>
    <li v-for="row in agenda" :key="row">{{row.education1}}</li>
    <li v-for="row in agenda" :key="row">{{row.education2}}</li>
</ul>

<h2>Certifications<hr></h2>
<p v-for="row in agenda" :key="row">{{row.certi0}}<b>{{row.certi1}} </b><br>
 {{row.certi2}} <b>{{row.certi3}} </b></p>
</div>
</div>

</template>
<script>
import axios from "axios";
export default {
  data() {
    return {
      agenda: [],
      form: {
        id: '',
        name: ''
      },
    };
  },
  mounted() {
    this.load();
  },
  methods: {
    load() {
      axios
        .get("http://localhost:3000/users")
        .then((res) => {
          this.agenda = res.data;
        })
        .catch((err) => {
          console.log(err);
        });
    },
  },
};


</script>
<style scoped>

.one {
    border: 1px solid none;
    background-color: lightgray;
    padding: 40px;
    float: left;
  width: 25%;
  height: 848px; 
  padding: 20px;
text-align: justify;  

}
span {
    color: red;
}
h2 {
    font-family: georgia;
}
hr {
    color: black;
}
.two {
    padding: 20px;
    background-color: grey;
    float: left;
    width:41%;
    height: 850px;
    margin-bottom: 30px;
}
.all {
    margin-left: 320px;
    margin-top: 30px;

}
.row:after {
  content: "";
  display: table;
  clear: both;
}

</style>