# Slash [/] snippets

This extension provides my own most used snippets.
It contains snippets for React, Redux, React Native and ofcourse HTML boilerplate.

## StyleSheet

| Prefix    | Method                     |
| --------- | -------------------------- |
| `sty->`   | `style={styles.${1}}`      |
| `muicl->` | `className={classes.${1}}` |

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

### `rnc`

```javascript
import React from 'react';
import { View, Text } from 'react-native';

const $1 = () => {
  return (
    <View>
      <Text>$0</Text>
    </View>
  );
};

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

## Material-UI React

### `muirsc`

```javascript
import React from 'react';
import { makeStyles } from '@material-ui/core/styles';
import { Typography, Box } from '@material-ui/core';

const useStyles = makeStyles({});

const $1 = ({ className = '' }) => {
  const classes = useStyles();
  const rootClass = `${classes.root} ${className}`;

  return (
    <Box className={rootClass}>
      <Typography>$0</Typography>
    </Box>
  );
};

export default $1;
```

### `muirscpropt`

```javascript
import React from 'react';
import PropTypes from 'prop-types';
import { makeStyles } from '@material-ui/core/styles';
import { Typography, Box } from '@material-ui/core';

const useStyles = makeStyles({});

const $1 = ({ className = '' }) => {
  const classes = useStyles();
  const rootClass = `${classes.root} ${className}`;

  return (
    <Box className={rootClass}>
      <Typography>$0</Typography>
    </Box>
  );
};

$1.propTypes = {
  className: PropTypes.string,
};
export default $1;
```

### `muirscpropt-is`

```javascript
import React from 'react';
import PropTypes from 'prop-types';
import { Typography, Box } from '@material-ui/core';

import { useStyles } from './styles.js';

const $1 = ({ className = '' }) => {
  const classes = useStyles();
  const rootClass = `${classes.root} ${className}`;

  return (
    <Box className={rootClass}>
      <Typography>$0</Typography>
    </Box>
  );
};

$1.propTypes = {
  className: PropTypes.string,
};
export default $1;
```

### `muirscpropt-container`

```javascript
import React from 'react';
import PropTypes from 'prop-types';

import $1View from './$1View';

const $1 = ({ className = '' }) => {
  return <$1View className={className} />;
};

$1.propTypes = {
  className: PropTypes.string,
};
export default $1;
```

### `muirscpropt-presentation`

```javascript
import React from 'react';
import PropTypes from 'prop-types';
import { Typography, Box } from '@material-ui/core';

import { useStyles } from './styles';

const $1View = ({ className = '' }) => {
  const classes = useStyles();
  const rootClass = `${classes.root} ${className}`;

  return (
    <Box className={rootClass}>
      <Typography>$0</Typography>
    </Box>
  );
};

$1View.propTypes = {
  className: PropTypes.string,
};
export default $1View;
```

### `muistylehook`

```javascript
import { makeStyles } from '@material-ui/core/styles';

export const useStyles = makeStyles({
  root: {},
});
```

## console.log

### `clo`

```javascript
console.log('[MY] $1 >>>', $1);
```

### `gotcha`

```javascript
console.log('gotcha!$1');
```
