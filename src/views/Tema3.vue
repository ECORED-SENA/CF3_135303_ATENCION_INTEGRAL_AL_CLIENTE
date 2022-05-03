<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    .titulo-principal.color-acento-contenido
      .titulo-principal__numero
        span 3
      h1 Bases de datos
    
    .row  
      .col-12.col-md-4.mb-3(data-aos="zoom-in-right")
        figure
          img.img400(src='@/assets/curso/tema3/t3-1.png', alt='Texto que describa la imagen')
      .col-12.col-md-8.mb-3(data-aos="zoom-in-left")
        p Las bases de datos conocidas con las siglas BD (español) o DB (en inglés) o BBDD en términos informáticos, son estructuras diseñadas principalmente para <b>recopilar y alojar</b> información de diferentes tipos. En este sentido, podría afirmarse que varias bases de datos con fines específicos conforman en conjunto, es decir, un sistema de información.
        p Hoy en día las bases de datos son una herramienta importante en la gestión empresarial, dado que a través de ellas es posible alojar, actualizar o ingresar información, y de acuerdo con esto tienen usabilidad tanto para realizar actividades individuales como colectivas dentro de la organización. Asimismo, permiten capturar información de los clientes logrando de esta manera tener procesos estandarizados y centralizados para los datos que se generan en la compañía. También, agrupan los datos de la empresa, posibilita que los datos sean compartidos entre los colaboradores, y con esto tener procesos más estructurados y almacenar gran volumen de información. 
      p.mb-5 En términos prácticos, una base de datos tiene una composición sencilla, los datos son agrupados mediante <b>tablas,</b> y cada una está integrada por columnas y filas, cada fila con diversos datos y se denomina <b>registro</b> y, las columnas conocidas como <b>campos</b> contienen la información específica para cada registro. Con fines ilustrativos en la siguiente figura se muestra su estructura y en la tabla siguiente un ejemplo aplicado con dichos conceptos.
    
    .titulo-sexto.color-acento-contenido.mb-5(data-aos="zoom-in-right")
      h5 Figura 1
      span Estructura de una base de datos
    
    .row.justify-center.mb-5(data-aos="zoom-in-up")
      .col-12.col-md-8
        figure
          img.img800(src='@/assets/curso/tema3/t3-2.svg', alt='Texto que describa la imagen')      
   
    p.mb-5 En términos empresariales, la mayoría de bases de datos que se utilizan son las denominadas “relacionales” y tal cual como se evidencia en la estructura anterior, dentro de la base de datos, las tablas deben tener algún tipo de conexión que permita que todas ellas tengan un campo en común, lo cual en el esquema anterior se observa mediante las flechas.

    .titulo-sexto.color-acento-contenido.mb-5(data-aos="zoom-in-right")
      h5 Tabla 1
      span Ejemplo de una tabla de clientes de una empresa

    .bgr.mb-5
      .row.justify-center(data-aos="zoom-in-up") 
        .col-12.col-md-10.mt-5
          .tabla-a.bgr_6.mb-4 
            table
              thead
                tr
                  th.bgr_2 Apellido
                  th.bgr_2 Nombres
                  th.bgr_2 Empresa
                  th.bgr_2 Número de contacto
                  th.bgr_2 Correo electrónico
                  th.bgr_2 Municipio
              tbody
                tr
                  td Jaramillo Rojas
                  td Diana Carolina
                  td EPM
                  td 315 563 51 63
                  td diany@gmail.com
                  td Medellín
                tr
                  td López Escudero
                  td Gloria Amparo
                  td SENA
                  td 399 000 00 20
                  td gloria@gmail.com
                  td Bogotá D.C.
                tr
                  td Parra Guarín
                  td Nelly
                  td SENA
                  td 300 800 90 00
                  td nelly@gmail.com
                  td Neiva
                tr
                  td Cardona Grisales
                  td Esperanza
                  td Colpensiones
                  td 380 00 00 00
                  td espera@gmail.com
                  td Cali
          p.mb-5.p-3.p-md-0 De acuerdo con los conceptos vistos previamente, en la tabla expuesta se observan cuatro registros de clientes y para cada uno se relacionan seis campos: apellido, nombres, empresa, número de contacto, correo electrónico y municipio. En el entendimiento de las bases de datos se debe tener presente que la primera fila hace relación a los campos de la base de datos, por tanto, no se consideran registros.
    
    h2.mb-5(data-aos="zoom-in-left") Tipos de bases de datos

    p.mb-5 A nivel de informática existen varios tipos de bases de datos, lo anterior, dado que las bases de datos varían según el fin con el cual se almacenará la información y el posterior uso que se le dará a dicha información. En cuanto a lo que tiene que ver con servicio al cliente, se hará mención a dos de estas clasificaciones: según la variabilidad y según el contenido. A continuación, podrá apropiar los tipos de bases de datos de una forma más clara:

    .row
      .col-lg-4(data-aos="fade-up")
        .tarjeta-avatar-b.mb-5
          .tarjeta-avatar-b__img
            img.img90(src='@/assets/curso/tema3/t3-3.svg' alt='AvatarTop')
          .tarjeta.bgr_7
            .p-4
              div
                h2 Variabilidad
                p.m-0 Estáticas
                p.m-0 Dinámicas
      .col-lg-4(data-aos="fade-down")
        .tarjeta-avatar-b.mb-5
          .tarjeta-avatar-b__img
            img.img90(src='@/assets/curso/tema3/t3-4.svg' alt='AvatarTop')
          .tarjeta.bgr_7
            .p-3
              div
                h2 Según el contenido
                p.m-0 Bibliográficas
                p.m-0 De texto completo
                p.m-0 De directorio
      .col-lg-4(data-aos="fade-up")
        .tarjeta-avatar-b.mb-5
          .tarjeta-avatar-b__img
            img.img90(src='@/assets/curso/tema3/t3-5.svg' alt='AvatarTop')
          .tarjeta.bgr_7
            .p-4
              div
                h2 Según los modelos
                p.m-0 Transaccionales
                p.m-0 Relacionales
    
    h3.mb-5(data-aos="zoom-in-left") Bases de datos según la variabilidad

    p.mb-5 La agrupación con base en la variabilidad se da a partir del modelo en que los datos están estructurados dentro de la base de datos. En esta categoría existen dos tipos que son:

    .row.mb-5.justify-center
      .col-12.col-md-10
        .row
          .col-md-6.col-lg.mb-5.mb-lg-0(data-aos="fade-up")
            .tarjeta-avatar
              img.posit_3(src='@/assets/curso/tema3/t3-6.svg' alt='AvatarTop')
              .tarjeta.bgr_4
                .p-4
                  h2 Estáticas:
                  p Son diseñadas exclusivamente con fines de lectura, almacenamiento y registro de datos históricos, sin embargo, luego son susceptibles de uso para análisis de proyecciones y comportamientos de una determinada variable. Por ejemplo, la empresa puede tener una base de datos del histórico de devoluciones que se han realizado en el último año, dicha información puede ser consultada o ser utilizada para dimensionar los recursos necesarios con el fin de poder atender dichos trámites al año siguiente. En este caso, la variable son las devoluciones y la utilidad será predecir la cantidad de agentes necesarios para atender este tipo de solicitudes.
          .col-md-6.col-lg.mb-5.mb-lg-0(data-aos="fade-down")
            .tarjeta-avatar
              img.posit_3(src='@/assets/curso/tema3/t3-7.svg' alt='AvatarTop')
              .tarjeta.bgr_8
                .p-4
                  h2 Dinámicas:
                  p Son diseñadas exclusivamente con fines de lectura, almacenamiento y registro de datos históricos, sin embargo, luego son susceptibles de uso para análisis de proyecciones y comportamientos de una determinada variable. Por ejemplo, la empresa puede tener una base de datos del histórico de devoluciones que se han realizado en el último año, dicha información puede ser consultada o ser utilizada para dimensionar los recursos necesarios con el fin de poder atender dichos trámites al año siguiente. En este caso, la variable son las devoluciones y la utilidad será predecir la cantidad de agentes necesarios para atender este tipo de solicitudes.

    h3.mb-5(data-aos="zoom-in-left") Bases de datos según el contenido      

    p.mb-5 Esta tipología responde a la categorización del contenido a partir del cual se espera dar la usabilidad a los datos. Allí, se identifican tres tipos que son: 

    .row.justify-center.mb-5(data-aos="zoom-in-up")
      .col-12.col-md-10(data-aos="zoom-in-down")
        AcordionA.mb-5(tipo="a" clase-tarjeta="tarjeta tarjeta--azul")
          .row(titulo="Bases de datos bibliográficas. ")
            .col-md-4.mb-4.mb-md-0
              figure.justify-center
                img.img200(src='@/assets/curso/tema3/t3-8.png', alt='Texto que describa la imagen')
            .col-md-8.align-items-center
              p.m-0 Las bases de datos <b>bibliográficas</b> son aquellas que permiten recopilar información que responde a áreas de conocimiento específico, especialmente relacionadas con publicaciones académicas o técnicas; a nivel de tecnología se recogen en catálogos informáticos, por ejemplo, los investigadores tienen como la mejor fuente de búsqueda de información las bases de datos bibliográficas porque consolidan las referencias alrededor de temáticas específicas.
          .row(titulo="Bases de datos de texto completo. ")
            .col-md-4.mb-4.mb-md-0
              figure.justify-center
                img.img200(src='@/assets/curso/tema3/t3-9.png', alt='Texto que describa la imagen')
            .col-md-8.align-items-center
              p.m-0 Las <b>bases de datos de texto completo</b> posibilitan la búsqueda de información a partir de <em>key words</em> (palabras clave), la diferencia con las bases de datos bibliográficas es que en estas se podrá tener acceso a la información completa, por ejemplo, Google es una base de datos de texto completo, ya que al ingresar en el buscador se puede acceder inmediatamente a consultar el documento, imagen o video que se requiera.
          .row(titulo="Bases de datos de directorio.")
            .col-md-4.mb-4.mb-md-0
              figure.justify-center
                img.img200(src='@/assets/curso/tema3/t3-10.png', alt='Texto que describa la imagen')
            .col-md-8.align-items-center
              p.m-0 Las bases de datos de tipo <b>directorio</b> alojan la información específica de un grupo de interés de la compañía, entendiendo estos como aquellos grupos con los cuales la empresa tiene relación constante, a nivel general son: los colaboradores, clientes, proveedores, distribuidores, entres de control, entre otros. Dichas bases de datos son de alta relevancia, ya que permiten organizar la información según los requerimientos puntuales que se tengan, por ejemplo, una base de datos que aloje la información de los colaboradores de la compañía relacionando sus datos de nombres, fecha de nacimiento, estado civil, estudios y datos de contacto.

    h3.mb-5(data-aos="zoom-in-left") Bases de datos según el modelo

    p.mb-5 Esta es la clasificación más técnica en términos informáticos de las bases de datos y se interpretan como la forma en que se administran los datos al interior de las mismas. Tienen varios tipos; sin embargo, las más usadas en el contexto empresarial son: 

    .row.mb-5.justify-center
      .col-12.col-md-2(data-aos="fade-up")
        .titulo-sexto.color-primario
          span Las <b>transaccionales.</b>
      .col-12.col-md-2(data-aos="fade-down")
        .titulo-sexto.color-secundario
          span Las <b>relacionales.</b>
    
    p.mb-5 Las bases de datos <b>transaccionales</b> están orientadas a todo tipo de procesos, tanto básicos como complejos y tienen como característica fundamental que realizan una función determinada, adicionalmente que tienen la ventaja que envían y recepcionan datos a gran velocidad. Por su parte, las bases de datos relacionales, que son hoy en día las más utilizadas optimizan los procesos al interior de las tablas, es decir, el centro de este modelo son las “relaciones” entre datos.

    .row.justify-center.mb-5
      .col-12.col-md-8(data-aos="zoom-in-up")
        .cajon.bgr_9.p-5.mb-4
          p.m-0 Ambos tipos de bases de datos (transaccionales y relacionales) están desarrolladas bajo plataformas denominadas motores de bases de datos como Access, MySQL, Oracle, entre otras y estas a su vez se encuentran conectadas con lenguajes de programación, es decir, con códigos específicos, tales como Phyton, C++, Visual Basic, HTML, etc. y en este sentido la combinación entre un motor de base de datos y el lenguaje de programación da como resultado software (programas) con funciones específicas.

    h3.mb-5(data-aos="zoom-in-left") Registro de información en bases de datos

    .row.mbottom 
      .col-12.col-md-4.mb-3(data-aos="zoom-in-right")
        figure
          img.img400(src='@/assets/curso/tema3/t3-11.png', alt='Texto que describa la imagen')
      .col-12.col-md-8.mb-3(data-aos="zoom-in-left")
        p En términos operativos de bases de datos, se entiende registro de información como el proceso mediante el cual una persona o un bot (robot que hace tareas operativas) ingresa información en un sistema, lo cual va originando algo que se conoce como “alimentar” la base de datos y es realizado a través de un usuario, que es aquella persona que tiene la potestad de ingresar a una DB o a un S.I.
        p Para el registro de información en la base de datos se deben tener presente los roles, entendidos estos como el tipo de accesos que se permiten a cada usuario, en este sentido asociado al tratamiento de bases de datos a nivel estándar se tienen los siguientes roles:

    .row.mb-5
      .col-md-4.col-lg.mb-5.mb-lg-0(data-aos="fade-up")
        .tarjeta-avatar
          img.posit_4(src='@/assets/curso/tema3/t3-12.svg' alt='AvatarTop')
          .tarjeta.bgr_10
            .p-4
              h4.text-center Rol Administrador
              p Es aquel que tiene la facultad de realizar cualquier tipo de acciones sobre la base de datos, asociado tanto a los datos como a los usuarios.
      .col-md-4.col-lg.mb-5.mb-lg-0(data-aos="fade-down")
        .tarjeta-avatar
          img.posit_4(src='@/assets/curso/tema3/t3-13.svg' alt='AvatarTop')
          .tarjeta.bgr_10
            .p-4
              h4.text-center Rol de Registro y Edición
              p Este tipo de roles están asociados a aquellos usuarios que ingresan, procesas y/o modifican los datos.
      .col-md-4.col-lg.mb-5.mb-lg-0(data-aos="fade-up")
        .tarjeta-avatar
          img.posit_4(src='@/assets/curso/tema3/t3-14.svg' alt='AvatarTop')
          .tarjeta.bgr_10
            .p-4
              h4.text-center Rol de Consulta
              p Estos usuarios pueden ingresar a la base de datos con la finalidad de detallar la información y algunos casos, bajar información; sin embargo, no pueden modificar.
    
    p.mb-5 De acuerdo con los roles, en cada empresa realizan sobre las bases de datos la asignación de perfiles, entendiendo este último concepto como la asociación para cada rol de transacciones (operaciones) específicas que puede realizar el usuario. A modo de ejemplo y para mayor comprensión se presenta esta situación: 

    .row.justify-center(data-aos="fade-down").mb-5
      .col-12.col-md-2.bgr_11.justify-center.p-4
        img.img160(src='@/assets/curso/tema3/t3-15.svg' alt='AvatarTop')
      .col-12.col-md-6.bgr_12
        p.m-0 <b>Diana Carolina</b> es agente de servicio enfocada en la recepción de pedidos, por tanto, desde su rol de registro y edición tiene un perfil para ingresar pedidos, mientras que <b>María Valentina</b> que es una agente de servicio en el contact center, enfocada en brindar información a los clientes tiene asociado a su rol de consulta un perfil para consultar los pedidos de los clientes.
      .col-12.col-md-2.bgr_11.justify-center.p-4
        img.img160(src='@/assets/curso/tema3/t3-16.svg' alt='AvatarTop')
      p.mt-5 Según lo anterior, cada quien tendrá según su rol y perfil, diferentes formas de interactuar con las bases de datos. En este caso si María Valentina quisiera ingresar un pedido no lo podría realizar, dado que tiene asociado exclusivamente acceso en modo consulta, por lo que Diana Carolina tiene acceso a poder realizar más acciones sobre la base de datos que María Valentina consulta.
    
    h3.mb-5(data-aos="zoom-in-left") Seguridad de la información
    
    p.mb-5 Dado que hoy en día la información es uno de los activos más importantes en una organización, en temas de bases de datos, no solo es importante garantizar el ingreso de información sino también asegurar la disponibilidad, actualización y alojamiento en pro de la continuidad del negocio. Se invita, a continuación, a que revise más sobre este importante tema:

    .row  
      .col-12.col-md-6.mb-3(data-aos="zoom-in-right")
        div.bgr_13.p-3
          .row
            .col-3.align-items-center
                img.img160(src='@/assets/curso/tema3/t3-17.png' alt='AvatarTop')
            .col-9
                h4 <em>Back-up</em>
                p Las empresas deben tener por su seguridad un back-up (respaldo), que permita que en caso de que se tenga alguna falla técnica de tipo informático sea posible seguir contando con la información.
                p.m-0 Técnicamente los back-up tienen por fin garantizar que la misma información se encuentre disponible mínimo en dos repositorios diferentes, ya sea físicos (instalaciones de la empresa) o en nube (servidores por fuera de ella), esto permitirá hacer frente a los ataques informáticos o errores humanos.      
      .col-12.col-md-6(data-aos="zoom-in-left")
        div.bgr_14.p-3
          .row
            .col-3.align-items-center
                img.img160(src='@/assets/curso/tema3/t3-18.png' alt='AvatarTop')
            .col-9
                h4 ISO 27001 de 2013
                p.m-0 Las empresas enfocadas en garantizar buenos procesos de gestión de la información cuentan con la ISO 27001 de 2013, que está enfocada en dar lineamientos sobre cómo las organizaciones deberán gestionar la información de forma segura y si bien las Normas ISO no son obligatorias, sí se convierten en lineamientos para las buenas prácticas empresariales.
 


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
