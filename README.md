# React-Native-SwitchNavigator-Auth-Starter-App
A very lean React Native client with a createNavigatorStack for convenience. Useful for any app that starts with authentication.

*App.js*
``` js
const AppStack = createStackNavigator({ 
  Home: HomeScreen, 
  About: AboutScreen 
});
const AuthStack = createStackNavigator({ 
  SignUp: SignUpScreen, 
  SignIn: SignInScreen 
});

export default createAppContainer(createSwitchNavigator(
  {
    AuthLoading: AuthLoadingScreen,
    App: AppStack,
    Auth: AuthStack,
  },
  {
    initialRouteName: 'AuthLoading',
  }
));
```

Feel free to fork this as a starter repo for your react native project.
