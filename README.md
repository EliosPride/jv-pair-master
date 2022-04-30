# jv-pair

Реализуйте generic-класс **Pair**, содержащий пару элементов разных типов и не запрещающий элементам принимать значение null.

Реализуйте методы **getFirst()**, **getSecond()**, **equals()** и **hashCode()**, а также статический фабричный метод **of()**. Конструктор должен быть закрытым (private).

С корректно реализованным классом Pair должен компилироваться и успешно работать следующий код:

```java
Pair<Integer, String> pair = Pair.of(1, "hello");
Integer i = pair.getFirst(); // 1
String s = pair.getSecond(); // "hello"

Pair<Integer, String> pair2 = Pair.of(1, "hello");
boolean mustBeTrue = pair.equals(pair2); // true!
boolean mustAlsoBeTrue = pair.hashCode() == pair2.hashCode(); // true!
```