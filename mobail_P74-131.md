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
fontSize:フォントサイズ。double値で指定  
fontWeight:フォントの太さ。FontWeightというクラスのw100～w900、あるいはboldという定数で指定  
fontFamily:フォントファミリー。テキスト（String）で指定  
fontStyle:フォントスタイル。FontStyale列挙型のnormal、italicという値で指定  
color:テキスト色。Colorクラスで指定

```dart
style: TextStyle(fontSize:32.0,
color: const Color(0xff000000),
fontWeight: FontWeight.w700,
fontFamily: "Roboto"),
```

## Colorについて
```dart
color: const Color(0x000000),
```
※引数を6または8桁の１６進数で指定する  
  → RGBまたはARGBの値を指定している  

ARGBの値を個別に因数で指定してインスタンスを作成するメソッド
```dart
Color.fromARGB(アルファ,赤,緑,青)
```

## テーマを指定する
Dark Theme:ダークテーマをON/OFFするもの。通常表示はOFFに、暗い背景をベースにした表示にしたければONにしておく  
Primary Swatch:テーマの基本的な色を指定します  
Primary Color:標準のテキストなどの色  
Accent Color:アクセントの色  
Devider Color:仕切り線の色  
Canvas Color:キャンバス（グラフィック描画の部分）の色  
Background Color:背景色として報じを作る際に使われる色  
FontFamily:使用するフォントファミリーの指定  


- テーマ指定
MaterialAppインスタンスを作成する際、themeにThemeDataが設定さえれるようになります。





