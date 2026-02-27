<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    p.mb-5 El siguiente mapa integra los criterios y especificidades de los conocimientos expuestos en el presente componente formativo.

    .row.justify-content-center.mb-5
      .col-lg-10.mb-5.col-sm-9
        figure
          img(src="@/assets/curso/temas/sintesis1.svg", alt="En este componente se detalla, diseño físico y diseño lógico. 1. Diseño lógico:  a. Crear mapas altamente técnicos de las estructuras y reglas de datos subyacentes.  b. Reduce el almacenamiento de datos innecesario. c. Análisis de impacto. 2. Diseño físico: a. Creación de bases de datos con el modelo de diseño lógico teniendo en cuenta las estrategias adecuadas y mejores prácticas de seguridad. b. El diseño físico inicial debe revisarse periódicamente para asegurarse de que sigue satisfaciendo las necesidades del cliente. 3. Ubicación física: a. Almacenamiento seguro, recuperable, confiable y fácil administración. b. Diferentes ubicaciones, sistemas y esquemas. c. Data centers en diferentes países.")

    .row.justify-content-center
      .col-lg-12.col-sm-9
        figure.mb-5
          img(src="@/assets/curso/temas/sintesis2.svg", alt="Modelo multidimensional. Un modelo multidimensional dentro del entorno de las bases de datos es un sistema de software creado para el almacenamiento y la reconstrucción eficiente de miles de datos que se encuentran relacionados, almacenados, revisados y estudiados desde diferentes perspectivas  (conocidas con el nombre de dimensiones). 1. Conceptos: a. Cubos: OLAP, manejo de una robusta cantidad de datos. b. Dimensiones: agregan datos en detalle dentro del nivel deseado. c. Medida: dato numérico que representa una actividad. 2. Tipos de bases: a. Tablas de hechos fact: es la tabla central que almacena la expresión numérica del negocio. b. Tablas de dimensiones O Lock Up: estas tablas se conectan y alimentan a la tabla fact.  3. Esquemas: a. Estrella o star: una gran tabla central unida con puntos radiales desde el centro. b. Copo de nieve o snowflake: son diferentes tablas que pueden ser generadas de tablas adicionales.")
      .col-auto
        a.anexo.mb-4(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
          .anexo__icono
            img(src="@/assets/template/icono-pdf.svg")
          .anexo__texto
            p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
