# introjs.dart v1.0.0
A dart wrapper for [intro.js](https://github.com/usablica/intro.js) `v2.3.0`.

Check the original repo's README for more info.

## `pubspec.yaml`
```yaml
...
dependencies:
    inrojs: ^1.0.0
...
```

## How to use
This Dart package includes the original intro.js in it so you can include it from your packages once you've run `pub get`:

```html
<link href="packages/introjs/introjs.css" rel="stylesheet">
<script type="text/javascript" src="packages/introjs/intro.js"></script>

<script type="application/dart" src="myapp.dart"></script>
```

The minified js scripts are under the `minified` directory:

```html
<link href="packages/introjs/minified/introjs.min.css" rel="stylesheet">
<script type="text/javascript" src="packages/introjs/minified/intro.min.js"></script>

<script type="application/dart" src="myapp.dart"></script>
```

Add all the `data-intro`s and `data-step`s to your HTML elements (see original README and [documentation](https://github.com/usablica/intro.js/wiki/Documentation) for more details) and then in `myapp.dart`:

```dart
import "package:introjs/introjs.dart";

void main() {
  new IntroJs().start();
}
```

## Examples
Examples for using the Dart wrapper can be found in the `example` directory.
