# Flutter의 위젯 기반 UI

Flutter의 핵심 철학은 "모든 것이 위젯"이라는 개념입니다. 위젯 기반 UI에 대해 자세히 살펴보겠습니다.

## 위젯이란?

위젯(Widget)은 Flutter UI를 구성하는 기본 요소입니다. 버튼, 텍스트, 이미지와 같은 단순한 UI 요소부터 복잡한 레이아웃, 상태 관리, 애니메이션까지 모든 것이 위젯으로 구현됩니다.

## 위젯의 종류

Flutter의 위젯은 크게 두 가지 유형으로 나뉩니다:

1. **Stateless Widget (상태가 없는 위젯)**
   - 한 번 생성되면 변경되지 않는 정적인 위젯
   - 입력(매개변수)이 변경되지 않는 한 다시 그려지지 않음
   - 예: Text, Icon, RaisedButton 등

2. **Stateful Widget (상태가 있는 위젯)**
   - 시간에 따라 상태가 변할 수 있는 동적인 위젯
   - 사용자 입력이나 데이터 변경에 따라 UI가 업데이트됨
   - 예: Checkbox, TextField, ProgressIndicator 등

## 위젯 트리

Flutter 앱은 중첩된 위젯들의 트리 구조로 구성됩니다:

```
MyApp
 └── MaterialApp
     └── Scaffold
         ├── AppBar
         │   └── Text
         └── Center
             └── Column
                 ├── Text
                 ├── SizedBox
                 └── ElevatedButton
```

## 주요 위젯 카테고리

1. **레이아웃 위젯**
   - Row, Column: 수평/수직 방향으로 자식 위젯 배치
   - Container: 패딩, 마진, 배경색 등을 설정할 수 있는 박스
   - Stack: 위젯들을 겹쳐서 배치

2. **기본 UI 요소**
   - Text: 텍스트 표시
   - Image: 이미지 표시
   - Icon: 아이콘 표시
   - Button 종류: ElevatedButton, TextButton, IconButton 등

3. **입력 위젯**
   - TextField: 텍스트 입력
   - Checkbox, Switch, Slider: 값 선택 위젯

4. **테마 위젯**
   - Material 디자인: MaterialApp, Scaffold, AppBar 등
   - Cupertino 디자인: CupertinoApp, CupertinoPageScaffold 등

## 위젯 구현 예시

### Stateless Widget 예시:

```dart
class WelcomeWidget extends StatelessWidget {
  final String name;
  
  // 생성자
  const WelcomeWidget({required this.name, Key? key}) : super(key: key);
  
  @override
  Widget build(BuildContext context) {
    return Container(
      padding: EdgeInsets.all(16.0),
      child: Text('Welcome, $name!'),
    );
  }
}
```

### Stateful Widget 예시:

```dart
class CounterWidget extends StatefulWidget {
  const CounterWidget({Key? key}) : super(key: key);
  
  @override
  _CounterWidgetState createState() => _CounterWidgetState();
}

class _CounterWidgetState extends State<CounterWidget> {
  int _counter = 0;
  
  void _incrementCounter() {
    setState(() {
      _counter++;
    });
  }
  
  @override
  Widget build(BuildContext context) {
    return Column(
      children: [
        Text('Count: $_counter'),
        ElevatedButton(
          onPressed: _incrementCounter,
          child: Text('Increment'),
        ),
      ],
    );
  }
}
```

## 위젯 기반 UI의 장점

1. **일관된 개발 패러다임**: 모든 UI 요소가 위젯이므로 학습과 개발이 일관됩니다.

2. **컴포지션**: 작은 위젯들을 조합하여 복잡한 UI를 구성할 수 있습니다.

3. **재사용성**: 위젯을 쉽게 재사용하여 코드 중복을 줄일 수 있습니다.

4. **테스트 용이성**: 위젯 단위로 테스트할 수 있어 테스트가 용이합니다.

5. **선언적 UI**: UI를 선언적으로 정의하여 가독성과 유지보수성이 향상됩니다.

Flutter의 위젯 기반 UI는 이러한 접근 방식으로 개발자가 직관적이고 효율적으로 앱을 구축할 수 있게 해줍니다.
