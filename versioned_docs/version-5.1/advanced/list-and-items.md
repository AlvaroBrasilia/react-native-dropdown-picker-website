---
id: list-and-items
title: List and Items
---

## Disable an Item
You may want to disable an item, The item will be unselectable.

```js
{label: 'Item', value: 1, disabled: true}
```

## Props
### `itemKey`
Specifies which item key should be used as a key.

```jsx
itemKey="value"
```
| Type     | Default  |
| -------- | -------- |
| string   | `value`  |

### `closeAfterSelecting`
Closes the drop-down menu after selecting an item.  

```jsx
closeAfterSelecting={true}
```
:::note
This only works with **single** item pickers.
:::
| Type     | Default  |
| -------- | -------- |
| bool     | false    |

### `itemSeparator`
Specifies if the item separater should be visible.

```jsx
itemSeparator={true}
```
| Type     | Default  |
| -------- | -------- |
| bool     | false    |

### `renderListItem`
Customizes the `renderListItem`.

```jsx
renderListItem={(props) => <Item {...props} />}
```
+ **See: [RenderListItem.js](https://github.com/hossein-zare/react-native-dropdown-picker/blob/5.x/src/components/RenderListItem.js)**

| Type     |
| -------- |
| function |

### `ListEmptyComponent`
Changes the default `ListEmptyComponent`.

```jsx
ListEmptyComponent={({
  listMessageContainerStyle, listMessageTextStyle, ActivityIndicatorComponent, loading, message
}) => (
  <View style={listMessageContainerStyle}>
    {loading ? (
      <ActivityIndicatorComponent />
    ) : (
      <Text style={listMessageTextStyle}>
        {message}
      </Text>
    )}
  </View>
)}}
```

## Styling
### `listItemContainerStyle`
```jsx
listItemContainer={{
  height: 40
}}
```

### `listItemLabelStyle`
```jsx
color="#000"
```

### `selectedItemContainerStyle`
```jsx
selectedItemContainerStyle={{
  backgroundColor: "grey"
}}
```

### `selectedItemLabelStyle`
```jsx
selectedItemLabelStyle={{
  fontWeight: "bold"
}}
```

## `customItemContainerStyle`
```jsx
customItemContainerStyle={{
  //
}}
```

## `customItemLabelStyle`
```jsx
customItemLabelStyle={{
  fontStyle: "italic"
}}
```

### `disabledItemContainerStyle`
```jsx
disabledItemContainerStyle={{
  //
}}
```

### `disabledItemLabelStyle`
```jsx
disabledItemLabelStyle={{
  opacity: 0.5
}}
```

### `listMessageContainerStyle`
```jsx
listMessageContainerStyle={{
  //
}}
```

### `listMessageTextStyle`
```jsx
listMessageTextStyle={{
  //
}}
```

### `itemSeparatorStyle`
```jsx
itemSeparatorStyle={{
  backgroundColor: "#000"
}}
```