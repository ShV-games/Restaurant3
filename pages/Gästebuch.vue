<template>
  <section class = "container">
    
    <h1>Gästebuch</h1>
    <input type="text" name="Name" id="Name" v-model="Name">
    <input type="text" name="Kommentar" id="Kommentar" v-model="comment">
    <input type="submit" @click="onClick">
    <p>Kommentar von {{Name}}: {{comment}}</p>
    
  </section>
  
  
</template>

<script>
export default{
  methods:{
    onClick(){
     this.comment
     this.Name

    }

  },
  data(){
    return{
      comment: "",
      Name: ""
    }
  }
}

</script>