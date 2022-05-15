<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 4
      h1 Requerimientos
    
    p.mb-5 Un requerimiento en términos de servicio al cliente es cualquier solicitud que realiza un cliente a una empresa a través de un canal oficial habilitado por la compañía. Son muy importantes estos requerimientos, ya que son los que materializan las <b>necesidades de los clientes</b> y en este sentido, permiten a la empresa tener contacto efectivo con ellos y en un escenario ideal obtener información valiosa para fidelizarlos e incluso para anticiparse a sus próximas necesidades de compra.

    h3.mb-5(data-aos="zoom-in-left") Características de los requerimientos

    p Las características están asociadas a su tipología, ya que dependiendo de ella dará el alcance para la aplicación del protocolo del servicio y en términos de personal, define incluso un perfil para el tipo de personal que se requiere para gestionar cada uno de ellos, por ejemplo, el perfil para una persona de televentas no es el mismo para una persona de servicio enfocada en soporte técnico.
    p.mb-5 Estos son los tipos de requerimientos que se abordan en las empresas con presencia en Colombia:

    .row.justify-center.mb-3
      .col-12.col-md-2(data-aos="zoom-in-up").mb-3.mb-md-0
        div.bgr_15.p-4.justify-align
          a.lnk(@click="modal1 = true") Informativos
      .col-12.col-md-3(data-aos="zoom-in-down").mb-3.mb-md-0
        div.bgr_15.p-4.justify-align
          a.lnk(@click="modal2 = true") Peticiones, quejas, reclamos, sugerencias, felicitaciones (PQRSF)
      .col-12.col-md-3(data-aos="zoom-in-up").mb-3.mb-md-0
        div.bgr_16.p-4.justify-align
          span Soporte técnico
      .col-12.col-md-2(data-aos="zoom-in-down").mb-3.mb-md-0
        div.bgr_16.p-4.justify-align
          span Pedidos
    .row.justify-center.mb-5
      .col-12.col-md-2(data-aos="zoom-in-up").mb-3.mb-md-0
        div.bgr_16.p-4.justify-align
          span Televentas
      .col-12.col-md-2(data-aos="zoom-in-down").mb-3.mb-md-0
        div.bgr_16.p-4.justify-align
          span Cobranza
      .col-12.col-md-2(data-aos="zoom-in-up").mb-3.mb-md-0
        div.bgr_16.p-4.justify-align
          span Sondeos
    
    ModalA(:abrir-modal.sync="modal1")
      .row.align-items-center     
        .col-md-2
          figure.justify-center
            img.img160(src='@/assets/curso/tema4/t4-1.svg', alt='Texto que describa la imagen')
        .col-md-10.mb-4.mb-md-0
          h4 Requerimientos informativos: 
          p Los usuarios valoran su tiempo, por tanto, se comunican frecuentemente a las empresas con el fin de conocer información sobre canales de venta, horarios de atención, direcciones de sedes/sucursales, precios, características de los productos, políticas comerciales y otros aspectos que consideran básicos de las empresas.
    ModalA(:abrir-modal.sync="modal2")
      .row.align-items-center     
        .col-md-2
          figure.justify-center
            img.img160(src='@/assets/curso/tema4/t4-2.svg', alt='Texto que describa la imagen')
        .col-md-10.mb-4.mb-md-0
          h4 Peticiones, quejas, reclamos, sugerencias, felicitaciones (PQRSF):  
          p Las Peticiones (P), Quejas (Q), Reclamos (R), Sugerencias (S) y Felicitaciones (F) son en muchas ocasiones la mayor composición dentro de los requerimientos de los usuarios, ya que la mayoría de sus solicitudes hacia la empresa están enfocadas en ellas. A nivel general, las PQRS hacen alusión a inconformidades o dificultades con la empresa, su personal o los productos adquiridos, mientras que las felicitaciones aluden a un reconocimiento de cliente hacia la empresa y las sugerencias una visión de mejora desde una perspectiva propositiva. 
    
    p.mb-3.mb-md-5 Atendiendo la importancia de este tema, se invita a revisar el video que se muestra a continuación, con el fin de hacer mayor énfasis en las PQRSF:

    .bg_grad-01
      .row.justify-center.pt-5.pb-5
        .col-12.col-md-10
          figure
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/2L91WMqw96A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)

    p.mb-5 Adicionalmente y con el fin de que logre una mayor apropiación sobre este tema se expondrán dos ejemplos que darán alcance a la aplicación de los conceptos vistos sobre requerimientos, esto es:    

    .row.justify-center.mb-5
      .col-12.col-md-5.mb-3.mb-md-0(data-aos="zoom-in-right")
        div.bgr_17.p-4
          p.text-bold Ejemplo 1
          figure.mb-3  
            img.img450(src='@/assets/curso/tema4/t4-3.png' alt='AvatarTop')
          p Manuel llega a la empresa y le indica que requiere una copia de su última factura porque la necesita para legalizar unos viáticos en su empresa, en este caso lo que Manuel está escalando a la empresa es una <b>petición;</b> sin embargo, el agente de servicio que atiende su requerimiento lo trata de forma descortés y le indica que esto no es posible, por lo que Manuel indica que interpondrá una <b>queja</b> a la empresa por el mal comportamiento del agente de servicio que lo atendió.
      .col-12.col-md-5(data-aos="zoom-in-left")
        div.bgr_18.p-4
          p.text-bold Ejemplo 2
          figure.mb-3  
            img.img450(src='@/assets/curso/tema4/t4-4.png' alt='AvatarTop')
          p Gloria va a pagar su factura en un restaurante, pero al detallar ve que le han cobrado erróneamente, por lo que solicita que se llame al administrador para formular un <b>reclamo,</b> al llegar a la mesa el administrador le indica que los disculpe, que ya mismo le generan nuevamente la factura con el valor correcto, por lo que el cliente indica que a nivel de <b>sugerencia</b> considera importante que se revisen las facturas por parte de los meseros antes de entregarlas a los comensales. 
    
    p.mb-5 Se invita a ver con mayor detalle a través del siguiente gráfico todo lo que tiene que ver con PQRSF:

    TabsA.color-primario.mb-5(data-aos="zoom-in-up")
      .tarjeta.color-primario--borde.bgr_19.p-4(titulo="Petición")
        h4 Petición
        p En términos generales, hace referencia a una solicitud formal de un cliente para obtener de igual manera una respuesta de la empresa ante un tema específico, el fin de una petición es “obtener información”. Cabe mencionar, que cuando se indica que es una solicitud formal implica que en la empresa debe quedar trazabilidad de la misma, es decir, documentada o registrada en algún sistema de información, así mismo, al usuario le debe quedar un soporte de su requerimiento, lo que usualmente se conoce como <b>radicado</b> o <b>consecutivo.</b>
        p También en términos normativos existe una definición en Colombia, dada en la Ley 1755 de 2015, donde se informa en su Artículo 14 que para las entidades públicas “Salvo norma legal especial y so pena de sanción disciplinaria, toda petición deberá resolverse dentro de los quince días siguientes a su recepción”.
        p Pese a lo anterior, es de destacar que en actividades económicas no reguladas, el tiempo de gestión de peticiones lo define la empresa a través de sus políticas internas, estableciendo procedimientos y protocolos que aseguren la oportuna respuesta al cliente, aunque es un término muy usado, la referencia de los 15 días mencionados previamente.
      .tarjeta.color-primario--borde.bgr_19.p-4(titulo="Queja")
        h4 Queja
        p Se entiende como la manifestación del cliente sobre algo que considera injusto, un problema, dificultad o inconformidad. Se clasifica como queja cuando el motivo de la misma está asociado a cualquier temática, excepto el funcionamiento del producto o la prestación del servicio. 
        p En otras palabras, las quejas son cuando el cliente manifiesta insatisfacción en la forma como fue atendido o manejado su requerimiento. Es de mencionar, que en Colombia, usualmente las quejas están relacionadas con el personal de la empresa, es decir, por una percepción de mal servicio.
        p Similar a como ocurre con las peticiones, también se debe asegurar que se tenga el registro de la acción interpuesta por parte del cliente, así como también el cliente/ usuario deberá tener alguna constancia de la presentación de la misma.
      .tarjeta.color-primario--borde.bgr_19.p-4(titulo="Reclamo")
        h4 Reclamo
        p También se entiende como una manifestación de inconformidad, solo que en este caso, está directamente relacionado con el producto (si es una empresa de tangibles) o con la prestación del servicio (si es una empresa de intangibles). En Colombia, los reclamos suelen estar relacionados con el mal funcionamiento de los productos, incumplimiento de la promesa del servicio o temas asociados con cobros incorrectos (facturaciones erróneas o entregas tardías).
        p Al igual que en las peticiones y las quejas, los reclamos deben quedar documentados o registrados en la empresa y el cliente debe tener algún tipo de soporte de la acción interpuesta.
      .tarjeta.color-primario--borde.bgr_19.p-4(titulo="Sugerencias")
        h4 Sugerencias
        p Este es un concepto muy bonito, dado que el hecho que el cliente presente una sugerencia a la empresa, ya implica un nivel de involucramiento o interés en la misma, lo cual en primera instancia ya es una ganancia para la organización. Las sugerencias son una opción que tienen los clientes para dar a conocer a la empresa ideas, opiniones, propuestas, acciones de mejora o algún aspecto que consideran puede mejorar el desempeño de la compañía.
        p A diferencia de las peticiones, quejas y reclamos, de las sugerencias si bien debe quedar trazabilidad en la organización como parte de su compromiso con la mejora continua, en este caso, el cliente no debe quedarse con algún tipo de constancia asociada a la entrega de la misma.
      .tarjeta.color-primario--borde.bgr_19.p-4(titulo="Felicitaciones")
        h4 Felicitaciones
        p Son la forma que tiene un cliente de dar a conocer a la empresa que desde su óptica está haciendo bien las cosas. Técnicamente, las felicitaciones expresadas de manera formal (es decir, a través de algún canal de la compañía), es la mejor representación de la satisfacción del cliente, lastimosamente, en nuestra cultura son menos frecuentes.
    
    p.mb-5 Continuando con este aprendizaje, se invita a revisar los demás tipos de requerimientos que se abordan en las empresas, por favor consulte lo que se expone a continuación:

    .tarjeta.bg_grad-05.p-4.mb-5(data-aos="zoom-in-up")
      SlyderA
        .row.p-5
          .col-md-7.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema4/t4-5.png', alt='Texto que describa la imagen')
          .col-md-5.align-items-center
            div
              h4 Soporte técnico
              p Este soporte tiene varios alcances, el primero de ellos es cuando los clientes tienen desconocimiento o dudas sobre el manejo de los productos o servicios de la empresa; el segundo es cuando tienen dificultad para acceder a alguno de los canales digitales de la compañía; finalmente, el tercero que es cuando tienen problemas con sus servicios y requieren de la empresa para validar remotamente o en el sitio su funcionamiento.
        .row.p-5
          .col-md-7.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema4/t4-6.png', alt='Texto que describa la imagen')
          .col-md-5.align-items-center
            div
              h4 Pedidos
              p En términos comerciales son los requerimientos de compras de un cliente hacia la empresa. En este orden de ideas, los agentes de servicio al cliente que están asociados a la gestión de pedidos deben estar en la capacidad de crearlos (tomarlos) e informar sobre el estado de los mismo (dar seguimiento).
        .row.p-5
          .col-md-7.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema4/t4-7.png', alt='Texto que describa la imagen')
          .col-md-5.align-items-center
            div
              h4 Televentas
              p Son canales especializados en las ventas a través de canales telefónicos, si bien hacen parte más del mundo comercial que del alcance de servicio al cliente, hoy en día es común que los agentes de servicio se vean orientados también a tener metas comerciales, es decir, a que su gestión también tenga asociados indicadores de ventas.
        .row.p-5
          .col-md-7.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema4/t4-8.png', alt='Texto que describa la imagen')
          .col-md-5.align-items-center
            div
              h4 Cobranza
              p Es la actividad donde se realizan gestiones para la recuperación del dinero que las empresas tienen pendiente por cobro, cuando hacen ventas a crédito. Es la actividad que completa el ciclo de la venta, con el fin de que el cliente compre nuevamente.
        .row.p-5
          .col-md-7.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema4/t4-9.png', alt='Texto que describa la imagen')
          .col-md-5.align-items-center
            div
              h4 Sondeos
              p La satisfacción del cliente es el fin último de las compañías en su relación con ellos, es por eso, que la realización de actividades enfocadas en conocer la opinión de estos respecto a la empresa, sus productos, sus canales de atención y su personal es vital para evaluar lo que está haciendo bien y lo que podría hacer mejor. 
        .row.p-5
          .col-md-7.mb-4.mb-md-0
            figure
              img(src='@/assets/curso/tema4/t4-10.png', alt='Texto que describa la imagen')
          .col-md-5.align-items-center
            div
              h4 Otros tipos de requerimientos
              p Las actividades de preventa, el agendamiento de citas, la actualización de bases de datos, la toma de domicilios y referidos de clientes. 

    h3.mb-5(data-aos="zoom-in-left") Técnicas para la gestión de requerimientos

    .row.mb-5
      .col-12.col-md-4.mb-3.mb-md-0(data-aos="zoom-in-right")
        figure
          img(src='@/assets/curso/tema4/t4-11.png', alt='Texto que describa la imagen')
      .col-12.col-md-8(data-aos="zoom-in-left")
        p Con el fin de comprender de manera asertiva el lenguaje comunicacional en los procesos de atención al cliente y antes de ver el paso a paso para la gestión de requerimientos, se hace necesario conocer algunos conceptos básicos que se tienen a nivel operativo, en este sentido, surgen: la <b>creación</b> del caso, como el momento en el que se formaliza el requerimiento por parte del cliente hacia la empresa; el <b>escalamiento</b> del caso, obedece al momento en el que el agente de servicio debe direccionar el requerimiento para que sea gestionado por otra persona o área de la compañía y el cierre del caso se da cuando el recurso que está atendiendo el requerimiento tiene la competencia para dar la solución al cliente.
        p Ahora bien, desde la perspectiva de la atención al cliente, el procedimiento técnico para la gestión de requerimientos se basa en el protocolo de servicio definido por la compañía, ya que este es elaborado teniendo en cuenta la <b>identidad de la empresa,</b> el <b>perfil de clientes</b> y los <b>diferentes tipos de solicitudes</b> que un cliente pudiese presentar. No obstante, podrían mapearse a través de un flujo como son a nivel general las actividades que sigue la gestión de requerimientos en una compañía, todo ello desde la óptica de un agente de servicio, donde siempre se tendrá como fin la <b>satisfacción de los clientes.</b>
    
    h6.mb-5 Flujo para la atención de requerimientos

    .bgr_19.mb-5
      figure.p-2.p-md-5(data-aos="zoom-in-up") 
        img(src='@/assets/curso/tema4/t4-12.svg', alt='Texto que describa la imagen')
    
    p Lo que muestra este flujo hace alusión a que el primer paso técnico por parte del agente de ventas es validar la identidad del usuario, posteriormente se debe verificar si el requerimiento que pretende presentar es viable o no para la empresa, ello implica revisar si en efecto está dentro de las políticas y tiempos que tiene en sus lineamientos la organización para registrarlo, una vez se tiene dicha validación se procede a revisar si dentro del perfil el agente tiene el perfil para dar solución, en caso que sí pueda gestionarlo debe proceder a cerrarlo, en caso que no, debe escalarlo al área o persona que corresponda. En cualquiera de estos escenarios siempre deberá cerrar la gestión en el sistema de información o base de datos indicada en el procedimiento de la empresa. 
    p.mb-5 Para un mejor entendimiento de este tema se plantean los siguientes ejemplos:

    .row.mb-5
      .col-12.col-md-6.bgr_1.p-5.mb-3.mb-md-0(data-aos="zoom-in-right")
        figure.mb-3
          img.img90(src='@/assets/curso/tema4/t4-13.svg', alt='Texto que describa la imagen')
        h4 Agente de servicio con alcance para dar gestión al requerimiento y cerrarlo
        p El agente de servicio recibe una llamada de un cliente indicando que requiere realizar una devolución de un pedido que llegó con la talla equivocada, el primer paso que hace el agente es validar los datos de la persona que realiza la llamada, una vez realizada la revisión en el CRM y valida que efectivamente la persona sí hizo el pedido y que adicional se encuentra en los días hábiles para realizar el cambio del producto, por lo que procede a ingresarlo en el sistema de información y le informa al cliente que en el transcurso de 5 días hábiles recibirá el nuevo producto y deberá también tener listo el enviado previamente para entregarlo al domiciliario.
        p Estado del caso: cerrado.
      .col-12.col-md-6.bgr_2.p-5(data-aos="zoom-in-left")
        figure.mb-3
          img.img90(src='@/assets/curso/tema4/t4-14.svg', alt='Texto que describa la imagen')
        h4 Agente de servicio NO tiene alcance para dar gestión al requerimiento y escalarlo
        p El agente de servicio recibe una llamada de un cliente indicando que su servicio de Internet no funciona, el agente procede a realizar las validaciones sobre el usuario, una vez identifica que el suscriptor sí es quien dice ser, registra en el CRM el daño y le informa al cliente que el caso ha sido creado, escalando el caso para que sea atendido por el equipo de mantenimiento de redes quienes en el transcurso del día irán a su domicilio a resolver la situación.
        p Estado del caso: escalado.

    h3.mb-5(data-aos="zoom-in-left") Inclusión en la recepción de requerimientos desde el rol de agente de servicio

    p.mb-5 En un sentido amplio, la inclusión significa <b>considerar y valorar los diferentes puntos de vista</b> bajo las particularidades, estilos y necesidades de las personas. En este sentido, dado que el primer momento de verdad de un cliente cuando está escalando una solicitud a la empresa es la recepción del requerimiento, deben tenerse en cuenta algunas consideraciones en el momento de la interacción entre agente de servicio y cliente; por ello, revise con atención lo que se expone a continuación:

    SlyderD(:datos="datosSlyder")(data-aos="zoom-in-up")





