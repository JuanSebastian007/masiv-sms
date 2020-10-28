<template>
  <div class="header">
    <div
      class="row"
      style="padding: 15px; margin: inherit; background: #fff; height: 50px"
    >
      <div class="col-6 text-left" style="align-self: center">
        <h6 style="margin: inherit">SMS > Envios masivos > Enviar</h6>
      </div>
      <div class="col-6">
        <div class="row" style="justify-content: flex-end">
          <div class="col-1 question">
            <svg
              width="1em"
              height="1em"
              viewBox="0 0 16 16"
              class="bi bi-question-circle"
              fill="currentColor"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                d="M8 15A7 7 0 1 0 8 1a7 7 0 0 0 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
              />
              <path
                d="M5.255 5.786a.237.237 0 0 0 .241.247h.825c.138 0 .248-.113.266-.25.09-.656.54-1.134 1.342-1.134.686 0 1.314.343 1.314 1.168 0 .635-.374.927-.965 1.371-.673.489-1.206 1.06-1.168 1.987l.003.217a.25.25 0 0 0 .25.246h.811a.25.25 0 0 0 .25-.25v-.105c0-.718.273-.927 1.01-1.486.609-.463 1.244-.977 1.244-2.056 0-1.511-1.276-2.241-2.673-2.241-1.267 0-2.655.59-2.75 2.286zm1.557 5.763c0 .533.425.927 1.01.927.609 0 1.028-.394 1.028-.927 0-.552-.42-.94-1.029-.94-.584 0-1.009.388-1.009.94z"
              />
            </svg>
          </div>
          <div class="col-1 dialog">
            <svg
              width="1em"
              height="1em"
              viewBox="0 0 16 16"
              class="bi bi-chat-square"
              fill="currentColor"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                d="M14 1H2a1 1 0 0 0-1 1v8a1 1 0 0 0 1 1h2.5a2 2 0 0 1 1.6.8L8 14.333 9.9 11.8a2 2 0 0 1 1.6-.8H14a1 1 0 0 0 1-1V2a1 1 0 0 0-1-1zM2 0a2 2 0 0 0-2 2v8a2 2 0 0 0 2 2h2.5a1 1 0 0 1 .8.4l1.9 2.533a1 1 0 0 0 1.6 0l1.9-2.533a1 1 0 0 1 .8-.4H14a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"
              />
            </svg>
          </div>
          <div class="col-4" style="">
            <div class="dropdown">
              <button
                class="dropdown-toggle estratec-btn"
                type="button"
                id="dropdownEstratec"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >
                <div id="circulo">
                  <p>E</p>
                </div>
                <p>Estratec</p>
              </button>
              <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
                <a class="dropdown-item" href="#">Cambiar contraseña</a>
                <a class="dropdown-item" href="#">Salir</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div
      class="row"
      style="padding: 15px; margin: inherit; background: #333; height: 50px"
    >
      <div class="col-9" style="text-align: start">
        <button class="btn-enviar">Enviar</button>
      </div>
      <div class="col-3" style="display: flex; justify-content: space-between">
        <button class="btn-sms">SMS V3</button>
        <div class="dropdown">
          <button
            class="dropdown-toggle btn-enviar-dropdown"
            type="button"
            id="dropdownEnviar"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          >
            Enviar
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Header",
  props: {},
};
</script>
<style scoped>
.question,
.dialog {
  max-width: 50px;
  cursor: pointer;
}
.question:hover,
.dialog:hover {
  background: #e7e7e7;
}
.btn-enviar-dropdown {
  background: #01c787;
  color: #fff;
  border: 1px solid #01c787;
  min-width: 100px;
  border-radius: 3px;
}
.btn-enviar-dropdown:hover {
  background: #06ac69;
}
.btn-sms {
  background: #fff;
  color: #01c787;
  border: 1px solid #01c787;
  min-width: 100px;
  border-radius: 3px;
}
.btn-sms:hover {
  background: #06ac69;
  color: #fff;
}
.btn-enviar {
  background: transparent;
  color: white;
  border: inherit;
}
.estratec-btn {
  display: flex;
  min-width: 140px;
  justify-content: space-between;
  background: transparent;
  border: inherit;
  align-items: center;
}
.estratec-btn:hover {
  background: #e7e7e7;
}
.dropdown-toggle:after {
  color: #7777;
  align-self: center;
}
#circulo {
  width: 25px;
  height: 25px;
  border-radius: 50%;
  background: green;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
#circulo > p {
  color: white;
  font-size: 14px;
  margin: inherit;
}
h6 {
  font-size: 14px;
}
p {
  margin: inherit;
}
</style>