<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: ActividadController(:cuestionario="cuestionario") 
      // Para parrafo usar: ActividadController(:parrafo="parrafo")
      ActividadController(:cuestionario="cuestionario")
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Ventas en el formato comercial',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la comprensión de los conceptos fundamentales relacionados con la publicidad en el punto de venta, la promoción, los eventos promocionales, los productos y servicios, el portafolio de productos, la estrategia comercial de ventas, las técnicas de venta, las buenas prácticas de manufactura, las demostraciones, las degustaciones, la comunicación comercial, el material publicitario y la omnicanalidad en el <i>retail</i>. ',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO',
      preguntas: [
        {
          id: 1,
          texto:
            'La publicidad en el punto de venta se diferencia de otras acciones comerciales porque:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Se ubica dentro del establecimiento, cerca del producto, para comunicar de forma persuasiva en el momento de compra.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Reemplaza el diseño del envase y no requiere relación con el producto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Solo se usa fuera del establecimiento para atraer transeúntes.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Tiene como finalidad exclusiva controlar el inventario del almacén.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 2,
          texto:
            'Cuando una pieza publicitaria comunica características, beneficios, precios o promociones de un producto, cumple principalmente la función de:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Recordar únicamente la marca sin aportar información.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Informar al cliente para orientar su decisión de compra.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Sustituir el servicio de asesoría comercial.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Cerrar automáticamente la venta sin interacción del cliente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 3,
          texto:
            'Si una marca desea que el cliente mantenga presente un producto para futuras necesidades, la publicidad está cumpliendo el objetivo de:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Eliminar la competencia del establecimiento.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Cambiar el diseño físico del local.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Recordar la marca, el producto o el lugar donde puede adquirirse.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Reducir todos los precios de la categoría.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 4,
          texto: 'Una promoción de ventas resulta eficaz cuando:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es compleja para que el cliente tarde más en comprenderla.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'No se comunica al público hasta finalizar la campaña.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Se dirige solo al personal interno y evita al consumidor.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Es conocida, comprendida, atractiva y percibida como alcanzable por el cliente.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 5,
          texto: 'Una promoción estratégica se caracteriza porque:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Puede buscar comportamientos presentes o futuros, como probar un producto nuevo junto a uno conocido.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Tiene como único objetivo aumentar las ventas de inmediato.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Elimina la necesidad de planear la campaña de comunicación.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Solo se aplica cuando no existe competencia en el mercado.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 6,
          texto:
            'La publicidad utilizada para fortalecer el posicionamiento de una marca dentro del establecimiento corresponde principalmente a:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Publicidad institucional o de imagen.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Publicidad exclusivamente normativa.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Publicidad destinada únicamente al control de inventarios.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Publicidad enfocada en reemplazar el empaque del producto.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 7,
          texto:
            'Los elementos de comunicación visual ubicados dentro del establecimiento hacen parte del <i>marketing</i>:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Industrial.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Financiero.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'En el punto de venta.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Exclusivamente digital.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 8,
          texto: 'Un <i>stand custom</i> se caracteriza principalmente porque:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Es diseñado de forma personalizada para comunicar la identidad de una marca o producto.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Tiene siempre el mismo diseño para cualquier empresa.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Se utiliza únicamente para almacenar mercancía.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Reemplaza completamente la exhibición de productos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 9,
          texto:
            'En un establecimiento de <i>retail</i>, la publicidad en el punto de venta busca principalmente:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Facilitar la decisión de compra mediante información y estímulos visuales.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Sustituir la atención del personal de ventas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Eliminar la exhibición física de los productos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Reducir el número de referencias disponibles para el cliente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 10,
          texto: 'El material POP cumple principalmente la función de:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Apoyar la comunicación y promoción del producto en el punto de venta.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Reemplazar el inventario físico del establecimiento.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Controlar los procesos contables de la empresa.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Sustituir la capacitación del personal comercial.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 11,
          texto:
            'Una estrategia comercial de ventas debe partir del contexto porque:',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Permite omitir los objetivos y trabajar solo con promociones.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Impide usar canales digitales en la comunicación comercial.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La situación actual de la empresa y sus variables internas y externas orientan las acciones posibles.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Toda empresa debe aplicar exactamente la misma estrategia que su competencia.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 12,
          texto:
            'La diferencia entre estrategia de <i>marketing</i> y estrategia comercial de ventas es que:',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La estrategia comercial solo se ocupa del diseño gráfico de las piezas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'La estrategia de <i>marketing</i> solo aplica a clientes fidelizados.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Ambas tienen el mismo fin y no requieren diferenciación.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'La estrategia de <i>marketing</i> genera oportunidades y la comercial aprovecha esas oportunidades para lograr rentabilidad.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 13,
          texto:
            'Para diseñar una estrategia comercial efectiva, el uso de la matriz DOFA permite:',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Analizar el contexto y la filosofía empresarial para orientar las acciones comerciales.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Eliminar la necesidad de conocer a los clientes.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Fijar precios sin estudiar el mercado.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Reemplazar los responsables, plazos e indicadores.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 14,
          texto: 'Las ventas electrónicas se caracterizan porque:',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Dependen exclusivamente de visitas puerta a puerta.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Se apoyan en la transferencia de datos mediante canales digitales como correo, redes, sitios web o mensajería.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Solo pueden realizarse por televisión.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No permiten planear acciones de venta.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 15,
          texto:
            'En buenas prácticas de manufactura, si se sospecha que una materia prima es inadecuada, se debe:',
          imagen: require('@/assets/actividad/imagen05.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Mezclarla con producto terminado para evitar desperdicios.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Usarla rápidamente antes de que se deteriore.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Aislarla, rotularla y eliminarla según el procedimiento establecido.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Guardarla junto al producto terminado hasta decidir su destino.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 16,
          texto:
            'La limpieza en seco se diferencia de la limpieza en húmedo porque:',
          imagen: require('@/assets/actividad/imagen6.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Utiliza detergente y abundante agua en todas las superficies.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Solo se permite en superficies de contacto directo con alimentos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Reemplaza los planes de desinfección y monitoreo ambiental.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Elimina suciedad seca sin usar agua, mediante aspiradora, soplador, escoba, cepillo o raspador.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 17,
          texto: 'Una demostración comercial fortalece la venta porque:',
          imagen: require('@/assets/actividad/imagen7.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Presenta pruebas, hechos y beneficios del producto para convencer y entusiasmar al cliente.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Evita que el cliente conozca el uso real del producto.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Sustituye todos los argumentos del asesor comercial.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Solo sirve para productos que no requieren explicación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 18,
          texto:
            'La degustación en el punto de venta tiene como objetivo principal:',
          imagen: require('@/assets/actividad/imagen8.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Evitar que el cliente pruebe el producto antes de comprarlo.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Permitir que el cliente pruebe el producto para motivar la compra y medir su reacción.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Reemplazar el control de inventario de alimentos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Reducir la presencia de impulsadores en zonas de alta circulación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 19,
          texto:
            'En la comunicación comercial, el nivel corporativo se orienta principalmente a:',
          imagen: require('@/assets/actividad/imagen9.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Definir únicamente promociones de precio.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Vender solo productos nuevos en el punto de venta.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Construir, defender y mantener la reputación de la marca.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Reemplazar la comunicación interna de la empresa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },

        {
          id: 20,
          texto: 'La omnicanalidad se diferencia de la multicanalidad porque:',
          imagen: require('@/assets/actividad/imagen10.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Usa canales separados sin compartir información entre ellos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Se limita a abrir redes sociales sin integrarlas con la tienda física.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Elimina la necesidad de conocer el recorrido del cliente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Integra canales físicos y digitales para ofrecer una experiencia coherente y sin interrupciones.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto: 'Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: 'Ha superado la actividad. ',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica. ',
    },
  }),
}
</script>
