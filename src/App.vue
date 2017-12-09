<template>
  <div id="app" >
    <div class="head div-center shadow">
        <div class="nav-left"></div>
        <div class="nav-right">
          <a class="nav-item">Home</a>
          <a class="nav-item">bbbbbbbb</a>
        </div>
    </div>
    <div class="profile">
      <div style="margin-top: 5rem">
        <div class="row div-center">
          <div class="col-md-8 col-md-offset-2">
            <img :src="'../static/image/cat.jpg'" class="img-circle center-block">
            <div class="text-center">
              <h1 class="title is-4">Eivense Mou</h1>
              <h2 class="subtitle is-3">Another Nickname Moday</h2>
              <p>A Senior Student learning in Shanghai University
                <br>Major in Computer Science and Technology.
                <br>Prefer Java & Python & Vue & React</p>
            </div>
            <hr>
          </div>
        </div>
      </div>
    </div>
    <div class="main">
      <div class="row div-center">
        <div class="col-md-8 col-md-offset-2">
            <div class="container">
              <div class="box"></div>
              <div class="box"></div>
              <div class="box"></div>
            </div>
          <div class="container">
            <div class="box"></div>
            <div class="box"></div>
            <div class="box"></div>
          </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      msg: 'Moooooday',
      msg1:"Every Day is Moday",
      msg2:""
    }
  },
    methods:{

    },
    beforeCreate:function () {
        let url="http://45.77.120.135/test?name=vue";
        let self=this;
//        fetch(url).then(function (response) {
//            return response.json();
//        }).then(function (data) {
//            self.msg2=data;
//            console.log(data);
//        })
    }
}

</script>

<style>
  .profile{
    padding: 20px  50px 15px 50px;
  }
  .head{
    height: 52px;
    width:1400px;
    display: flex;
  }
  p{
    margin: 2rem;
  }
  .main{
    padding: 15px  50px 15px 50px;
  }
  .box{
    height:220px;
    width: 300px;
    border-radius: 5px;
    color:#7a7a7a;
    box-shadow: 0 2px 1px #7a7a7a,0 0 0 1px #7a7a7a;
    border: 1px solid #7a7a7a;
    margin: auto;
  }

</style>