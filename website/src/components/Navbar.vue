<template>
  <header>
    <div id="nav" :class="[isSticky? stickyClass: '']">
        <div>
          <router-link to="/">
            <img src="../assets/images/logo_transparent.png" alt="Dejie Logo" class="logo">
          </router-link> 
        </div>
        <div>
          <router-link to="/about">
            <span>About</span>
          </router-link>
        </div>
    </div>
  
  </header>

</template>

<script>
export default{
    name: "Navbar",
    data(){
      return {
        isSticky: true,
        stickyClass: 'is_sticky'
      }
    },
    created(){
      window.addEventListener('scroll', this.handleScroll);
    },
    destroyed(){
      window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
      handleScroll(){
        let header = document.querySelector('body');
        let windowPos = window.scrollY > 175;
        header.classList.toggle('scrolling-active', windowPos);
   
      }
    }
}
</script>

<style lang="scss">
.logo{
    width: 5rem;
    height: auto;
}
#nav {
  padding: 1rem 3rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  align-content: center;
}

#nav a {
  font-weight: bold;
  color: black;
}

#nav a.router-link-exact-active {
  color: #42b983!important;
}

#nav.is_sticky {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 1030;
  -webkit-animation: .95s ease-in-out 0s normal none 1 running fadeInDown;
  animation: .95s ease-in-out 0s normal none 1 running fadeInDown;
  -webkit-transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
  transition: all 0.3s cubic-bezier(0.645, 0.045, 0.355, 1);
}

/* After Scroll */

.scrolling-active{
  background: black;
  color:white;
  box-shadow: 0 3px 1rem rgba(0,0,0,.1);
  transition: 1s;
  .intro-container{
    opacity: .5;
  }
  #nav a{
    color: white;
  }
}


</style>


