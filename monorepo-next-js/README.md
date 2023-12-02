# Crear un monorepo con Next JS

Vas a actuar como un programador especializado en Next JS y TypeScript.

Soy analista programador y mi trabajo consiste en revisar el código de otros programadores y crear la documentación de un programa para enviarla al cliente. En algunas ocasiones necesito realizar tareas de programación que me quitan mucho tiempo y quiero que seas tu quien realice esas tareas de programación. Actualmente tengo un proyecto realizado en Next JS con TypeScript. No hay ningún fichero js, todos los ficheros son tsx y ts. El proyecto está finalizado al 100% preparado para subir a producción una vez se realizan unos ajustes:

Tu tarea es la siguiente. Dentro del proyecto de Next JS tengo la siguiente estructura de directorios:

./ => directorio raíz
./app
/app/components
/app/directorio1/app
/app/directorio2/app
/app/directorio3/app

la carpeta app del directorio raíz y la carpeta app de directorio1, directorio2 y directorio3 tienen los siguientes archivos de TypeScript: [NOMBRE-FICHERO] y [NOMBRE-FICHERO] A continuación te dejo un ejemplo del contenido de ambos ficheros:

fichero [NOMBRE-FICHERO]
[CODIGO]

fichero [NOMBRE-FICHERO]
[CODIGO]

Como te he dicho, el proyecto es 100% Typescript por eso te dejo el contenido del fichero [NOMBRE-FICHERO]
[CODIGO]


Lo que tienes que hacer es convertir directorio1, directorio2, directorio3 en monorepos pero se tienen que cumplir las siguientes condiciones:

1. todo tiene que ser con npm. No puedes usar yarn, pnpm ni ningún otro gestor de paquetes o librerías externas

2. los monorepos son individuales así que cada directorio tiene que tener su propio package.json

3. los monorepos tienen que tener un fichero tsconfig.json pero quiero que hereden la configuración el fichero tsconfig.json que se encuentra en el directorio raíz

4. los monrepos tienen que ejecutarse de manera individual, es decir cada uno tiene que tener su propio start y build y funcionar como proyectos independientes

5. cada monorepo tiene que tener las librerias y configuraciones necesarias para ejecutar jsx

6. en la carpeta componentes que se encuentra dentro de app en el directorio raíz (./app/components) tengo componentes que quiero que sean compartidos entre los diferentes monorepos. Es decir, si por ejemplo tengo un componente llamado ComponenteCompartido.tsx quiero que pueda ser usado en directorio1, directorio2 y directorio3. Configura el fichero tsconfig.json y next.config.js o next.config.ts para aceptar las importaciones por alias de typescript.