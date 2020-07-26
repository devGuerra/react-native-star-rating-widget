# react-native-star-widget

## Installation
1. install react-native-star-widget
`npm install react-native-star-widget --save`
or
`yarn add react-native-star-widget`
2. if not already installed, add [react-native-svg](https://github.com/react-native-community/react-native-svg)

## Usage
```js
const Example = () => {
  const [rating, setRating] = useState(0);
  return (
      <StarRating
        rating={rating}
        onChange={setRating}
      />
  );
};
```

## Props
| Name       | Type                 | Default         | Description                                      |
| ---------- | -------------------- | --------------- | ------------------------------------------------ |
| rating     | number               | **REQUIRED**    | Rating Value. Should be between 0 and `maxStars` |
| onChange   | (number) => void     | **REQUIRED**    | called when rating changes                       |
| maxStars   | number               | 5               | number of stars                                  |
| minRating  | number               | 0.5             | minimum selectable rating                        |
| starSize   | number               | 32              | star size                                        |
| color      | string               | "#fdd835"       | star color                                       |
| emptyColor | string               | same as `color` | empty star color                                 |
| style      | StyleProp<ViewStyle> | undefined       | optional style                                   |