<template>
  <div id="app" >
    <div class="head shadow">
      <div class="container">
        <div class="nav"></div>
      </div>
    </div>
    <div class="profile">
      <div style="margin-top: 8rem">
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
    padding: 50px;
  }
  .head{
    height: 52px;
  }
  .div-center{
    margin:auto;
  }
  p{
    margin: 2rem;
  }

</style>