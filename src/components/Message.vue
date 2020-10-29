<template>
  <div id="message">
    <div>
      <div class="row" style="justify-content: space-evenly">
        <div class="col-6" style="font-size: 20px; text-align: left">
          Mensaje
        </div>
        <div class="col-6" style="display: flex; justify-content: flex-end">
          <button class="btn-test">Probar</button>
        </div>
      </div>
      <div class="container-fluid box-message">
        <TextSMS></TextSMS>
      </div>
      <!--  -->
    </div>
  </div>
</template>
<script>
import TextSMS from "@/components/TextSMS";
export default {
  name: "message",
  components: {
    TextSMS,
  },
};
</script>
<style scoped>
.box-message {
  background: rgb(221, 221, 221);
  margin-top: 15px;
  border-radius: 5px;
  padding: 20px 15px;
  border: 1px solid #333;
}
.btn-test {
  background: #fff;
  color: #192354;
  border: 1px solid #192354;
  display: inline;
  border-radius: 3px;
  width: 40%;
  height: 35px;
}
#message {
  padding: 15px 25px 15px 0px;
  background: #fff;
}
</style>