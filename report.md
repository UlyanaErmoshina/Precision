## Отчёт о тестировании приложения для бонусной системы
### Краткое описание

4.05.2020 было проведено функциональное тестирование приложения для бонусной системы, в результате которого был выявлен дефект.

### Описание тестов

В ходе работы было проведено позитивное, функциональное тестирование.
Цель тестирования: проверка функции начисления бонусов
Описание тестирования:

Название: проверка функции начисления бонусов
Описание: Проверка функции начисления бонусов при введении валидных данных. Пример валидных данных: 0.3, 0.6

Шаги:
1. Открыть IntelliJ IDEA 2020.1.1
2. Вести код
public class Main {
    public static void main(String[] args) {
        double regularBonus = 0.3;
        double specialBonus = 0.6;
        double totalBonus = regularBonus + specialBonus;
        System.out.println(totalBonus);
    }
}
3. Запустить приложение
4. Ожидаемый результат: 0.9
5. Фактический результат: 
0.8999999999999999


### Результаты
В результате тестирования выявлен следующий дефект:

[Неверное итоговое значение бонусов](https://github.com/UlyanaErmoshina/Precision/issues/2)



Тестирование производилось в следующем окружении:
* Windows 10, x64
* IntelliJ IDEA 2020.1.1
