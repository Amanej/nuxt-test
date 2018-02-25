<template>
  <section class="container">
    <div class="about">
      <h1>{{title}} About me</h1>
      <p>Im awesome!</p>
      <span>So are you!</span>
    </div>
  </section>
</template>

<script>
export default {
  asyncData (context) {
    //console.log(context);
    // called every time before loading the component
    return {
      title: context.params.title
    }
  },
}
</script>

<style>
.about {
  text-align: center;
}
</style>
