# Chat App

Chatting application from raect native using firebase realtime databse, reactwebview(Rails)


## Getting Started


### Install

```
$ npm install
```

- **React Native 0.60+**


[Link](url) sample text with link. 


```bash
code bash
```


*Note* For `iOS` using `cocoapods`, run:

```bash
$ cd ios/ && pod install
```

See docs for [manual linking guide](docs/Linking.md)

### **Upgrading to React Native *0.60+*** 
 
New React Native comes with `autolinking` feature, which automatically links Native Modules in your project.
In order to get it to work, make sure you `unlink` `Async Storage` first:

```bash
$ react-native unlink @react-native-community/async-storage
```


## Usage

### Import

```js
import AsyncStorage from '@react-native-community/async-storage';
```

### Store data
```jsx

storeData = async () => {
  try {
    await AsyncStorage.setItem('@storage_Key', 'stored value')
  } catch (e) {
    // saving error
  }
}

```

### Read data
```jsx

getData = async () => {
  try {
    const value = await AsyncStorage.getItem('@storage_Key')
    if(value !== null) {
      // value previously stored
    }
  } catch(e) {
    // error reading value
  }
}

```
### Advanced
See docs for [api and more examples](docs/API.md) or [advanced usages](docs/advanced).

## Writing tests

Using [Jest](https://jestjs.io/) for testing? Make sure to check out [docs on how to integrate it with this module.](./docs/Jest-integration.md)

## Contribution

See the [CONTRIBUTING](CONTRIBUTING.md) file for how to help out.

## License

MIT
