<template>
  <div class="container">
      <div class="image-container">
          <img alt="car" src="../assets/car.png" class="fixed-margin header-car">
      </div>
      <div class="bg-light pt-5 pb-5">
            <b-container class="pl-5 pr-5">
                <b-row>
                    <b-col sm="12" md="6">
                        <b-form-group id="input-group-3" label="Modelo" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-select
                            id="input-3"
                            v-model="form.model"
                            :options="models"
                            required
                            ></b-form-select>
                        </b-form-group>
                    </b-col>
                    <b-col sm="12" md="6">
                        <b-form-group id="input-group-3" label="Versión" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-select
                            id="input-3"
                            v-model="form.version"
                            :options="versions"
                            required
                            ></b-form-select>
                        </b-form-group>
                    </b-col>
                </b-row>
                <b-row>
                    <b-col sm="12" md="6">
                        <b-form-group id="input-group-3" label="Estado" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-select
                            id="input-3"
                            v-model="form.state"
                            :options="states"
                            required
                            ></b-form-select>
                        </b-form-group>
                    </b-col>
                    <b-col sm="12" md="6">
                        <b-form-group id="input-group-3" label="Distribuidor" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-select
                            id="input-3"
                            v-model="form.distributor"
                            :options="distributors"
                            required
                            ></b-form-select>
                        </b-form-group>
                    </b-col>
                </b-row>
                    <h1 class="section-title">
                        Datos personales
                    </h1>
                    <h6 class="section-subtitle">
                        Escribe tus datos personales
                    </h6>
                <b-row class="mt-5">
                    <b-col sm="12" md="4">
                        <b-form-group id="input-group-3" label="Nombre (s)" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-input
                            id="input-1"
                            v-model="form.name"
                            type="email"
                            placeholder="Escribe tu nombre"
                            required
                            ></b-form-input>
                        </b-form-group>
                    </b-col>
                    <b-col sm="12" md="4">
                        <b-form-group id="input-group-3" label="Apellido Paterno"
                        label-for="input-3"
                        class="text-left custom-label">
                            <b-form-input
                            id="input-1"
                            v-model="form.lastnamefather"
                            type="email"
                            placeholder="Escribe tu apellido"
                            required
                            ></b-form-input>
                        </b-form-group>
                    </b-col>
                    <b-col sm="12" md="4">
                        <b-form-group id="input-group-3" label="Apellido Materno"
                        label-for="input-3"
                        class="text-left custom-label">
                            <b-form-input
                            id="input-1"
                            v-model="form.lastnamemother"
                            type="email"
                            placeholder="Escribe tu apellido"
                            required
                            ></b-form-input>
                        </b-form-group>
                    </b-col>
                </b-row>
                <b-row class="mt-4">
                    <b-col sm="12" md="4">
                        <b-form-group id="input-group-3" label="Email" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-input
                            id="input-1"
                            v-model="form.email"
                            type="email"
                            placeholder="Correo@email.com.mx"
                            required
                            ></b-form-input>
                        </b-form-group>
                    </b-col>
                    <b-col sm="12" md="4">
                        <b-form-group id="input-group-3" label="Teléfono" label-for="input-3"
                        class="text-left custom-label">
                            <b-form-input
                            id="input-1"
                            v-model="form.phone"
                            placeholder="018444390654"
                            required
                            ></b-form-input>
                        </b-form-group>
                    </b-col>
                </b-row>
                <b-row class="mt-5">
                    <b-col>
                        <b-form-group id="input-group-3" label="Deseo ser contactado por"
                        label-for="input-3" class="text-left custom-label">
                            <b-button-group class="w-100">
                                <b-button class="btn-custom">
                                    <b-icon icon="telephone-fill" class="align-middle"
                                    style="width: 0.85rem; height: 0.85rem"></b-icon>
                                    Teléfono
                                </b-button>
                                <b-button class="btn-custom">
                                    <b-icon icon="envelope-fill" class="align-middle"
                                    style="width: 0.85rem; height: 0.85rem"></b-icon>
                                    Email
                                </b-button>
                                <b-button class="btn-custom">Ambos</b-button>
                            </b-button-group>
                        </b-form-group>
                    </b-col>
                </b-row>
                    <h1 class="section-title">
                        Forma de pago
                    </h1>
                    <h6 class="section-subtitle">
                        Personaliza tu cotización
                    </h6>
                <b-row>
                    <b-container class="w-75 mt-4">
                        <b-row>
                            <b-col>
                                <b-form-group id="input-group-3" label="Elige tu tipo de pago"
                                label-for="input-3" class="text-left custom-label">
                                    <b-button-group class="w-100">
                                        <b-button class="btn-custom">
                                            Contado
                                        </b-button>
                                        <b-button class="btn-custom">
                                            Crédito
                                        </b-button>
                                    </b-button-group>
                                </b-form-group>
                            </b-col>
                        </b-row>
                        <b-row>
                            <b-col sm="12" md="6">
                                <b-form-group id="input-group-3" label="Cantidad de enganche"
                                label-for="input-3" class="text-left custom-label">
                                    <b-form-input
                                    id="input-1"
                                    v-model="form.amount"
                                    type="text"
                                    placeholder="Correo@email.com.mx"
                                    required
                                    ></b-form-input>
                                </b-form-group>
                            </b-col>
                            <b-col sm="12" md="6">
                                <b-form-group id="input-group-3" label="Plazo" label-for="input-3"
                                class="text-left custom-label">
                                    <b-form-select
                                    id="input-3"
                                    v-model="form.deadline"
                                    :options="deadlines"
                                    required
                                    style="height: calc(1.95em + 0.75rem + 2px);"
                                    ></b-form-select>
                                </b-form-group>
                            </b-col>
                        </b-row>
                    </b-container>
                </b-row>
                <h1 class="section-title">
                    Comentarios
                </h1>
                <h6 class="section-subtitle">
                    Nos importan tus comentarios
                </h6>
                <b-row class="mt-4">
                    <b-col>
                        <b-form-group id="input-group-3" label-for="comment"
                         label="¿Dudas? ¿Comentarios?"
                        class="text-left custom-label">
                            <b-form-textarea
                            id="comment"
                            v-model="form.comment"
                            required
                            rows="6"
                            max-rows="6"
                            placeholder="Escribenos"
                            ></b-form-textarea>
                        </b-form-group>
                    </b-col>
                </b-row>
                <b-row>
                    <b-col sm="12" md="6" class="pl-2">
                        <b-row class="pl-4">
                            <b-form-checkbox
                            id="checkbox-1"
                            v-model="terms"
                            name="checkbox-1"
                            value="accepted"
                            unchecked-value=" "
                            class="d-flex"
                            >
                                He leído y acepto el <strong><u>aviso de seguridad</u></strong>
                            </b-form-checkbox>
                        </b-row>
                        <b-row class="pl-4">
                            <b-form-checkbox
                            id="checkbox-2"
                            v-model="promotions"
                            name="checkbox-2"
                            value="accepted"
                            unchecked-value=" "
                            class="d-flex"
                            >
                                No deseo recibir promociones
                            </b-form-checkbox>
                        </b-row>
                    </b-col>
                    <b-col sm="12" md="6" class="d-flex wrap-sendbtn">
                        <b-button class="btn-send" variant="outline-primary">Enviar</b-button>
                    </b-col>
                </b-row>
            </b-container>
      </div>
  </div>
