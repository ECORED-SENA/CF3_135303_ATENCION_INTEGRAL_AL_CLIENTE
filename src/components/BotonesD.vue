<template lang="pug">
.btns
  .row.justify-center 
    .col-12.col-md-8.posit_1.position-relative
      img.img800(src='@/assets/curso/tema2/t2-28.svg', alt='Texto que describa la imagen')
      .btns__item(
        v-for="(boton, index) in botones"
        :style="getStyles(boton, index)"
        @mouseover="hover = index"
        @mouseleave="hover = null"
      )
        .indicador--hover(v-if="index === 0 && indicador")
        .btns__text.row.align-items-center.justify-content-end.px-3.py-4(v-if="index === hover" :style="{left:boton.left, top:boton.top}")
          .col-md-12.p-2.text-white
            h5.mb-3.font-weight-bold
              | {{ boton.titulo }}
            p.mb-0(v-html="boton.texto")
        
    

</template>

<script>
export default {
  name: 'BotonesD',
  data: () => ({
    indicador: true,
    hover: null,
    size: '12%',
    botones: [
      {
        pos_x: '5%',
        pos_y: '67%',
        right: '0',
        top: '-100',
        titulo: 'Automatización de procesos',
        texto:
          'El ERP tiene como una de sus finalidades, evitar las manualidades y por tanto, optimizar los tiempos de las personas. ',
      },
      {
        pos_x: '18%',
        pos_y: '22%',
        left: '0',
        top: '-100%',
        titulo: 'Integración entre plataformas',
        texto:
          'Al tener varios procesos sobre un mismo aplicativo permite que varias plataformas estén técnicamente integradas en una sola, lo que genera mayor agilidad en los procesos. ',
      },
      {
        pos_x: '43%',
        pos_y: '6%',
        left: '50%',
        top: '-100%',
        titulo: 'Generación de reportes',
        texto:
          'Los ERP son herramientas muy útiles en el momento de requerirse informes, lo que permite tener un panorama completo con información de calidad.',
      },
      {
        pos_x: '68%',
        pos_y: '28%',
        left: '100%',
        top: '-70%',
        titulo: 'Información en tiempo real',
        texto:
          'La empresa tendrá siempre a su disposición la información actualizada para su uso.',
      },
      {
        pos_x: '82%',
        pos_y: '68%',
        left: '-18%',
        top: '-70%',
        titulo: 'Flexibilidad para la implementación',
        texto:
          'Los ERP usualmente se pueden adquirir a través de módulos, lo que permite para la compañía flexibilidad en términos de impacto en costos y en términos de apropiación para los colaboradores.',
      },
    ],
  }),
  watch: {
    selected() {
      this.indicador = false
    },
    hover() {
      this.indicador = false
    },
  },
  methods: {
    getStyles(boton, index) {
      const image = this.hover === index ? boton.img_h : boton.img
      return {
        'background-image': `url(${image})`,
        top: boton.pos_y,
        left: boton.pos_x,
        width: this.size,
        'padding-top': this.size,
      }
    },
  },
}
</script>

<style lang="sass" scoped>
.btns
  position: relative
  &__item
    width: 80px
    position: absolute
    background-size: auto
    background-repeat: no-repeat
    cursor: pointer
    background-position: center
    transition: background-image 0.2s ease-in-out
  &__text
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1)
    text-align: left
    border-radius: 20px
    position: absolute
    left: 200%
    background-color: #373660
    width: 400px
    z-index: 100
    line-height: 1.2em
    transform: translate(-50%)
    .number
      position: absolute
      top: -10px
      left: 3%
      width: 91px

@media (max-width: $bp-max-xs)
  .btns__text
    text-align: center
    width: 200px
    left: 100px
</style>
