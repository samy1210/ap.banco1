<template>
    <div>
    <div class="columns is-mobile myContenidoCentral">
    <div class="column">
        <div class="tituloIngresaCuenta">INGRESA A TU CUENTA</div>
        <div class="formulario">
            <b-field label="Cuenta">
            <b-numberinput :controls="false"></b-numberinput>
        </b-field>
        <b-field label="Tipo de cuenta">
        <b-select placeholder="Selec tipo cuenta"></b-select>
        </b-field>

        <b-field label="Calve">
            <b-input type="password" value="clave12345" password-reveal></b-input>
        </b-field>

        <b-button type="is-warning">Ingresar</b-button>
      </div>  
      <div class="transacciones">
  <b-menu>
    <b-menu-list>
      <b-menu-item icon="settings" :active="isActive" expanded>
        <template slot="label" slot-scope="props">
          TRANSACCIONES
          <b-icon class="is-pulled-right" :icon="props.expanded ? 'menu-down' : 'menu-up'"></b-icon>
        </template>
        <b-menu-item icon="account" label="Banca personal"></b-menu-item>
        <b-menu-item icon="account" label="Banca empresarial"></b-menu-item>
        <b-menu-item icon="account" label="Banca seguros"></b-menu-item>
        <b-menu-item icon="account" label="Pago de facturas"></b-menu-item>
        <b-menu-item icon="cellphone-link">
          <template slot="label">
            TARJETAS DE CREDITO
            <b-dropdown aria-role="list" class="is-pulled-right" position="is-bottom-left">
              <b-icon icon="dots-vertical" slot="trigger"></b-icon>
              <b-dropdown-item aria-role="listitem">Action</b-dropdown-item>
              <b-dropdown-item aria-role="listitem">Another action</b-dropdown-item>
              <b-dropdown-item aria-role="listitem">Something else</b-dropdown-item>
            </b-dropdown>
          </template>
        </b-menu-item>
        <b-menu-item icon="account" label="Devi Vissa"></b-menu-item>
        <b-menu-item icon="account" label="Credi Mastercard"></b-menu-item>
      </b-menu-item>
    </b-menu-list>
  </b-menu>
      </div>
    </div>
      <div class="column">2</div>
      <div class="column">3</div>
    </div>
    </div>
</template>

<script>
export default {
    data() {
    return {
      isActive: true
    }
  }
};
</script>

<style scoped>
.tituloIngresaCuenta {
    text-align: center;
    color: azure;
    background-color: black;
    height: 42px;
}
.myContenidoCentral{
    margin-top: 0px;
}
.formulario{
    background-color: gray;
}
</style>