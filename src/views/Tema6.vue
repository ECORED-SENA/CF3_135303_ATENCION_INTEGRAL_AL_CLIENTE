<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 6
      h1 Informes
    
    p Son la herramienta de gestión más utilizada en el ámbito empresarial, en los informes se resume la planeación, gestión y/o seguimiento sobre un tema, actividad o proyecto en particular. Si bien los agentes de servicio a nivel general no están enfocados en la generación de informes, sí es importante que conozcan su estructura en caso de que le sean solicitados.
    p.mb-5 A <b>nivel empresarial,</b> los ítems que se suelen abordar en informes de tipo empresarial son:

    .row.mb-5
      .col-12.col-md-3(data-aos="zoom-in-right")
        figure.mb-3
          img.tranform_1.img120(src='@/assets/curso/tema6/t6-1.svg', alt='Texto que describa la imagen')
        .titulo-sexto.color-primario
          p <b>Objetivo:</b>
          p Cuál es la razón que origina la presentación del documento. 
      .col-12.col-md-3(data-aos="zoom-in-left")
        figure.mb-3
          img.tranform_1.img120(src='@/assets/curso/tema6/t6-2.svg', alt='Texto que describa la imagen')
        .titulo-sexto.color-secundario
          p <b>Destinatario:</b>
          p A quién está dirigido el informe.
      .col-12.col-md-3(data-aos="zoom-in-right")
        figure.mb-3
          img.tranform_1.img120(src='@/assets/curso/tema6/t6-3.svg', alt='Texto que describa la imagen')
        .titulo-sexto.color-acento-contenido
          p <b>Desarrollo de la temática:</b>
          p Se aborda el tema objetivo del informe, para ello se sugiere la incorporación de gráficos, indicadores y tablas, que ayuden a un mejor entendimiento. 
      .col-12.col-md-3(data-aos="zoom-in-left")
        figure.mb-3
          img.tranform_1.img120(src='@/assets/curso/tema6/t6-4.svg', alt='Texto que describa la imagen')
        .titulo-sexto.color-acento-botones
          p <b>Conclusiones y/o recomendaciones:</b>
          p Este punto constituye el valor agregado de los informes y está orientado en conocer de una forma técnica cuál es la percepción de los grandes resultados del informe y cuáles son las opciones de mejora que se identifican.
    
    .row.mb-5
      .col-12.col-md-4.mb-3.mb-md-0(data-aos="zoom-in-right")
        figure.mb-3
          img(src='@/assets/curso/tema6/t6-5.png', alt='Texto que describa la imagen')
      .col-12.col-md-8(data-aos="zoom-in-left")
        p A nivel de formatos, la mayoría de informes son realizados en programas de ofimática, tipo procesador de datos (Word) o tipo presentación (Power Point) y entregados en formato no editable (tipo PDF). No obstante, las empresas que implementan informes o reportes en aplicaciones de inteligencia de negocios (BI) acuden a la herramienta de visualización, con el fin de tener la información de forma digital y en tiempo real, lo anterior se conoce como <em>“dashboards”</em> o tableros de visualización, cada vez más implementados en las compañías.
        p.mb-5 Algunas de las aplicaciones de la inteligencia de negocios, que tienen componente de visualización de información son Power BI (de Microsoft), Qlik y Tableau.
    
    h2.mb-5(data-aos="zoom-in-left") Tipos de informe según su contenido

    p.mb-5 Según su contenido, los informes pueden ser clasificados en: 

    .row.mb-5(data-aos="zoom-in-up")
      .col-sm-6.col-xl-3.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema6/t6-6.svg')})`}")
            .tarjeta-flip__contenido.p-4.p-xl-5
              h3 Expositivos
              p Cuando el fin es dar a conocer información de tipo descriptivo, usualmente no tienen profundidad en análisis, por lo que su objetivo es mostrar la realidad de hechos o actividades empresariales, en el mundo empresarial se conocen como “mostrar la foto”, es decir, contar lo que está aconteciendo tal cual como se está presentado la situación.
      .col-sm-6.col-xl-3.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema6/t6-7.svg')})`}")
            .tarjeta-flip__contenido.p-4.p-xl-5
              h3 Interpretativos
              p Se realizan cuando tienen por fin no solo describir la información sino también suministrar análisis, conclusiones y recomendaciones.
      .col-sm-6.col-xl-3.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema6/t6-8.svg')})`}")
            .tarjeta-flip__contenido.p-4.p-xl-5
              h3 Demostrativos
              p Son aquellos que propenden por mostrar los hallazgos respecto a alguna hipótesis de negocio planteada o dar a conocer una postura respecto a una situación específica, en este segundo caso de uso, siempre deberá quedar claro cuál es la situación (es decir, lo que está aconteciendo) y cuál es la postura (es decir, la reflexión personal).
      .col-sm-6.col-xl-3.mb-4.mb-xl-0
        .tarjeta.tarjeta-flip.color-primario(@mouseover="indicadorTarjetaFlip = false")
          .indicador--hover(v-if="indicadorTarjetaFlip")
          .tarjeta-flip__contenedor
            .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema6/t6-9.svg')})`}")
            .tarjeta-flip__contenido.p-4.p-xl-5
              h3 Persuasivos
              p Tienen por fin obtener alguna aprobación o convencer a determinado público respecto a una valoración que se está dando sobre un tema.

    p Desde la perspectiva de los agentes de atención al cliente cuando le es asignada la elaboración de informes, usualmente se realizan con <b>fines expositivos,</b> bajo dos tipos de escenarios, el primero, cuando se está <b>analizando el protocolo de servicio implementado con un cliente,</b> en este caso, se solicita describir el paso a paso seguido con el cliente desde el momento del contacto inicial para la recepción de su requerimiento, hasta la última interacción que se haya tenido con él; el segundo escenario se da cuando el jefe o supervisor solicita <b>un informe de gestión desde el rol,</b> en el cual el deberá desagregar las diferentes actividades que ha estado realizado en su día a día y cuáles han sido los logros obtenidos.
    

</template>

<script>
export default {
  name: 'Tema3',
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
