<template>
  <v-container>
    <v-layout mt-5>
      <v-flex xs12>
        <h1>Elementos de la arquitectura cliente/servidor.</h1>
        <p
          class="text-justify"
        >De lo dicho hasta ahora, podemos deducir que los principales elementos que conforman la arquitectura cliente/servidor son los siguientes:</p>

        <h2>El servidor</h2>

        <p class="text-justify">
          Cuando hablamos de una forma genérica, si mencionamos a un servidor, nos referimos a un ordenador, normalmente con prestaciones elevadas, que ejecuta servicios para atender las demandas de diferentes clientes.
          Sin embargo, bajo el punto de vista de la arquitectura cliente/servidor, un servidor es un proceso que ofrece el recurso (o recursos) que administra a los clientes que lo solicitan (consultar la definición de cliente más abajo). Es muy frecuente que, para referirse a un proceso servidor, se utilice el término back-end. Según el tipo de servidor implantado, tendremos un tipo de arquitectura cliente/servidor diferente. Por último, mencionar que en algunas ocasiones, un servidor puede actuar, a su vez, como cliente de otro servidor
        </p>

        <h2>El cliente</h2>

        <p class="text-justify">
          Igual que antes, al hablar de forma genérica sobre un cliente, nos referimos a un ordenador, normalmente con prestaciones ajustadas, que requiere los servicios de un equipo servidor. Sin embargo, bajo el punto de vista de la arquitectura cliente/servidor, un cliente es un proceso que solicita los servicios de otro, normalmente a petición de un usuario. En entornos cliente/servidor, suele utilizarse el término front-end para referirse a un proceso cliente.
        </p>
        <p class="text-justify">
          Normalmente, un proceso cliente se encarga de interactuar con el usuario, por lo que estará construido con alguna herramienta que permita implementar interfaces gráficas (GUI). Además, se encargará de formular las solicitudes al servidor y recibir su respuesta, por lo que deberá encargarse de una parte de la lógica de la aplicación y de realizar algunas validaciones de forma local.
        </p>

        <h2>El Middleware</h2>

        <p class="text-justify">
          Es la parte del software del sistema que se encarga del transporte de los mensajes entre el cliente y el servidor, por lo que se ejecuta en ambos lados de la estructura. El middleware permite independizar a los clientes y a los servidores, sobre todo, gracias a los sistemas abiertos, que eliminan la necesidad de supeditarse a tecnologías propietarias. Por lo tanto, el middleware facilita el desarrollo de aplicaciones, porque resuelve la parte del transporte de mensajes y facilita la interconexión de sistemas heterogéneos sin utilizar tecnologías propietarias.
        </p>

        <p class="text-justify">
          Además, ofrece más control sobre el negocio, debido a que permite obtener información desde diferentes orígenes (uniendo tecnologías y arquitecturas distintas) y ofrecerla de manera conjunta.
        </p>

        <p class="text-justify">Podemos estructurar el middleware en tres niveles: </p>
        <ul>
            <li>El protocolo de transporte, que será común para otras aplicaciones del sistema.</li>
            <li>El sistema operativo de red</li>
            <li>El protocolo del servicio, que será específico del tipo de sistema cliente/servidor que estemos considerando.</li>
        </ul>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "Elementos"
};
</script>