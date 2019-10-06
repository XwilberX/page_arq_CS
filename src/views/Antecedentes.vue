<template>
  <v-container>
    <v-layout mt-5>
      <v-flex xs12>
        <h1>Antecedentes</h1>
        <h2>Breve historia de los sistemas distribuidos</h2>
        <p
          class="text-justify"
        >Los sistemas distribuidos existen en el mundo de la informática en una u otra forma desde hace algún tiempo, aunque no se hayan llamado explícitamente sistemas distribuidos y no tuviesen la flexibilidad que tienen hoy en día. Al principio sólo existían los grandes ordenadores o mainframes en los que se ejecutaban Sistemas de gestión de Base de Datos (SGBD) jerárquicos. La conexión de los usuarios con el ordenador central se hacía mediante terminales tontas con conexiones punto a punto con el servidor. Los grandes ordenadores tenían un coste muy elevado y eran difíciles de mantener, pero eran capaces de dar servicio a un número muy elevado de usuarios y tenían la ventaja (o desventaja) de ser administrados de forma centralizada. En este tipo de sistemas el software era monolítico, es decir, el interfaz de usuario, la lógica de negocio y el acceso a las bases de datos estaba todo contenido en una gran aplicación que se ejecutaba en el mainframe. Dado que las terminales utilizadas para conectarse al ordenador central no tenían ninguna capacidad de proceso, la aplicación entera se ejecutaba completamente en el ordenador central.</p>
        
        <p
          class="text-justify"
        >La aparición de los PCs introdujo un cambio muy importante en las arquitecturas monolíticas y las aplicaciones para ellas desarrolladas. Las nuevas aplicaciones basadas en el paradigma cliente/servidor permitieron que parte del procesamiento realizado en el servidor fuese descargado a los PCs cliente. Las aplicaciones cliente/servidor normalmente distribuyen los componentes de la aplicación de forma que la base de datos reside en el servidor, el interfaz de usuario reside en el cliente, y la lógica de negocio puede residir tanto en el cliente (en forma de código), como en el servidor (en forma de procedimientos almacenados) o en ambos. Con la llegada de la arquitectura cliente/servidor multicapa la arquitectura cliente/servidor original pasó a llamarse cliente servidor de dos capas.</p>

        <p
          class="text-justify"
        >La arquitectura cliente/servidor fue en algunos aspectos una revolución que cambió la vieja forma en que se hacían las cosas. A pesar de resolver muchos de los problemas de las aplicaciones basadas en mainframes, la arquitectura cliente/servidor tenía sus propios problemas. Por ejemplo, como la lógica de negocio y el acceso a la base de datos estaban contenidos normalmente en la parte cliente, cualquier cambio de la lógica de negocio, en el acceso a la base de datos o en la propia base de datos requerirá a menudo actualizar la parte cliente de todos los usuarios de la aplicación. Los problemas con esta tradicional arquitectura cliente/servidor, a menudo denominada cliente/servidor de dos capas fueron resueltos con lo que se conoce con el nombre de cliente/servidor multicapa. Conceptualmente, una aplicación puede tener cualquier número de capas, pero las arquitecturas multicapa suelen tener sólo tres capas. Estas arquitecturas dividen la arquitectura del sistema en tres capas lógicas:</p>
        <ol class="text-justify">
          <li>La capa de interfaz con el usuario.</li>
          <li>La capa de reglas o lógica de negocio.</li>
          <li>La capa de acceso a la base de datos.</li>
        </ol>
        <br />
        <p
          class="text-justify"
        >De esta forma, el cliente es básicamente una interfaz, que no tiene por qué cambiar si cambian las especificaciones del negocio. Las arquitecturas cliente/servidor multicapa mejoran a las arquitecturas de dos capas en dos aspectos fundamentalmente:</p>

        <ol class="text-justify">
          <p
            class="text-justify"
          >1. Hace a la aplicación más robusta al aislar al cliente de los cambios en el resto de la aplicación. La capa de interfaz de usuario se comunica solo con la capa de lógica de negocio, nunca directamente con la capa de acceso a la base de datos. La capa de lógica de negocio se comunica por un lado con la capa de interfaz de usuario y por otro lado con la capa de acceso a la base de datos. De esta forma un cambio en la base de datos no afecta a la parte cliente que recordemos que es la que tiene que ser redistribuida si se producen cambios en ella.</p>
          <p
            class="text-justify"
          >2. Dado que la arquitectura multicapa particiona la aplicación en más componentes que la arquitectura tradicional cliente/servidor, también permite una mayor flexibilidad en la utilización de la aplicación.</p>
        </ol>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: "Antecedentes"
};
</script>
