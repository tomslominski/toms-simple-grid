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

See [_index.scss](_index.scss) for a full list of variables you can modify.
