<template>
  <div id="app">
    
      <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="d-flex flex-grow-1">
        <span class="w-100 d-lg-none d-block"><!-- hidden spacer to center brand on mobile --></span>
        
      <a class="navbar-brand" href="#">
        <div>
          <b-img class="nav-img" src="spa.png"  fluid alt="Responsive image"></b-img>
          <p class="domain">Spabooking.in</p>
        </div>
        </a>
        <div class="w-100 text-right">
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#myNavbar7">
                <span class="navbar-toggler-icon"></span>
            </button>
        </div>
    </div>
    <div class="collapse navbar-collapse flex-grow-1 text-right" id="myNavbar7">
        <ul class="navbar-nav ml-auto flex-nowrap">
            <li class="nav-item">
              <div>
          <!--   <b-img height="auto" width=".1em" src="spa.png"></b-img>-->
              </div>
                <router-link to="/" >Home</router-link>
            </li>
            <li class="nav-item">
                 <router-link to="/Cats">Cats </router-link>
            </li>
            <li class="nav-item">
                <router-link to="/Dogs">Dogs </router-link>
            </li>
            <li class="nav-item">
                <router-link to="#">FAQs </router-link>
            </li>
            <li class="nav-item">
                <b-img class="notification" src="notification.png" fluid alt="Notification"></b-img>
            </li>
            <li class="nav-item">
                <b-button pill variant="warning"  size="sm">
                  <span class="login-text">Login</span>
                  </b-button>
            </li>
        </ul>
    </div>
</nav>
    
    <router-view/>
   
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.navbar{
  
  padding: 60px;
  background-image: linear-gradient( rgba(29,11,0,1), rgb(53,21,22));
  a {
    font-weight: bold;
    color: rgb(253, 191, 20);
    font-family: 'Roboto', sans-serif;
    font-weight: lighter;
  }
}
a:hover{
  color:#fdbf14;
}

.nav-item{
padding-right: 3em
}
.nav-img{
  height: auto;
  width: 1.5em;
}
.domain{
  font-size:.875em;

  font-weight:500;
   font-family: "Comfortaa", cursive;
   font-weight:normal;
   color: #fdbf14;
   margin:0em;
}
.login-text{
  font-size: .875em;
padding-left: 1em;
padding-right: 1em;
}
.notification{
  height: auto;
  width: 1.4em;
}
</style>
