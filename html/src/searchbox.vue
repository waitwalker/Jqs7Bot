<template lang='jade'>
input(type='text' @keydown.enter='submit')
</template>

<script>
export default{
  methods:{
    submit(event){
      let v = event.target.value.trim();
      if (v !== ''){
        window.location.href = '/user/' + v;
      }
    }
  }
}
</script>
