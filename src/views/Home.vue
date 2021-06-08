<template>
  <div class="home">
    <div class="go">
      <div class="back">
        <a href="#"><i class="fas fa-angle-left"></i></a>
      </div>
      <div class="forward">
        <a href="#"><i class="fas fa-angle-right"></i></a>
      </div>
    </div>
    <div class="account">
      <p>Forcex</p>
     <div class="avatar-box">
       <div class="avatar"><img width="30px" src="../assets/logo.png"></div>
     </div>
    </div>
    <div class="body">
      <b>Made for Forcex
      </b>
      <p>Get better recommendations the more you listen.
      </p>
    </div>
    <div class="music-box">
        <div v-for="item in musics" :key="item" class="music">
          <div class="music-image">
            <img :src="item.image">
          </div>
          <div style="margin-top: 2%" class="çizgi"></div>
          <h3>{{ item.name}}</h3>
          <p class="author">{{item.author}}</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      musics: [
        {
          name: "Wondress",
          image: "https://cdn.discordapp.com/attachments/824240985320062996/851838153966223360/iu.png",
          author: "Forcex"
        },
        {
          name: "Forcex",
          image: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.prO6dWvomYyK1881o-qn6wHaEK%26pid%3DApi&f=1",
          author: "Bille Ellish"
        },
        {
          name: "BibPob",
          image: "https://cdn.discordapp.com/attachments/824240985320062996/851838153966223360/iu.png",
          author: "NoName"
        },
        {
          name: "Biliyom",
          image: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse3.mm.bing.net%2Fth%3Fid%3DOIP.prO6dWvomYyK1881o-qn6wHaEK%26pid%3DApi&f=1",
          author: "Enes Batur"
        },
        {
          name: "NoName",
          image: "https://cdn.discordapp.com/attachments/824240985320062996/851839151652864000/iu.png",
          author: "No Name"
        }
      ]
    }
  }
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@200&display=swap');
 .go {
   width: 2.6rem;
   height: 2.4rem;
   background-color: black;
   margin-left: 19%;
   margin-top: 1%;
   border-radius: 30px;
 }

 .go > .back > a {
   text-decoration: none;
   color: #bcbcbc;
   font-size: 34px;
   display: flex;
   justify-content: center;
   transition: color 0.7s;
 }

 .go > .back > a >i  {
   margin-top: 9% !important;
 }

 .go > .back > a:hover {
   color:white;
 }

.forward > a {
   border-radius: 30px;
   background-color: black;
   text-decoration: none;
   color: #bcbcbc;
   font-size: 33px;
   display: flex;
   justify-content: center;
   transition: color 0.7s;
   margin-top: 19%;
 }

.forward > a > i {
   margin-top: 7% !important;
 }

 .forward > a:hover {
   color:white;
 }

 .account {
   width: 8.7rem;
   height: 2.2rem;
   background-color: #000000;
   margin-left: 87%;
   margin-top: -3%;
   border-radius: 30px;
 }

 .account > p {
   text-align: center;
   padding: 7px 60px;
   font-size: 18px;
 }

 .avatar-box {
   margin-top: -37.6%;
   margin-left: 2%;
   width: 2.6rem;
   height: 2.0rem;
   border-radius: 50px;
   background-color: #292727;
 }

 .avatar > img{
   margin-top: 8%;
   margin-left: 15%;
 }

 .body {
   margin-left: 18%;
   margin-top: 7%;
 }

 .body > b {
   font-size: 30px;
 }

 .body > p {
   font-size: 17px;
   font-family: 'Source Sans Pro', sans-serif;
   margin-top: 0%;
 }

 .music-box {
   margin-left: 18%;
   margin-top: 2%;
 }

 .music-box > .music {
   width: 12rem;
   height: 16rem;
   background-color: black;
   display: inline-block;
   margin: 1%;
   border-radius: 3px;
 }

 .music > h3 {
   margin-left:6%;
   margin-top: 9%;
   font-size: 18px;
 }

.music:hover {
  transition: 0.7s;
  transform: translate(-0%,-3%);
}

.music-image {
  margin-left: 8.7%;
  margin-top: 6%;
}

.music-image > img {
  border-radius: 3px;
  width: 160px;
  height: 140px;
}

.author {
  margin-left: 6% !important;
  font-size: 14px;
}
</style>
