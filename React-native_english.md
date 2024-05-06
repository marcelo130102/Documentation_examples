# Basic React Native Tutorial

In this tutorial, we'll learn the basics of React Native, a popular tool for building cross-platform mobile applications using JavaScript and React.

![React Native in 100 seconds](https://www.youtube.com/watch?v=gvkqT_Uoahw)

## What is React Native?

React Native is a mobile development framework created by Facebook that allows building native mobile applications using JavaScript and React. This means you can write your code once and run it on both iOS and Android, saving time and effort in mobile app development.

## Prerequisites

- Basic knowledge of JavaScript.
- Node.js installed on your system.
- A code editor (recommended: Visual Studio Code).

## Step 1: Setting up the environment

To get started, you need to install React Native CLI (Command Line Interface) globally on your system. You can do this by running the following command in your terminal:

```bash
npm install -g react-native-cli
```

## Step 2: Create a new project

After installing React Native CLI, you can create a new project by running the following command:

```bash
react-native init MyProject
```

This will create a new folder named `MyProject` with the structure of a React Native project.

## Step 3: Running the application

Once the project is created, navigate to the project folder and start the application by running the following commands:

```bash
cd MyProject
react-native run-android
```

or

```bash
cd MyProject
react-native run-ios
```

These commands will start the application on an emulator or connected device.

## Step 4: Edit the application

Open the project in your code editor and edit the `App.js` file. This is the entry point of your application. You can start by modifying the text or adding new components.

```javascript
import React from 'react';
import { View, Text } from 'react-native';

const App = () => {
  return (
    <View style={{ flex: 1, justifyContent: 'center', alignItems: 'center' }}>
      <Text>Hello, world!</Text>
    </View>
  );
}

export default App;
```

## Step 5: Experiment

Now you can experiment! Add new components, styles, functionalities, and explore the possibilities of React Native.

## Conclusion

In this tutorial, we've covered the basics to start developing mobile applications with React Native. From here, you can delve deeper into the official documentation and explore different aspects of this framework to build awesome mobile applications.
