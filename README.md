# react-native-style-block
react-native-component  
Simple and fast  
To use function to describe react native style  

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

### API

- `sb.layout(alignItems = 'flex-start', justifyContent = 'flex-start')`
> {
  **alignItems**,
  **justifyContent**,
}

- `sb.center()`
> {
  alignItems: 'center',
  justifyContent: 'center',
}

- `sb.alignCenter()`
> {
  alignItems: 'center'
}

- `sb.contentCenter()`
> {
  justifyContent: 'center'
}

- `sb.size(width, height)`
> {
  **width**,
  **height**,
}

- `sb.margin(top, right, bottom, left)`
> `sb.margin()` => {
  marginTop: 0,
  marginRight: 0,
  marginBottom: 0,
  marginLeft: 0,
}  
> `sb.margin(top)` => {
  marginTop: **top**,
  marginRight: **top**,
  marginBottom: **top**,
  marginLeft: **top**,
}  
> `sb.margin(top, right)` => {
  marginTop: **top**,
  marginRight: **right**,
  marginBottom: **top**,
  marginLeft: **right**,
}  
> `sb.margin(top, right, bottom)` => {
  marginTop: **top**,
  marginRight: **right**,
  marginBottom: **bottom**,
  marginLeft: **right**,
}  
> `sb.margin(top, right, bottom, left)` => {
  marginTop: **top**,
  marginRight: **right**,
  marginBottom: **bottom**,
  marginLeft: **left**,
}

- `sb.padding(top, right, bottom, left)`
> `sb.padding()` => {
  paddingTop: 0,
  paddingRight: 0,
  paddingBottom: 0,
  paddingLeft: 0,
}  
> `sb.padding(top)` => {
  paddingTop: **top**,
  paddingRight: **top**,
  paddingBottom: **top**,
  paddingLeft: **top**,
}  
> `sb.padding(top, right)` => {
  paddingTop: **top**,
  paddingRight: **right**,
  paddingBottom: **top**,
  paddingLeft: **right**,
}  
> `sb.padding(top, right, bottom)` => {
  paddingTop: **top**,
  paddingRight: **right**,
  paddingBottom: **bottom**,
  paddingLeft: **right**,
}  
> `sb.padding(top, right, bottom, left)` => {
  paddingTop: **top**,
  paddingRight: **right**,
  paddingBottom: **bottom**,
  paddingLeft: **left**,
}

- `sb.radius(value = 0)`
> {
  borderRadius: **value**,
}

- `sb.border(direction = 'all', width = 1, color = 'black', style = 'solid')`
> `sb.border('all', width, color, style)` => {
  borderWidth: **width**,
  borderColor: **color**,
  borderStyle: **style**,
}  
> `sb.border('Top', width, color, style)` => {
  borderTopWidth: **width**,
  borderTopColor: **color**,
  borderTopStyle: **style**,
}  
> `sb.border('Right', width, color, style)` => {
  borderRightWidth: **width**,
  borderRightColor: **color**,
  borderRightStyle: **style**,
}  
> `sb.border('Bottom', width, color, style)` => {
  borderBottomWidth: **width**,
  borderBottomColor: **color**,
  borderBottomStyle: **style**,
}  
> `sb.border('Left', width, color, style)` => {
  borderLeftWidth: **width**,
  borderLeftColor: **color**,
  borderLeftStyle: **style**,
}

- `sb.flex(value = 1)`
> {
  flex: **value**,
}

- `sb.bgColor(color = 'white')`
> {
  backgroundColor: **color**,
}

- `sb.color(color = 'white')`
> {
  **color**,
}

- `sb.alignSelf(alignSelf = 'stretch')`
> {
  **alignSelf**,
}

- `sb.textAlign(textAlign = 'center')`
> {
  **textAlign**,
}

- `sb.font(size = 14, height, weight = 'normal')`
> {
  fontSize: **size**,
  lineHeight: **height** || **size**,
  fontWeight: **weight**,
}

- `sb.position(mode = 'absolute', top, right, bottom, left)`
> {
  position: **mode**,
  top: **top** || "",
  right: **right** || "",
  bottom: **bottom** || "",
  left: **left** || "",
}

- `sb.direction(direction = 'row')`
> {
  flexDirection: **direction**,
}
