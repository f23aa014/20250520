## 5/20：まとめtest

RANをクリックすると実行される


```dart
import 'package:flutter/material.dart';

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {

 
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Flutter Demo',
      
      home: Text(
        'Hello Flutter World!!',
        style:TextStyle(fontSize: 32.0)
        ),
    );
  }
}
```
上記のコードを実行すると赤文字の`Hello Flutter World!!`が表示  
※背景は黒くなりませんでした。(chromeで実行)


## アプリ画面とウィジェットツリー
Flutterでは、画面表示は`ウィジェット`と呼ばれる部品によって作成される
## アプリ実行の仕組み

## StatelessWidgetクラスについて
## MaterialAppクラスについて
## マテリアルデザインについて


