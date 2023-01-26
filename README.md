# IU1-22B Java course (GUI application development)
## Hometask 1

Реализуйте класс **Vehicle**, который будет моделировать транспортные средства.
Сделайте, так чтобы можно было задать тип транспортного средства, его среднюю скорость,
расход на 100км. Реализуйте методы, которые помогут вычислить: сколько времени уйдет на преодоление заданной дистанции и метод, который
рассчитает необходимое количество топлива на преодоление дистанции.
Протестируйте корректность работы данных методов.

```java
public class Vehicle {

}
```

1. Дописать код нескольких функций в файлах:
- Function1.java
- Function2.java

### Fucntion1
```java
public class Function1 {
    public static void main(String[] args) {
        System.out.println("Function testing:");
        System.out.printf("Test 1 %s.\n", ClassForTest
                .compareResults(findMax(new int[]{3, 4, 10, -1}), 10) ? "passed" : "failed");

        try {
            findMax(new int[0]);
            System.out.println("Test 2: failed.");
        } catch (RuntimeException e) {
            System.out.println("Test 2: passed.");
        }
    }

    // реализовать функцию, которая будет находить максимум в массиве
    // обработать случай, когда длина массива равна нулю
    // в этом случае выбрасывать исключение
    private static int findMax(int[] arr) {
        return 1;
    }
}
```

Function2
```java
public class Function2 {
    public static void main(String[] args) {
        int[] a = new int[]{1, 2, 3, 4, 5};
        int[] b = new int[]{-5, -6, -7};
        // test 1
        System.out.printf("Test 1 %s.\n", ClassForTest.compareResults(merge(a, b), new int[]{-7, -6, -5, 1, 2, 3, 4, 5}) ? "passed" : "failed");

        //test 2
        System.out.printf("Test 2 %s.\n", ClassForTest.compareResults(merge(new int[0], new int[0]), new int[]{}) ? "passed" : "failed");

        //test 3
        System.out.printf("Test 3 %s.\n", ClassForTest.compareResults(merge(b, a), new int[]{5, 4, 3, 2, 1, -5, -6, -7}) ? "passed" : "failed");

    }

    /*
    методу передаются два упорядоченных массива(могут быть упорядочены по-разному), реализуйте функцию,
    которая объединит их и вернет упорядоченный массив с порядком таким же как и a
     */
    private static int[] merge(int[] a, int[] b) {
        return new int[]{1};
    }
}
```

### Выдача: 28 February, 2022
### Дедлайн: 7 Marth, 2022 (1 week)
