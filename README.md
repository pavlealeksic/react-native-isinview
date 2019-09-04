# react-native-isinview
Detects if a ScrollView or ListView element is inside the users viewport and reports back on changes

##Install

```js
npm i -S react-native-isinview
```
or with yarnpkg:
```js
yarn add react-native-isinview --save
```

##Props
- `onChange` **(required)**: callback function that report true or false if component is in view.
- `active` : if set true it will activate a listener to the view (default: true).
- `delay` : set the frequency for the listener (default: 200).

##Uage
```js
import IsInview from 'react-native-isinview'

render() {
  return (
  <ScrollView>
    <IsInview onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </IsInview>

    <IsInview onChange={inView => console.log('Inview: '+ inView)}>
      ....
    </IsInview>

  </ScrollView>
  );
}
```
