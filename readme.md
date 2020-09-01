# Slash [/] snippets

This extension provides my own most used snippets.
It contains snippets for React, Redux, React Native and ofcourse HTML boilerplate.

## StyleSheet

|  Prefix | Method                |
| ------: | --------------------- |
| `sty->` | `style={styles.${1}}` |

## React Native Components

### `rnsc`

```javascript
import React from 'react';
import { View, Text, StyleSheet } from 'react-native';

const $1 = () => {
  return (
    <View>
      <Text>$0</Text>
    </View>
  );
};

const styles = StyleSheet.create({});

export default $1;
```

## React Components

### `rsc`

```javascript
import React from 'react';

const $1 = () => {
  return (
    <div>
      <h2>$0</h2>
    </div>
  );
};

export default $1;
```
