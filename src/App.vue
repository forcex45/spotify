<template>
  <div id="app">
    <div class="nav">
       <ul style="list-style-type: none">
         <li> <a href="#"><button><i class="fas fa-home"></i> Home</button></a></li>
         <li> <a href="#"><button><i class="fal fa-search"></i> Search</button></a></li>
         <li> <a href="#"><button><i class="fad fa-books"></i> Library</button></a></li>
       </ul>
      <div class="çizgi"></div>
      <div class="box">
        <a href="#"><i style="color: white" class="fas fa-plus"></i>&#160;Create Playlist</a>
        <a id="a" href="#"><i style="color: white" class="fas fa-heart"></i>&#160;Liked Songs</a>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<style>
body {
  color: white;
  margin: 0;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
}

.çizgi {
  border-bottom: 1px solid #1f1e1e;
}

.nav {
  top: 0;
  width: 14em;
  height: 100%;
  position: fixed;
  background-color: black;
}

.nav ul li a {
  display: flex;
  justify-content: flex-start;
  font-size: 27px;
  text-decoration: none;
  color:white;
 }

.nav ul  {
  margin-left: -23%;
  margin-top: 50%;
}

.nav > ul > li > a > button {
  font-size: 21px;
  width: 90%;
  height: 4rem;
  background-color: black;
  border: none;
  color:#bcbcbc;
  transition: color 0.8s;
}
.nav > ul > li > a > button:hover {
  color:white;
}
.nav > ul > li > a > button:focus {
  background-color: #2d2b2b;
  border-radius: 3%;
  color:white;
}

.box a {
  color:#bcbcbc;
  display: flex;
  justify-content: center;
  font-size: 20px;
  text-decoration: none;
  margin-left: -1%;
  margin-top:7%;
  transition: color 0.8s;
}

#a {
  margin-left: -8%;
}

.box a:hover {
  color:white;
}
</style>a
