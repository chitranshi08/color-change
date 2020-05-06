<template>
  <div>
   {{message}} i am {{form}}
   <input type="text" v-model="message">
   <button @click="getMessage">Click</button>

</div>
</template>

<script>
export default {
  name: 'ProductOne',
  data:()=>({
    message:null,
    inputText:null,
    form:"charu"
  }),
  methods:{
    getMessage(){
      this.message = this.inputText
      this.inputText = null
    }
  }
  
}
</script>

<style scoped>



</style>
