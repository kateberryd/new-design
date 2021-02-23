<template>
   <nav class="navbar  justify-content-between ">
       <img class="logo" src="../assets/logo.svg" alt="">
        <form class="form-inline "  >
            <button class="btn btn-outline-primary mr-2" type="submit">Log In</button>
            <button class="btn btn-outline-primary " type="submit">Request Enterprise demo</button>
        </form>
     </nav>
</template>

<script>
export default {
  name: 'Navbar',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    nav{
        margin-top: 20px;
        margin-left: 160px;
        margin-right: 100px;
    }
    .logo{
        width: 120px;
    }

</style>
