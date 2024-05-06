# Tutorial de [https://nodejs.org/en](Node.js)

En este tutorial, aprenderás los conceptos básicos de Node.js y cómo empezar a construir aplicaciones web utilizando este entorno de ejecución de JavaScript del lado del servidor.

![NodeJs in 5](https://www.youtube.com/watch?v=_h-pj7YqHQw&t=206s&ab_channel=Jayanam)

## Instalación de Node.js

Para empezar, necesitarás instalar Node.js en tu máquina. Puedes descargar la última versión estable desde el sitio web oficial de Node.js: [nodejs.org](https://nodejs.org).

## Creación de un proyecto de Node.js

Una vez que hayas instalado Node.js, puedes crear un nuevo proyecto de Node.js utilizando el siguiente comando en tu terminal:

## Creación de un archivo package.json

El archivo `package.json` es un archivo fundamental en cualquier proyecto de Node.js. Este archivo contiene metadatos sobre tu aplicación, como el nombre, la versión, la descripción, los autores, las dependencias y mucho más.

Para crear un archivo `package.json`, puedes utilizar el comando `npm init`. Este comando te guiará a través de un proceso de preguntas para ayudarte a configurar tu archivo `package.json`.

```bash
npm init
```

¿Qué es el archivo package-lock.json?
El archivo package-lock.json es un archivo que se genera automáticamente cuando instalas paquetes a través de npm. Este archivo contiene información detallada sobre el árbol de dependencias de tu proyecto, incluyendo las versiones exactas de cada paquete que se ha instalado.

Este archivo es importante porque asegura que todos los que trabajan en el proyecto están utilizando las mismas versiones de los paquetes, lo que ayuda a prevenir errores y discrepancias.

Instalación de paquetes
Para instalar un paquete en tu proyecto de Node.js, puedes utilizar el comando npm install. Por ejemplo, si quisieras instalar el paquete express, podrías hacerlo con el siguiente comando:

```bash
npm install express
```

Esto instalará el paquete `express` en tu proyecto y agregará una entrada en el archivo `package.json` en la sección de dependencias. También generará o actualizará el archivo `package-lock.json` con la versión exacta del paquete que se ha instalado.

## ¿Qué es el archivo package-lock.json?

El archivo `package-lock.json` es un archivo que se genera automáticamente cuando instalas paquetes a través de npm, el gestor de paquetes de Node.js. Este archivo contiene información detallada sobre el árbol de dependencias de tu proyecto, incluyendo las versiones exactas de cada paquete que se ha instalado.

El propósito principal de este archivo es asegurar que la estructura de la carpeta `node_modules` sea idéntica en todas las instalaciones, independientemente de las actualizaciones de paquetes intermedias. Esto se logra especificando una versión exacta, ubicación y hash de integridad para cada paquete y subpaquete en tu proyecto.

### ¿Por qué es importante el archivo package-lock.json?

El archivo `package-lock.json` es importante por varias razones:

1. **Consistencia**: Asegura que todos los que trabajan en el proyecto están utilizando las mismas versiones de los paquetes, lo que ayuda a prevenir errores y discrepancias causadas por diferencias en las versiones de los paquetes.

2. **Eficiencia**: Al tener un registro detallado de la estructura exacta de la carpeta `node_modules`, npm puede evitar hacer solicitudes de red innecesarias cuando se instalan paquetes, lo que puede acelerar el proceso de instalación.

3. **Seguridad**: El archivo `package-lock.json` incluye hashes de integridad para cada paquete, lo que permite a npm verificar que los paquetes no han sido alterados desde que se instalaron.

### ¿Debería incluir el archivo package-lock.json en el control de versiones?

Sí, se recomienda incluir el archivo `package-lock.json` en tu sistema de control de versiones. Esto asegura que todos los que trabajan en el proyecto utilizan exactamente las mismas versiones de los paquetes, lo que ayuda a mantener la consistencia y prevenir errores.

## [https://vitejs.dev/](Vite)

### ¿Qué es Vite y cómo funciona?

Vite es un entorno de desarrollo para aplicaciones web modernas que se centra en la velocidad. Funciona cambiando la forma en que se desarrollan y se sirven las aplicaciones web durante el proceso de desarrollo.

En lugar de compilar todo el código antes de servirlo al navegador, como hacen otros marcos de trabajo como Webpack, Vite utiliza ESM (ECMAScript Modules) para servir módulos directamente al navegador durante el desarrollo. Esto significa que el código se compila y se sirve de manera incremental y bajo demanda, lo que resulta en tiempos de compilación rápidos y una experiencia de desarrollo ágil.

![Vite in 5 minutes](https://www.youtube.com/watch?v=KCrXgy8qtjM)

### Gestión de variables de entorno en Vite

Vite permite gestionar variables de entorno a través de archivos .env. Aquí hay un ejemplo de cómo hacerlo:

```env

VITE_API_URL=https://api.example.com
VITE_DEBUG=true

```

Al usar al inicio de cada variable la palabra `VITE_` no existe la necesidad de utilizar un paquete que maneje las variables de entorno como `dotenv`.

## [https://es.react.dev/](React)

![React in 5 minutes](https://www.youtube.com/watch?v=s2skans2dP4&ab_channel=DennisIvy)

## Instalación de React

Para instalar React, necesitarás tener Node.js y npm instalados en tu máquina. Una vez que los tengas, puedes instalar `create-react-app`, que es una herramienta de línea de comandos que te permite crear nuevos proyectos de React.

```bash
npx create-react-app my-app
```

Este comando creará un nuevo directorio llamado `my-app` con un proyecto de React inicializado.

## Creación de un proyecto de React

Para crear un nuevo proyecto de React, puedes utilizar el comando `create-react-app` seguido del nombre de tu proyecto. Por ejemplo, si quisieras crear un proyecto llamado `my-react-app`, podrías hacerlo con el siguiente comando:

```bash
npx create-react-app my-react-app
```

Esto creará un nuevo directorio llamado `my-react-app` con un proyecto de React inicializado. Dentro de este directorio, encontrarás varios archivos y directorios que forman la estructura básica de un proyecto de React.

Para iniciar tu aplicación, navega al directorio de tu proyecto y ejecuta el comando `npm start`:

```bash
cd my-react-app
npm start
```

Esto iniciará el servidor de desarrollo y abrirá tu aplicación en un navegador web.

Si bien este es la forma de crear un proyecto normal, para nuestro caso no es necesario utilizarlos, pero es importante conocerlo para nuestra futura creación de proyectos.

## npx vs npm

`npm` y `npx` son dos herramientas que vienen con Node.js, pero se utilizan para diferentes propósitos.

**npm** (Node Package Manager) es el gestor de paquetes por defecto para Node.js. Se utiliza para instalar y administrar paquetes de Node.js. Cuando instalas un paquete usando `npm install`, ese paquete se descarga y se almacena en tu directorio `node_modules`, y puedes requerirlo en cualquier archivo de tu proyecto.

Por otro lado, **npx** (Node Package Execute) es una herramienta que se utiliza para ejecutar paquetes de Node.js. `npx` viene con npm 5.2+ y superior. La principal diferencia entre `npm` y `npx` es que `npx` ejecuta paquetes sin necesidad de instalarlos previamente.

Por ejemplo, si quisieras usar la herramienta `create-react-app` para crear una nueva aplicación de React, podrías hacerlo con `npx` sin necesidad de instalar `create-react-app` globalmente en tu máquina:

Existe otro comandos para ejecutar paquetes de Node

```bash
npx create-react-app my-app
```

En resumen, `npm` es para instalar y administrar tus dependencias. `npx` es para ejecutar tus paquetes.

## Cómo ejecutar el proyecto de este repositorio

Una vez clonado el repositorio y luego de ejecutar `npm install` instalando las dependencias, para poder activar la aplicación ejecutamos `npm run dev`

La declaración de estos scripts podemos verlo en el `package.json`.

```json
  "scripts": {
    "dev": "vite",
    "build": "tsc && vite build",
    "lint": "eslint . --ext ts,tsx --report-unused-disable-directives --max-warnings 0",
    "preview": "vite preview"
  },
```

Si queremos ver el proyecto de la misma forma que se vería estando en un servidor real, usamos `npm run build` esto creará los archivos de nuestra aplicación en su versión live.
