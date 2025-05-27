# 5/27:教科書P74～95
参照URL: https://flutterstudio.app(Flutter Sutudio)  
>Flutter Studioとは？  
 
 ※注意点  
 ``` 
 誤：MyHomePage({Key key}) : super(key: key);  
 正：MyHomePage({Key? key}) : super(key: key);
```
***
### 基本code
```dart
import 'package:flutter/material.dart';

void main() {
  runApp(new MyApp());
}
class MyApp extends StatelessWidget {

  @override
  Widget build(BuildContext context) {
    return new MaterialApp(
      title: 'Generated App',
      theme: new ThemeData(
        primarySwatch: Colors.blue,
        primaryColor: const Color(0xFF2196f3),
        accentColor: const Color(0xFF2196f3),
        canvasColor: const Color(0xFFfafafa),
      ),
      home: new MyHomePage(),
    );
  }
}

class MyHomePage extends StatefulWidget {
  MyHomePage({Key key}) : super(key: key);
  @override
  _MyHomePageState createState() => new _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
    @override
    Widget build(BuildContext context) {
      return new Scaffold(
        appBar: new AppBar(
          title: new Text('App Name'),
          ),
        body:
          new Text(
          "Hello Flutter!",
            style: new TextStyle(fontSize:32.0,
            color: const Color(0xFF000000),
            fontWeight: FontWeight.w700,
            fontFamily: "Roboto"),
          ),
    
      );
    }
}
```
***
## テキストスタイルについて
fontSize
fontWeight
fontFamily
fontStyle
color

## Colorについて
