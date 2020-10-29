<template>
  <div id="textSMS">
    <div class="row">
      <div class="col-md-9" style="text-align: left">
        <label style="font-weight: bold"> Texto </label>
        <div style="display: flex">
          <select class="form-control" style="width: 30%">
            <option selected>Choose...</option>
            <option>...</option>
          </select>
          <button class="btn-tools">
            <svg
              width="1em"
              height="1em"
              viewBox="0 0 16 16"
              class="bi bi-calendar"
              fill="currentColor"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                d="M3.5 0a.5.5 0 0 1 .5.5V1h8V.5a.5.5 0 0 1 1 0V1h1a2 2 0 0 1 2 2v11a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V3a2 2 0 0 1 2-2h1V.5a.5.5 0 0 1 .5-.5zM1 4v10a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V4H1z"
              />
            </svg>
          </button>
          <button class="btn-tools">
            <svg
              width="1em"
              height="1em"
              viewBox="0 0 16 16"
              class="bi bi-link-45deg"
              fill="currentColor"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M4.715 6.542L3.343 7.914a3 3 0 1 0 4.243 4.243l1.828-1.829A3 3 0 0 0 8.586 5.5L8 6.086a1.001 1.001 0 0 0-.154.199 2 2 0 0 1 .861 3.337L6.88 11.45a2 2 0 1 1-2.83-2.83l.793-.792a4.018 4.018 0 0 1-.128-1.287z"
              />
              <path
                d="M6.586 4.672A3 3 0 0 0 7.414 9.5l.775-.776a2 2 0 0 1-.896-3.346L9.12 3.55a2 2 0 0 1 2.83 2.83l-.793.792c.112.42.155.855.128 1.287l1.372-1.372a3 3 0 0 0-4.243-4.243L6.586 4.672z"
              />
            </svg>
          </button>
        </div>
        <div>
          <textarea> </textarea>
        </div>
        <div style="text-align: end">
          <label> Caracteres: 0/160 </label>
        </div>
      </div>
      <!--  -->
      <div class="col-md-3">
        <label style="display: flex"> Tipo</label>
        <div class="form-check">
          <input class="form-check-input" type="radio" />
          <label class="form-check-label" for="inlineRadio1">Estandar</label>
        </div>
        <div class="form-check">
          <input class="form-check-input" type="radio" />
          <label class="form-check-label" for="inlineRadio1">Flash</label>
        </div>
        <!--  -->
        <label style="display: flex"> Formato</label>
        <div class="form-check">
          <input class="form-check-input" type="radio" />
          <label class="form-check-label" for="inlineRadio1">Corto</label>
          <p style="font-size: 10px">Máx. Caracteres 600</p>
        </div>
        <div class="form-check">
          <input class="form-check-input" type="radio" />
          <label class="form-check-label" for="inlineRadio1">Largo</label>
          <p>Máx. Caracteres: 600</p>
          <p>Perú: 400</p>
        </div>
        <div class="form-check">
          <input class="form-check-input" type="radio" />
          <label class="form-check-label" for="inlineRadio1"
            >Premium (Texto enriquecido)</label
          >
          <p>Emojis: máx. caracteres: 600. Peru: 400</p>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
p {
  font-size: 10px;
  text-align: left;
  margin: inherit;
}
.form-check-label {
  display: flex;
  text-align: left;
}
.form-check-input {
  display: flex;
  align-self: left;
}
.btn-tools {
  border: inherit;
  background: transparent;
}
textarea {
  background: white;
  width: 100%;
  height: 400px;
  border: 1px solid #333;
  border-radius: 5px;
}
.box-message {
  background: rgb(221, 221, 221);
  margin-top: 15px;
  border-radius: 5px;
  padding: 20px 15px;
  border: 1px solid #333;
}
</style>