</template>

<script>
export default {
  name: 'PriceQuoteForm',
  props: {
    msg: String,
  },
  data() {
    return {
      selected: null,
      terms: '',
      promotions: '',
      form: {
        email: null,
        name: null,
        lastnamemother: null,
        lastnamefather: null,
        phone: null,
        state: null,
        model: null,
        version: null,
        distributor: null,
        amount: null,
        deadline: null,
        comment: null,
      },
      models: [{ text: 'Seleccionar', value: null }, 'Mobi', 'Uno', 'Argo', 'Fiat 500L'],
      versions: [{ text: 'Seleccionar', value: null }, 'MTX', 'ATX'],
      states: [{ text: 'Seleccionar', value: null }, 'Aguascalientes', 'Baja California', 'Baja California Sur', 'Campeche'],
      distributors: [{ text: 'Seleccionar', value: null }, 'Coahuila Motors', 'Cumbre - Car One'],
      deadlines: [{ text: 'Seleccionar', value: null }, '12 MESES', '18 MESES', '24 MESES', '36 MESES'],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/styles/common';
@import '../assets/styles/variables';

.fixed-margin {
  margin-top: -2.2rem;
}

.image-container {
    background: linear-gradient(180deg, rgba(255, 192, 203, 0) 50%, #FFFFFF 50%);
}

.section-title {
    margin-top: 1.25rem;
    font-family: $title-font;
    text-transform: uppercase;
    justify-content: center;
    display: flex;
    width: 100%;
    align-items: center;
    letter-spacing: 0.6px;
    font-weight: 700;
    color: $base-color;
    font-style: italic;

    &::before,&::after {
        content: '';
        background-color: $base-color;
        height: 0.1rem;
        margin: .5rem;
        width: 3.5rem;
    }
}

.section-subtitle {
    @extend  %spaced-text;
    font-weight: 400;
}

.btn-custom {
    background-color: #fff;
    border-color:$base-color;
    color: $dark-text;
    border-radius: 0px;
    text-transform: uppercase;

    &.active, &:hover {
        border-color: $base-color !important;
        background-color:$base-color !important;
    }
}

.wrap-sendbtn {
    margin-top: 0.75rem;
    justify-content: flex-end !important;
}

.btn-send {
    text-transform: uppercase;
    color: $dark-text;
    font-size: 0.7rem;
    letter-spacing: 0.4rem;
    border-radius: 0px;
    border-color: $base-color;
    color: $dark-text;
    font-weight: 700;
    height: 35px;
}

@import '../assets/styles/queries';
</style>
