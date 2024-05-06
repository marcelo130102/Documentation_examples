# Tutorial Básico de React Native

En este tutorial, aprenderemos los conceptos básicos de React Native, una herramienta popular para construir aplicaciones móviles multiplataforma usando JavaScript y React.

![React Native in 100 seconds](https://www.youtube.com/watch?v=gvkqT_Uoahw)

## ¿Qué es React Native?

React Native es un framework de desarrollo móvil creado por Facebook que permite construir aplicaciones móviles nativas utilizando JavaScript y React. Esto significa que puedes escribir una vez tu código y ejecutarlo en iOS y Android, lo que ahorra tiempo y esfuerzo en el desarrollo de aplicaciones móviles.

## Requisitos previos

- Conocimientos básicos de JavaScript.
- Node.js instalado en tu sistema.
- Un editor de código (recomendado: Visual Studio Code).

## Paso 1: Configuración del entorno

Para comenzar, necesitas instalar React Native CLI (Command Line Interface) globalmente en tu sistema. Puedes hacerlo ejecutando el siguiente comando en tu terminal:

```bash
npm install -g react-native-cli
```

## Paso 2: Crear un nuevo proyecto

Después de instalar React Native CLI, puedes crear un nuevo proyecto ejecutando el siguiente comando:

```bash
react-native init MiProyecto
```

Esto creará una nueva carpeta llamada `MiProyecto` con la estructura de un proyecto de React Native.

## Paso 3: Ejecutar la aplicación

Una vez que se ha creado el proyecto, accede a la carpeta del proyecto e inicia la aplicación ejecutando los siguientes comandos:

```bash
cd MiProyecto
react-native run-android
```

o

```bash
cd MiProyecto
react-native run-ios
```

Estos comandos iniciarán la aplicación en un emulador o dispositivo conectado.

## Paso 4: Editar la aplicación

Abre el proyecto en tu editor de código y edita el archivo `App.js`. Este es el punto de entrada de tu aplicación. Puedes comenzar modificando el texto o agregando nuevos componentes.

```javascript
import React from 'react';
import { View, Text } from 'react-native';

const App = () => {
  return (
    <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
      <Text>Hola, mundo!</Text>
    </View>
  );
}

export default App;
```

## Paso 5: Experimenta

¡Ahora puedes experimentar! Agrega nuevos componentes, estilos, funcionalidades y explora las posibilidades de React Native.

## Conclusión

En este tutorial, hemos cubierto los conceptos básicos para empezar a desarrollar aplicaciones móviles con React Native. A partir de aquí, puedes profundizar más en la documentación oficial y explorar diferentes aspectos de este framework para construir aplicaciones móviles impresionantes.
