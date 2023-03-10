# react-native-animated-floating-button

animated button

![animated button example](https://github.com/developertrt/React-native-animate-floating-button/blob/main/images/demo.gif)

## Installation

```sh
npm install react-native-animated-floating-button
```

## Usage


```js
import { AnimatedFloatingButton } from 'react-native-animated-floating-button'

// ...

let images = [
    { image: require('./assets/images/Pin.png') },
    { image: require('./assets/images/Love.png') }
  ]

<AnimatedFloatingButton
    onMenuClick={(res) => {
     console.log(res)
    }}
    onIconClick={(res) => {
     console.log(res)
    }}
    menuImage={require('./assets/images/Plus.png')}
    iconColors={'lightpink'}
    style={{ backgroundColor: 'lightpink' }}
    images={images}
/>
```

### Properties
| Name                 | Description                                                                                                                                                                                                                                                                                          | Type                                                   |                   Default Value                   |
|----------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|:-------------------------------------------------:|
| `images`                | array of images, how many button of images open when onMenuClick                                                                                                                                                                                                                                                                               | array                                                 |                  _**required**_                   |   
| `menuImage`                | main image icon                                                                                                                                                                                                                                                                               | image                                                 |                  _**required**_                   |
| `onMenuClick`                | retrun menu is open or not                                                                                                                                                                                                                                                                                | `()=>Node`                                                |                  _**required**_                   |
| `onIconClick`                | retrun icon index when you click on item                                                                                                                                                                                                                                                                                | `()=>Node`                                                |                  _**required**_                   |
