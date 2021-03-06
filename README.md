# Tom's Simple Grid

Sass library for generating a basic flexbox based grid. Requires Dart Sass.

Include in your project with `@use 'node_modules/toms-simple-grid'`, or using `with` to configure it:

```
@use 'node_modules/toms-simple-grid' with (
	$grid-sizes: (
		"*": (1, 12),
		"sm": (1, 6, 12),
		"md": (1, 6, 12),
	),
	$grid-width: 800px
);
```

When building your project, include `node_modules` in your load path, for example using Dart Sass:

```
sass input.scss output.scss -I node_modules
```

See [_index.scss](_index.scss) for a full list of variables you can modify.

## Development

When installing this package locally for development, the dependencies will not link to the correct folder. To get around this, you have to add the dependencies to the load path manually.

```
sass input.scss output.css -I node_modules/toms-simple-grid/node_modules
```
