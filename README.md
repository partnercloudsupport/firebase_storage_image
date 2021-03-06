# firebase_storage_image

[![pub package](https://img.shields.io/pub/v/firebase_storage_image.svg)](https://pub.dartlang.org/packages/firebase_storage_image)

Flutter's [ImageProvider](https://docs.flutter.io/flutter/painting/ImageProvider-class.html) for images in [Firebase Cloud Storage](https://firebase.google.com/docs/storage/).

## Getting Started

`FirebaseStorageImage` implements [ImageProvider](https://docs.flutter.io/flutter/painting/ImageProvider-class.html). So you can use this directly for [Image](https://docs.flutter.io/flutter/widgets/Image-class.html), [CircleAvatar](https://docs.flutter.io/flutter/material/CircleAvatar-class.html), [ImageIcon](https://docs.flutter.io/flutter/widgets/ImageIcon-class.html), and something like that.

### Example

```dart
import 'package:flutter/material.dart';
import 'package:firebase_storage_image/firebase_storage_image.dart';

class YourCircleAvatar extends StatelessWidget {
  @override
  Widget build(BuildContext context) => const CircleAvatar(
        backgroundImage: FirebaseStorageImage(
          'gs://project-12345.appspot.com/path/to/avatar_image.png',
        ),
      );
}
```

## License

[MIT](LICENSE)

## Contribution

I need your help improving this package with leaving Pull Requests and Issues!
