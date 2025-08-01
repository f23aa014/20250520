## 6/04
複雑な構造のウィジェット

AppBarについて
AppBarの基本形
```dart
AppBar(
    title:ウィジェット,
    leading:ウィジェット,
    actions:<Widget>[ウィジェットのリスト],
    bottom:《PreferredSize》,
)
```
title タイトル表示部分。通常はTextを用意
leading　左は時に表示される。通常はボタン化アイコンなどのリストを用意
actions　titleの右側に表示される。ボタン・アイコンなどのリストを用意
bottom　上記の下に追加表示される部分。PreferredSizeインスタンスを用意

AppBarをカスタマイズする

BackButtonについて

actionsのアイコンについて

bottomの表示

- BottomNavigationBarについて
    画面の下部に表示できるbar
BottomNavigationBarの利用例
    
BottomNavigationBarの仕組み
    
アイコンのカラーとサイズ

ListViewについて

ListViewの利用例

