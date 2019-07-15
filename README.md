<img alt="React Native Review Modal" src="https://github.com/WrathChaos/react-native-review-modal/blob/master/assets/logo.png" width="1050"/>

Review Modal with dynamic rate system and comment feature for React Native

[![npm version](https://img.shields.io/npm/v/react-native-review-modal.svg)](https://www.npmjs.com/package/react-native-review-modal)
[![npm](https://img.shields.io/npm/dt/react-native-review-modal.svg)](https://www.npmjs.com/package/react-native-review-modal)
![Platform - Android and iOS](https://img.shields.io/badge/platform-Android%20%7C%20iOS-blue.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

<p align="center">
<img alt="React Native Review Modal" src="https://github.com/WrathChaos/react-native-review-modal/blob/master/assets/Screenshots/React-Native-Review-Modal.gif.gif" width="49.7%" />
</p>

<p align="center">
<img alt="React Native Review Modal" src="https://github.com/WrathChaos/react-native-gradient-header/blob/master/assets/Screenshots/example.png" width="49.7%" />
<img alt="React Native Review Modal" src="https://github.com/WrathChaos/react-native-gradient-header/blob/master/assets/Screenshots/example1.png" width="49.7%" />
</p>

## Installation

Add the dependency:

### React Native:

```js
npm i react-native-review-modal
```

## Peer Dependencies

###### IMPORTANT! You need install them.

```js
"react": ">= 16.x.x",
"react-native": ">= 0.55.x",
"react-native-modal": ">= 11.1.0",
"react-native-star-rating": ">= 1.1.0",
"react-native-vector-icons": ">= 6.6.0",
"react-native-linear-gradient": ">= 2.5.4",
"@freakycoder/react-native-text-area": ">= 0.0.11"
```

## Basic Usage

```js
import ReviewModal from "react-native-review-modal";

constructor(props) {
  super(props);
  this.state = {
    starCount: 3.6
  };
}

onStarRatingPress(rating) {
  this.setState({
    starCount: rating
  });
}

render() {
  return (
    <ReviewModal
      starRating={this.state.starCount}
      onStarRatingPress={rating => {
        this.onStarRatingPress(rating);
      }}
    />
  );
}
```

## Configuration - Props
 
| Property         |  Type   |       Default        | Description                                                                                |
| ---------------- | :-----: | :------------------: | ------------------------------------------------------------------------------------------ |
| backgroundColor  |  color  | "rgba(0, 0, 0, 0.5)" | change the backdrop's color                                                                |
| type             | string  |  "FadingCircleAlt"   | change the type of spinner's icon                                                          |
| size             | number  |          50          | change the spinner's size                                                                  |
| color            |  color  |        white         | change the spinner's color                                                                 |
| spinnerStyle     |  style  |       default        | set your own style for spinner                                                             |
| spinnerIsVisible | boolean |         true         | change the visibility of spinner                                                           |
| textColor        |  color  |        white         | change the dynamic text's color                                                            |
| textStyle        |  style  |       default        | set your own style for text                                                                |
| numberOfLines    | number  |          2           | RECOMMENDED! Do NOT change the number of lines, users cannot read long texts below 1.5 sec |


## Author

FreakyCoder, kurayogun@gmail.com

## License

React Native Review Modal Library is available under the MIT license. See the LICENSE file for more info.
