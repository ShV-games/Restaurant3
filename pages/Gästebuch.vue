<template>
  <section class = "container">
    
    <h1>Gästebuch</h1>
    <input type="text" name="Name" id="Name" v-model="Name" placeholder="Ihr Name">
    <input type="text" name="Kommentar" id="Kommentar" v-model="comment" placeholder="Kommentar">
    <input type="submit" @click="onClick">
    <p v-for="Eintrag in arr">Kommentar von {{Eintrag.gesName}}: {{Eintrag.gesComment}}</p>
    
  </section>
  
  
</template>

<script>
export default{
  methods:{
    onClick(){
     this.gesComment=this.comment;
     this.gesName= this.Name;



    this.arr.push ({gesComment: this.gesComment, gesName: this.gesName});
    console.log(this.arr);
    }

  },
  data(){
    return{
      comment: "",
      Name: "",
      gesName:"",
      gesComment:"",
      arr: []
    }
  }
}

</script>