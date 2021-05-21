<template>
  <div>
    <h1>
     Mi nombre es: <strong>{{ nombre }} Mi edad es {{edad}}</strong> <!--strong= negrita-->
    </h1>
    <!--recorrer todas las materias (creadas en el componente) y se van a recorrer una a una y se guardan en la variable materia simepre tiene que llevar un key unico -->
    <!--   <ul v-for="materia in materias" :key="materia">
      <li>
        {{ materia }}
      </li>
    </ul>-->
    <p>
      <!--para escribir el nombre dentro de la pagina y que se imprima hay que guardar el resultado(recibir el valor de la entrada ) en otra variable y despues que la muestre -->
      <!--el v-model es para asignar una variable del componente que se encuentre en el script-->
      <input type="text" v-model="nombre"/>
    </p>
    <p>
         <input type="text" v-model="edad"/>
    </p>
  </div>
</template>

<script>
export default {
  nombre: "componente",
  data() {
    return {
      nombre: "",
      edad: 0
    };
  },
  methods: {},
};
</script>

<style>
@import "../assets/styles/styles.css";
</style>