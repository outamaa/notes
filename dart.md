# Dart

## Conditional compilation

Here's an example where we conditionally export
- `web.dart` if we're compiling a web app
- `mobile.dart` if we're compiling a mobile app
- `unsupported.dart` otherwise

``` dart
export 'unsupported.dart'
    if (dart.library.html) 'web.dart'
    if (dart.library.io) 'mobile.dart';
```
