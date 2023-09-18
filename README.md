# Mirage UI Colors

The ultimate color system for developers and designers.

## Installation

yarn

```bash
yarn add @mirage-ui/colors
```

npm

```bash
npm install @mirage-ui/colors
```

## Usage

Tailwind CSS

```js
// tailwind.config.js
const { warning, functional, success } = require("@mirage-ui/colors");

module.exports = {
  theme: {
    colors: {
      ...warning,
      ...functional,
      ...success,
    },
  },
};
```

Vanilla CSS

```css
@import "@mirage-ui/colors/warning";
@import "@mirage-ui/colors/functional";
@import "@mirage-ui/colors/success";

--warning: var(--warning-200);
--black: var(--functional-black);
--success: var(--success-200);

.warning {
  color: var(--warning);
}

.functional {
  color: var(--black);
}

.success {
  color: var(--success);
}
```

Stitches

```js
import { createCss } from "@stitches/react";
import { warning, functional, success } from "@mirage-ui/colors";

const { styled } = createCss({
  theme: {
    colors: {
      ...warning,
      ...functional,
      ...success,
    },
  },
});

const Warning = styled("div", {
  color: "$warning500",
});
```

React

```js
import { primary, success, functional } from '@mirage-ui/colors'

export fuction SomePage(){
    return(
        <div>
            <h1 style={{color: primary}}>Primary</h1>
            <h1 style={{color: success}}>Success</h1>
            <h1 style={{color: functional}}>Functional</h1>
        </div>
    )
}

```
