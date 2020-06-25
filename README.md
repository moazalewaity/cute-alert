# Cute Alert

![img](https://i.imgur.com/16FXjDo.png)

I designed this JS library as an open-source project with the purpose of providing beautiful alert box messages for your website. Feel free to contribute with a pull request or suggestions. (This a second version that keeps the alert close button as a circle)

## Instructions

- Firstly clone this repo and import both "style.css" and "cute-alert.js" into your code.
- In your JS file, call cuteAlert() passing the following arguments: type, title, message and buttonText in object notation. (the last one is optional)

Examples:

```sh
cuteAlert({
  type: "success",
  title: "Congratulations!",
  message: "You won the match!",
  buttonText: "Yaay!!!"
});
```

```sh
cuteAlert({
  type: "error",
  title: "Sorry...",
  message: "You lost the match!",
  buttonText: "OK :-("
});
```

```sh
cuteAlert({
    type: "warning",
    title: "Be careful...",
    message: "That's dangerous!",
    buttonText: "OMG!",
  });
```

```sh
cuteAlert({
    type: "info",
    title: "Quick tip!",
    message: "Avoid this path...",
    buttonText: "OK!",
  });
```

cuteAlert() returns a Promise, so you can use "then" to execute an action after the modal window is closed:

```sh
cuteAlert({
  type: "error",
  title: "Sorry...",
  message: "You lost the match!",
  buttonText: "OK :-("
}).then(() => {
  location.reload();
});
```


## Design

- **Igor Ferrão de Souza** https://www.linkedin.com/in/igor-ferr%C3%A3o-de-souza-4122407b/


## Dev

- **Gustavo Mancuzo** - [gustavosmanc](https://github.com/gustavosmanc)


## Contributors

- **Leonardo Bertoncin** - [lbert1](https://github.com/lbert1)
