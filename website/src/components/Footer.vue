<template>
<div>
 <footer class="footer">
        <div class="footer-left">© 2021 Dejie Zhen</div>
        <div class="footer-right">
            <a target='_blank' href="https://www.linkedin.com/in/dejie-zhen/"><i class="fab fa-linkedin-in"></i></a>
            <a target='_blank' href="https://github.com/dejiezhen"><i class="fab fa-github"></i></a>
        </div>
    </footer>
</div>
   
</template>

<style lang="scss">
.footer{
    display: flex;
    justify-content: space-between;
    background-color: rgb(87, 87, 87);
    align-items: center;
    .footer-left, .footer-right{
        padding: 1rem 3rem;
    }
    .footer-right i{
        margin-right: 1.5rem;
        font-size: 1.5rem;
        color: white;
    }
}

@media only screen 
  and (min-device-width: 375px) 
  and (max-device-width: 812px) 
  and (-webkit-min-device-pixel-ratio: 3) { 
      .footer{
          flex-direction: column;
      }



  }

</style>