</template>

<script>
export default {
  name: 'Tema3',
  data: () => ({
    modal1: false,
    modal2: false,
    datosSlyder: [
      {
        titulo: 'Empatía',
        texto:
          'Si bien las empresas tienen estipulados los protocolos de servicio, justamente con el fin de estandarizar procesos y formas de atención, desde la conversación y la forma de entablar la relación con el cliente los agentes de servicio deben mostrarse empáticos, y para ello hay una pregunta clave ¿qué haría si lo que está mencionado el cliente me estuviera pasando a mí?, frecuentemente ponerse en el lugar del otro, ayuda a tener relaciones más constructivas.',
        imagen: require('@/assets/curso/tema4/t4-15.png'),
      },
      {
        titulo: 'Escucha',
        texto:
          'El principio de una comunicación efectiva es la escucha, por eso, el agente de servicio debe tener esta actitud hacia su cliente, esto no solo le permitirá ser más asertivo en la forma de abordar el requerimiento, sino que también generará un ambiente de interés y confianza.',
        imagen: require('@/assets/curso/tema4/t4-16.png'),
      },
      {
        titulo: 'Flexibilidad',
        texto:
          'Ello no significa pasarse por alto el protocolo de servicio, al contrario, el reto es cómo aplicar el protocolo, mostrándose comprometido con el cliente en tratar de dar solución al requerimiento, implica buscar alternativas y espacios para la concertación. Bajo esta perspectiva se debe tener presente que flexibilidad no implica saltarse el debido proceso, ni pasar por encima de los lineamientos técnicos, lo que propende es aplicar el principio de la apertura.',
        imagen: require('@/assets/curso/tema4/t4-17.png'),
      },
      {
        titulo: 'Entender la individualidad',
        texto:
          'Si bien las personas son sujetos activos dentro de una comunidad, en el momento de interactuar con un cliente, se deben dejar de lado los estereotipos, las pretensiones y asociaciones negativas que se tengan, por el contrario, el enfoque de servicio actual se enfoca en brindar experiencias memorables a partir del entendimiento de la individualidad.',
        imagen: require('@/assets/curso/tema4/t4-18.png'),
      },
      {
        titulo: 'Respeto por la diferencia',
        texto:
          'Indistinto de las condiciones físicas, mentales, económicas o comportamentales, todos los clientes tienen como factor común ser seres humanos, por tanto, merecen tener consideración y valoración de sus necesidades, y bajo este panorama, donde los agentes de servicio son la cara de la empresa y deben ser los primeros embajadores del respeto.',
        imagen: require('@/assets/curso/tema4/t4-19.png'),
      },
    ],
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
