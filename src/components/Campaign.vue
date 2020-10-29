<template>
  <div id="campaign">
    <div>
      <h5 class="campaign-title">Campaña</h5>
    </div>
    <form>
      <div class="row">
        <div class="col-8">
          <label>Nombre</label>
          <select class="form-control" placeholder="Selecciona una opcion">
            <option selected>Choose</option>
          </select>
        </div>
        <div class="col-4" style="align-self: flex-end">
          <button class="btn-created">Crear</button>
        </div>
      </div>
      <div class="row">
        <div class="col-12">
          <label> Destinatarios</label>
          <div class="box">
            <p>¡Sin Destinatarios!</p>
            <p style="text-align: center; font-size: 14px">
              Agregalos para habilitar las funcionalidades que hacen uso de los
              campos destinatarios.
            </p>
            <input type="file" hidden />
            <button class="upload-file">Cargar archivo</button>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-12">
          <label for="inputEmail4"
            >Guardar Campos
            <span style="font-size: 10px; align-self: center">(opcional)</span>
          </label>
          <select class="form-control" placeholder="Selecciona una opcion">
            <option selected>Choose</option>
          </select>
          <span
            style="
              font-size: 10px;
              text-align: start;
              display: flex;
              margin-top: 8px;
            "
          >
            Para hacer uso de este campo carga tus destinatarios.</span
          >
        </div>
      </div>
      <div style="border-bottom: 1px solid; margin-top: 30px"></div>
    </form>
    <div class="row" style="margin-top: 10px">
      <div class="col-12" style="display: flex; justify-content: space-between">
        <label style="margin: inherit"> Configuraciones </label>
        <button class="btn-edit">Editar</button>
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <label> Validar numeros repetidos</label>
        <p style="text-align: start">No</p>
      </div>
      <div class="col-12">
        <label> Enviar codigo aletorio</label>
        <p style="text-align: start">No</p>
      </div>
      <div class="col-12">
        <label> Enviar campañas por bloques</label>
        <p style="text-align: start">No</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Campaign",
};
</script>
<style scoped>
.btn-edit {
  background: #fff;
  border: 1px solid #1b9cf5;
  color: #1b9cf5;
  border-radius: 3px;
  min-width: 30%;
}
.upload-file {
  background: #fff;
  border: 1px solid #d3d5e2;
  border-radius: 3px;
  padding: 5px;
  min-width: 60%;
  color: #3c3f4a;
}
.row {
  margin-bottom: 10px;
}
.btn-created {
  background: #fff;
  color: #192354;
  border: 1px solid #192354;
  display: inline;
  border-radius: 3px;
  width: 100%;
  height: 35px;
}
select {
  height: 35px;
}
label {
  display: flex;
  font-weight: bold;
  font-family: Arial, Helvetica, sans-serif;
}
#campaign {
  padding: 15px;
}
.campaign-title {
  color: #192354;
  text-align: start;
}
</style>