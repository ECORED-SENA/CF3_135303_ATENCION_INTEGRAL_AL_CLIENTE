<template lang="pug">
.btns
  .row.justify-center 
    .col-12.col-md-4
      img.img400(src='@/assets/curso/tema2/t2-27.svg', alt='Texto que describa la imagen')
      .btns__item(
        v-for="(boton, index) in botones"
        :style="getStyles(boton, index)"
        @mouseover="hover = index"
        @mouseleave="hover = null"
      )
        .indicador--hover(v-if="index === 0 && indicador")
        .btns__text.row.align-items-center.justify-content-end.px-3.py-4(v-if="index === hover" :style="{left:boton.left, top:boton.top}")
          .col-md-12.p-2
            h5.mb-3.font-weight-bold
              | {{ boton.titulo }}
            p.mb-0(v-html="boton.texto")
        
    

</template>

<script>
export default {
  name: 'BotonesC',
  data: () => ({
    indicador: true,
    hover: null,
    size: '15%',
    botones: [
      {
        pos_x: '34%',
        pos_y: '2%',
        left: '-80%',
        top: '-50%',
        titulo: 'ERP:',
        texto:
          'Sistema de información en el que sistematiza varios procesos de su compañía, se dirá que la empresa tiene un Enterprise Resource Planning (Sistema de planificación de recursos empresariales) más conocido como <b>ERP.</b>',
      },
      {
        pos_x: '51%',
        pos_y: '2%',
        right: '-80%',
        top: '-80%',
        titulo: 'CRM:',
        texto:
          'Sistemas de información enfocados en clientes, es decir, si la empresa posee un sistema de información destinado solo a los clientes, se hará mención a un Customer Relationship Management (Sistema de gestión de las relaciones con los clientes), conocido como <b>CRM.</b>',
      },
      {
        pos_x: '34%',
        pos_y: '51%',
        left: '-80%',
        top: '30%',
        titulo: 'Billing:',
        texto:
          'Sistema enfocado exclusivamente en procesos de facturación y se denomiará <em>Billing</em> (facturadores).',
      },
      {
        pos_x: '51%',
        pos_y: '51%',
        right: '-80%',
        top: '30%',
        titulo: 'Sistema de BI:',
        texto:
          'Sistema enfocado al procesamiento de información de la empresa, se denomina Business Intelligence (Inteligencia de negocios) referenciado en el ámbito empresarial como <b>sistemas de BI.</b>',
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
    text-align: center
    border-radius: 20px
    position: absolute
    left: 200%
    background-color: #FFF6E6
    width: 400px
    z-index: 100
    line-height: 1.2em
    transform: translate(-50%)
    .number
      position: absolute
      top: -10px
      left: 3%
      width: 91px

@media (max-width: $bp-max-md)
  .btns__text
    text-align: center
    width: 200px
    left: 50%
</style>
