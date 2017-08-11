# react-native-style-block
react-native-component
simple and fast
use function to describe react native style

## Usage

### example
```javascript
<View style={styles.view}>
  <Image
    style={styles.image}
    source={require('./img/test.png')}
  />
  <Text style={styles.username}>username</Text>
  <Text style={styles.description}>description</Text>
</View>
```

```javascript
const sb = require('react-native-style-block');

const styles = {
  view: [
    sb.size('100%', 'auto'),
    { alignItems: 'center' },
    sb.padding(20, 0),
    sb.bgColor('#ffffff'),
    sb.border('Bottom', 1, '#eeeeee'),
    sb.margin(0,0,10,0)
  ],
  image: [
    sb.radius(30),
    sb.size(60, 60)
  ],
  username: [
    sb.margin(6,0,0,0),
    sb.font(20)
  ],
  description: [
    sb.font(14),
    sb.color('#999999')
  ]
}
```
