react-focuspoint
=================

A React component for 'responsive cropping' with [jQuery FocusPoint](https://github.com/jonom/jquery-focuspoint).

```
npm install --save react-focuspoint
```

## Usage

```jsx

var React = require('react');
var Focuspoint = require('react-focuspoint');

var MyComponent = React.createClass({

  render() {
    return (
      <Focuspoint
        src="/img/some-image.jpg"
        imageW={800}
        imageH={450}
        focusX={0.75}
        focusY={0.75}
      />
    );
  }

});

```

Most of these props correspond to [FocusPoint](https://github.com/jonom/jquery-focuspoint) options.

Props that correspond to data FocusPoint data attributes:

- `focusX` (required)
- `focusY` (required)
- `imageW`
- `imageH`

Props that are passed to FocusPoint constructor:

- `reCalcOnWindowResize`
- `throttleDuration`

Other props:

- `src` - Image src

## License
MIT
