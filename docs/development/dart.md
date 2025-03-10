# Dart 언어 개요

Dart는 Google이 개발한 클라이언트 최적화 프로그래밍 언어로, Flutter 프레임워크의 공식 언어입니다. 주요 특징은 다음과 같습니다:

## 주요 특징

1. **객체 지향 언어**: 모든 것이 객체이며, 클래스와 인터페이스 기반 상속을 지원합니다.

2. **정적 타입 지정**: 변수 타입을 명시적으로 선언할 수 있지만, 타입 추론도 지원하여 코드를 간결하게 작성할 수 있습니다.

3. **널 안전성(Null Safety)**: Dart 2.12부터 도입된 기능으로, 널 참조 오류를 컴파일 시점에 감지할 수 있습니다.

4. **비동기 프로그래밍**: async/await 구문과 Future를 사용한 비동기 프로그래밍을 지원합니다.

5. **JIT와 AOT 컴파일**: 개발 중에는 Just-In-Time(JIT) 컴파일로 빠른 개발 경험을, 배포 시에는 Ahead-Of-Time(AOT) 컴파일로 높은 성능을 제공합니다.

## 기본 문법

### 변수 선언

```dart
// 타입 추론
var name = 'John'; 

// 타입 명시
String lastName = 'Doe';

// 상수
final age = 30;
const PI = 3.14;

// 널 안전성
String? nullableString = null;
String nonNullableString = 'Hello';
```

### 함수

```dart
// 기본 함수
int add(int a, int b) {
  return a + b;
}

// 화살표 함수(람다)
int multiply(int a, int b) => a * b;

// 선택적 매개변수
void greet(String name, {String? greeting}) {
  print('${greeting ?? 'Hello'}, $name!');
}
```

### 클래스와 객체

```dart
class Person {
  // 인스턴스 변수
  String name;
  int age;
  
  // 생성자
  Person(this.name, this.age);
  
  // 명명된 생성자
  Person.guest() : name = 'Guest', age = 18;
  
  // 메서드
  void sayHello() {
    print('Hello, my name is $name and I am $age years old.');
  }
}

// 사용법
void main() {
  var person = Person('John', 30);
  person.sayHello();
  
  var guest = Person.guest();
  guest.sayHello();
}
```

### 컬렉션

```dart
// 리스트
var numbers = [1, 2, 3, 4, 5];
List<String> names = ['John', 'Jane', 'Bob'];

// 맵
var person = {
  'name': 'John',
  'age': 30,
  'isEmployed': true
};
Map<String, dynamic> data = {'key': 'value'};

// 세트
var uniqueNumbers = {1, 2, 3, 4, 5};
Set<String> uniqueNames = {'John', 'Jane', 'Bob'};
```

### 비동기 프로그래밍

```dart
Future<String> fetchData() async {
  // 비동기 작업 시뮬레이션
  await Future.delayed(Duration(seconds: 2));
  return 'Data loaded';
}

void main() async {
  print('Loading data...');
  String result = await fetchData();
  print(result);
}
```

Dart는 Flutter와 함께 사용하기 위해 최적화되었지만, 서버 측 애플리케이션 개발에도 사용할 수 있습니다. 문법이 Java, JavaScript와 유사하여 이러한 언어에 익숙한 개발자라면 쉽게 배울 수 있습니다.
