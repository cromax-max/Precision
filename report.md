# Отчёт о тестировании Precision

## Краткое описание

13 июля 2021 - 13 июля 2021 было проведено Функциональное тестирование приложения Precision.

На тестирование затрачено: 00:20 чч

В результате тестирования выявлены следующие дефекты:
* Итоговая сумма бонуса некорректна
  https://github.com/cromax-max/Precision/issues/1#issue-942992224


## Описание процесса тестирования

В качестве тестовых данных использовались данные:
```java
public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
  }
}
```

Тестирование производилось в следующем окружении:
* Windows10(64-bit)
* Java SE 11
* IntelliJ IDEA