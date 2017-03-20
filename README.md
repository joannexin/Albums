# Albums

This is my first react native app.

![Albums screenshot]()

## This is what I learnt

1. Generate the project using react native CLI, run “react-native init XXX(project name)” in command line
2. This produce a new react native project capable of running in either the android or iOS simulator. After generating the project, we started to use the simulator either “react-native run-ios” or “react-native run-android”
3. Create eslint for keep tracking syntax error. First, run “npm install --save-dev eslint-config-rallycoding” on command line to install what kind of syntax you would like to follow within this particular project; second, create “.eslintrc” file at root directory and echo “{"extends”: “rallycoding"}” in the file.
4. Don’t forget to import React from ‘react’, as well as import { AppRegistry } from ‘react-native’ in index.ios.js to kick off the project, also, this is the only time we call AppRegistry in this entire project.
5. When we create components, I am aware that there are two different type of components (class component and functional component). Here is the differences I learnt: Functional component are presentational components that just produce some amount of JSX and show data back to the user, whereas class component can access to component level state and life cycle methods.
6. Also, there are two important feature of react native: state and props. It’s very similar to React, and here is the main differences: state is the feature is only available to class components, state is use to record and react to user interactions. We only update our state object with “this.setState({});” whereas props is any type of data we pass from a parent to a child component. In another word, whenever we want to communicate from parent component to child component, we use props; state is component internal record keeping, we use state whenever we want to change some data overtime
7. react native doesn’t support bootstrap library for CSS, so one big challenge of react native is dealing with styling components. we declare const styles = { headerContainer: {} }; at the bottom and then apply the style within the open tag style={styles.headerContainer}
8. UI/UX is very important for react native, for example, whenever a user press a button on a touch screen, we need to show some interaction back to the user so that to tell the app is not freezing by using TouchableHighlight to TouchableOpacity, etc
9. Reusable component code is very important for future use. Therefore, break large components into pieces of micro-components are very handy.
