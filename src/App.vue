<template>
  <div id="app">
    <Header></Header>
    <div class="row height-100 overflow-auto">
      <div class="col-md-4 col-sm-12 overflow-auto">
        <Campaign></Campaign>
      </div>
      <div class="col-md-8 col-sm-12 overflow-auto">
        <Message></Message>
      </div>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Campaign from "@/components/Campaign";
import Message from "@/components/Message";
export default {
  name: "App",
  components: {
    Header,
    Campaign,
    Message,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
