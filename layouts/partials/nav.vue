<template>
    <header>

        <nuxt-link to="/" class="logo"></nuxt-link>
        <nav>
        <ul>
            <li><nuxt-link to="/">Home</nuxt-link></li>
             <li><nuxt-link to="Kontakt">Kontakt</nuxt-link></li>
            <li><nuxt-link to="Historie">Historie</nuxt-link></li>
        </ul>
    </nav>
    </header>

</template>

<script>
export default {
    name: "nav",
   
}
</script>

<style>
      header{
          background: rgb(243, 240, 90);
          display: grid;
          grid-template-columns: repeat(2,auto);
      }
      .logo, li a{
          padding: 1em 2em;
          display: block;
          text-transform: uppercase;
          text-decoration: none;
          font-weight: bold;
          color:rgb(0, 0, 0);
          font-size: .9em;
      }

      nav{
          justify-self: right;
      }
      ul{
          list-style-type: none;
      }
      li{
          display: inline;
      }
      li a{
          padding: 1em 2em;
          display: inline-block;
          background: rgba(20, 20, 20, 0.027);
      }
</style>