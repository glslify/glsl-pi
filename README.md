# glsl-pi

[![locked](http://badges.github.io/stability-badges/dist/locked.svg)](http://github.com/badges/stability-badges)

π available at your convenience for use within glslify.

## Usage

[![NPM](https://nodei.co/npm/glsl-pi.png)](https://nodei.co/npm/glsl-pi/)

### `PI = require('glsl-pi')`

This package exports the value of Pi
[as supplied by google](https://www.google.com/#q=pi): `3.14159265359`. You can use it like so:

``` glsl
#pragma glslify: PI = require('glsl-pi')

uniform float time;

void main() {
  gl_FragColor = vec4(vec3(PI * 2.0 * time), 1);
}
```

This is a *really* simple package but it saves me having to
lookup/copy/paste the value every time. Also a useful
alternative to using `#define PI` that's less leaky :)

## Contributing

See [stackgl/contributing](https://github.com/stackgl/contributing) for details.

## License

MIT. See [LICENSE.md](http://github.com/stackgl/glsl-pi/blob/master/LICENSE.md) for details.
