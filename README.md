<!-- 
This README describes the package. If you publish this package to pub.dev,
this README's contents appear on the landing page for your package.

For information about how to write a good package README, see the guide for
[writing package pages](https://dart.dev/guides/libraries/writing-package-pages). 

For general information about developing packages, see the Dart guide for
[creating packages](https://dart.dev/guides/libraries/create-library-packages)
and the Flutter guide for
[developing packages and plugins](https://flutter.dev/developing-packages). 
-->

This is a widget that displays a list of items.
Same widget that behaves like a row and like a column.

## Features

We currently have the following features:

- [RowColumn] is a widget that displays multiple items, either horizontally or vertically, manually after specifying the Axis direction.
- [FlexibleRowColumn] is a widget that displays multiple items, either horizontally or vertically automatically after detecting orientation.

## Getting started

Import the package:

```
import 'package:row_column/row_column.dart';
```

To start using this package, add the following to your `pubspec.yaml` file:

```
depensencies:
    row_column: ^0.0.1
```

## Usage

To user it just add the widget to the widget tree :

- This `RowColumn` can switch between column and row by specifying the `direction` property.:

```
RowColumn(
          mainAxisAlignment: MainAxisAlignment.spaceAround,
          direction: Axis.horizontal,
          children: [
            const Text('Hello'),
            const Text('My'),
            const Text('Lovely'),
            const Text('World'),
          ],
        ),
```


- This `FlexibleRowColumn` can detect the orientation of the device and switch betwin column and row automatically:

```
FlexibleRowColumn(
          mainAxisAlignment: MainAxisAlignment.spaceAround,
          children: [
            const Text('Hello'),
            const Text('My'),
            const Text('Lovely'),
            const Text('World'),
          ],
        ),
```

## Additional information

Tell users more about the package: where to find more information, how to
contribute to the package, how to file issues, what response they can expect
from the package authors, and more.
