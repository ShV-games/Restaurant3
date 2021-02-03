<template>
  <section class = "container">
    
    <h1>Bestellen</h1>
    <p1><img src="~assets/Bilder/Essen.jpg" alt="Leonardo" class="image" width="520" height="400"><input type="submit" @click="Spagethis"></p1>
    <p2><img src="~assets/Bilder/Downlad.jpg" alt="Leonardo" class="image" width="520" height="400"><input type="submit" @click="Pizzen"></p2>

    <h2>Ihre Bestellungen:</h2>
    <p v-for="Eintrag in arr">{{Eintrag.gesSpagethi}}</p>
    <p v-for="Eintrag in arr">{{Eintrag.gesPizza}}</p> 



    
  </section>
  
  
</template>

<script>
export default{
  methods:{
    Spagethis(){

     this.gesSpagethi= this.Spagethi;



    this.arr.push ({gesSpagethi: this.gesSpagethi});
    console.log(this.arr);
    },
    Pizzen(){
        this.gesPizza=this.Pizza;
        this.arr.push({gesPizza: this.gesPizza})

    }


  },
  data(){
    return{
      Pizza: "Pizza",
      Spagethi: "Spaghetti",
      gesSpagethi:"",
      gesPizza:"",
      arr: []
    }
  }
}

</script>