<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 5
      h1 Objeciones
    
    .row.mb-5
      .col-12.col-md-4(data-aos="zoom-in-right").mb-3.mb-md-0
        figure.justify-center
            img(src='@/assets/curso/tema5/t5-1.png', alt='Texto que describa la imagen')
      .col-12.col-md-8(data-aos="zoom-in-left")
        p Surgen dentro de la recepción de requerimientos, cuando el cliente siente que el agente de servicio no está entendiendo el requerimiento o cuando el agente le indica que no tiene alcance para recepcionarlo; por tanto, para un agente de servicio es muy importante conocer sobre objeciones, dado que al interactuar con el cliente, este probablemente manifieste no entender lo que se le está explicando, tener dudas o incluso, requerir más información. En palabras más sencillas, las objeciones son una serie de preguntas y afirmaciones interpuestas por los clientes cuando no siente empatía por el personal de la empresa hacia su solicitud.
        p Existen muchas interpretaciones de lo que es una objeción en términos de servicio al cliente. Algunos autores consideran que hace parte del proceso normal de interacción entre un cliente y un representante de la empresa; sin embargo, hay otros que indican que la presencia de objeciones puede denotar desconocimiento por parte de alguno de los dos interlocutores (agente de servicio o cliente). No obstante, a pesar de no existir consenso en por qué se dan, sí es claro, que es un tema clave que un agente de servicio al cliente debe conocer.
    
    p.mb-5 En consecuencia, a continuación, se enuncian dos definiciones de objeciones de autores y una propia:

    .bgr_20.mb-5
      .row
        .col-12.col-md-3
          figure.p-4
            img(src='@/assets/curso/tema5/t5-2.png', alt='Texto que describa la imagen')
        .col-12.col-md-9.align-items-center
          div.p-4.p-md-0
            ol.lista-ol--cuadro.mb-0
              li 
                .lista-ol--cuadro__vineta
                  span 
                | La Real Academia de la Lengua Española RAE (2021) referencia que la objeción es la “razón que se propone o dificultad que se presenta en contra de una opinión o designio, o para impugnar una proposición”.
              li 
                .lista-ol--cuadro__vineta
                  span 
                | Ardila (1984) “las objeciones son cualquier acto del comprador que de forma real o aparente interrumpe la labor del vendedor” (p. 9). 
              li.mb-0 
                .lista-ol--cuadro__vineta
                  span 
                | En sentido práctico, son los “peros” que expone el cliente potencial al vendedor durante el proceso de la venta.

    h2.mb-5(data-aos="zoom-in-left") Tipos de objeciones

    p.mb-5 Las objeciones desde la perspectiva de servicio, al igual que la mayoría de temas vistos, no tienen una única orientación; sin embargo, hay consenso en que existen a nivel general, dos tipos, los cuales se describen a continuación:

    .row.mb-5.justify-center
      .col-12.col-md-4.mb-3.mb-md-0(data-aos="zoom-in-right")
        div.bgr_21.p-5.mb-3.mb-md-0
          figure.mb-3
            img.img90(src='@/assets/curso/tema5/t5-3.svg', alt='Texto que describa la imagen')
          h4 Objeciones verdaderas: 
          p.mb-5 Se presentan cuando el cliente está realmente interesado en el tema a tratar; sin embargo, manifiesta inquietudes o dudas respecto a la información que se le está suministrando y si las respuestas realmente satisfacen las necesidades que él tiene, por lo que busca canalizarlas a través del agente de servicio.
          a.boton.bgr_23.indicador__container(@click="modal1 = true")
            span Ejemplo
            .indicador--click(v-if="mostrarIndicador")
   
      .col-12.col-md-4(data-aos="zoom-in-left")
        div.bgr_22.p-5.mb-3.mb-md-0
          figure.mb-3
            img.img90(src='@/assets/curso/tema5/t5-4.svg', alt='Texto que describa la imagen')
          h4 Objeciones falsas: 
          p Se dan cuando el cliente no está interesado en la información o en el producto, y por ende basa la comunicación en pretextos o cuestionamientos sin racionalidad, con el fin de dispersar la conversación o no manifestar la razón real por la que no desea adquirir los productos de la empresa o no desea tener relación comercial con ella.
          a.boton.bgr_23.indicador__container(@click="modal2 = true")
            span Ejemplo
            .indicador--click(v-if="mostrarIndicador")

    ModalA(:abrir-modal.sync="modal1")
      .row.mb-3
        .col-12.col-md-1.mb-3.mb-md-0
          figure
            img.img90(src='@/assets/curso/tema5/t5-3.svg', alt='Texto que describa la imagen')
        .col-12.col-md-1.align-items-end
          h4.mb-0 Ejemplo
      p Un cliente es contactado por un agente de servicio con el fin de conocer si el cliente está interesado en programar un mantenimiento preventivo para su lavadora, y la persona pregunta ¿por qué tendría que realizarlo si su electrodoméstico se encuentra en buen estado?, esta es una objeción verdadera porque obedece a un argumento racional, donde al obtener la respuesta podría tener un escenario más amplio para tomar la decisión.
    ModalA(:abrir-modal.sync="modal2")
      .row.mb-3
        .col-12.col-md-1.mb-3.mb-md-0
          figure
            img.img90(src='@/assets/curso/tema5/t5-4.svg', alt='Texto que describa la imagen')
        .col-12.col-md-1.align-items-end
          h4.mb-0 Ejemplo
      p Un cliente es contactado por un agente de servicio quien le ofrece un bono de descuento a un nuevo restaurante, el cual tiene 6 meses para ser usado, el cliente informa que no está interesado porque tiene mucho trabajo y no tiene tiempo para asistir a dicho restaurante, esto claramente es una objeción falsa porque aun cuando lo que manifiesta el cliente sea cierto, el tiempo para el disfrute del bono es bastante amplio, por lo que definitivamente este no es un argumento sólido para no aceptar el beneficio.
    
    p.mb-5 Asociado al manejo de objeciones, es claro mencionar que, si bien existe la teoría, las clasificaciones y los ejemplos, hay dos factores que influyen en la gestión de las mismas: 

    .row.justify-center.mb-5
      .col-12.col-md-1.mb-3.mb-md-0
        figure.justify-center
          img.img90(src='@/assets/curso/tema5/t5-5.svg', alt='Texto que describa la imagen')
      .col-12.col-md-4
        .titulo-sexto.color-primario
          span <b>La personalidad del agente,</b> dado que la esencia de la persona influye mucho en el trato con las demás personas.
      .col-12.col-md-1.mb-3.mb-md-0
        figure.justify-center
          img.img90(src='@/assets/curso/tema5/t5-6.svg', alt='Texto que describa la imagen')
      .col-12.col-md-4
        .titulo-sexto.color-secundario
          span <b>La experiencia,</b> cada vez que se tiene mayor contacto con los clientes se van adquiriendo más destrezas para interactuar y manejar situaciones que a simple vista incluso pueden ser inmanejables.
    
    h2.mb-5(data-aos="zoom-in-left") Resolución de objeciones

    p.mb-5 Navarro (2012) en su libro <b>Técnicas de ventas</b> propone un esquema interesante para el manejo de objeciones, comenzando por la <b>escucha</b> como el principio básico de la comunicación, luego a partir de la asertividad <b>anticiparse</b> a posibles alternativas de respuesta o solución, posteriormente a través de un ejercicio de empatía <b>comprender</b> la situación y finalmente si el cliente aún tiene inquietudes y <b>refuta</b> lo expuesto, exponer con argumentos claros y respetuosos la alternativa de solución.

    .row.mb-5.justify-center
      .col-12.col-md-10(data-aos="zoom-in-up")
        figure
          img.d-none.d-lg-flex(src='@/assets/curso/tema5/t5-11.svg', alt='Texto que describa la imagen')
    .row.mb-5     
      .col-12.mb-3(data-aos="zoom-in-right")
        figure.justify-center
          img.img200.d-flex.d-lg-none(src='@/assets/curso/tema5/t5-7.svg', alt='Texto que describa la imagen')
      .col-12.mb-3(data-aos="zoom-in-left")
        figure.justify-center
          img.img200.d-flex.d-lg-none(src='@/assets/curso/tema5/t5-8.svg', alt='Texto que describa la imagen')
      .col-12.mb-3(data-aos="zoom-in-right")
        figure.justify-center
          img.img200.d-flex.d-lg-none(src='@/assets/curso/tema5/t5-9.svg', alt='Texto que describa la imagen')
      .col-12(data-aos="zoom-in-left")
        figure.justify-center
          img.img200.d-flex.d-lg-none(src='@/assets/curso/tema5/t5-10.svg', alt='Texto que describa la imagen')

    p.mb-5 A nivel general, las objeciones más frecuentes que los clientes manifiestan a los agentes de servicios están relacionadas con:

    TabsB.color-acento-contenido(data-aos="zoom-in-up")
      .py-4.py-md-5(titulo="Precio" :icono="require('@/assets/curso/tema5/t5-12.svg')")
        .row
          .col-md-8.mb-4.mb-md-0.align-items-center
            div
              h4 Precio
              p.mb-0 Cuando los agentes tienen también rol comercial, el precio será siempre la variable de objeción por excelencia, dado que los clientes siempre querrán pagar menos para obtener los bienes y servicios de la empresa. En algunos casos, la cultura también impacta este tipo de objeciones, lo que comúnmente se llama “regatear”. El manejo de esta objeción se da principalmente en contrarrestar con argumentos desde las características, beneficios y ventajas del producto, así se tratará de mostrar una relación costo - beneficio positiva; en otras ocasiones, cuando el agente tiene el perfil de negociar también puede acudir a los descuentos para tratar de cerrar la venta.
          .col-md-4
            figure
              img(src='@/assets/curso/tema5/t5-17.png', alt='Texto que describa la imagen')
      .py-4.py-md-5(titulo="Comparación con la competencia" :icono="require('@/assets/curso/tema5/t5-13.svg')")
        .row
          .col-md-8.mb-4.mb-md-0.align-items-center
            div
              h4 Comparación con la competencia
              p.mb-0 Es frecuente que los clientes acudan a comparar a la empresa con los competidores, indicando que ellos hacen las cosas mejor, para ello el mecanismo de argumento frente a esto es conocer muy bien la empresa y su oferta de valor (su diferencial en el mercado), con la finalidad de hacer visible porque la compañía también tiene muchos puntos a favor.
          .col-md-4
            figure
              img(src='@/assets/curso/tema5/t5-18.png', alt='Texto que describa la imagen')
      .py-4.py-md-5(titulo="Tiempos de entrega" :icono="require('@/assets/curso/tema5/t5-14.svg')")
        .row
          .col-md-8.mb-4.mb-md-0.align-items-center
            div
              h4 Tiempos de entrega
              p.mb-0 Cuando el agente de servicio tiene alcance en el proceso de gestión de pedidos, los tiempos de entrega son una variable crítica para los clientes, y frecuentemente se contactan con la empresa para obtener información sobre el estado del pedido, para ello el primer paso del agente del servicio es validar si dicho pedido aún se encuentra dentro de los tiempos de entrega o ya está retrasado, en el primer caso, se debe hacer visible al cliente que el pedido se encuentra en gestión y que en cualquier momento puede llegar a sus manos. En el segundo caso, cuando ya los tiempos han pasado el agente de servicio debe escalar el caso y entregarle al cliente (en la medida de lo posible) una fecha u hora estimada de entrega.
          .col-md-4
            figure
              img(src='@/assets/curso/tema5/t5-19.png', alt='Texto que describa la imagen')
      .py-4.py-md-5(titulo="Inquietud sobre el porqué del contacto" :icono="require('@/assets/curso/tema5/t5-15.svg')")
        .row
          .col-md-8.mb-4.mb-md-0.align-items-center
            div
              h4 Inquietud sobre el porqué del contacto
              p.mb-0 Cuando el contacto es generado por el agente de servicio y no por el cliente se debe informar al cliente de dónde se obtuvo la información para contactarlo, cuál es el objetivo del contacto y que toda la información que se trate está respetando la Ley 1581 de 2012 (marco normativo de la protección de datos personales en Colombia).
          .col-md-4
            figure
              img(src='@/assets/curso/tema5/t5-20.png', alt='Texto que describa la imagen')
      .py-4.py-md-5(titulo="Agente no resuelve requerimiento del cliente" :icono="require('@/assets/curso/tema5/t5-16.svg')")
        .row
          .col-md-8.mb-4.mb-md-0.align-items-center
            div
              h4 Agente no resuelve requerimiento del cliente
              p.mb-0 Desde la óptica de cliente, siempre se espera que en el primer contacto los requerimientos quedan resueltos; sin embargo, por temas de perfiles, estructura organizacional y procedimientos técnicos, no siempre será así. Por tanto, el rol del agente de servicio será tener una comunicación efectiva con el cliente, informando en detalle por qué no puede gestionar su requerimiento, mostrando interés en la gestión del mismo, aunque aclarando que deben respetarse los flujos, tiempos o lineamientos de la empresa.
          .col-md-4
            figure
              img(src='@/assets/curso/tema5/t5-21.png', alt='Texto que describa la imagen')
           

      
               

       
    

</template>

<script>
export default {
  name: 'Tema3',
  data: () => ({
    modal1: false,
    modal2: false,
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
