# Проверка знаний Markdown

## 1. Математические Формулы

Квадратичное уравнение имеет вид:

$$
ax^2 + bx + c = 0
$$

Дискриминант вычисляется по формуле:

$$
D = b^2 - 4ac
$$

Корни уравнения:

$$
x_{1,2} = \frac{-b \pm \sqrt{D}}{2a}
$$

## 2. Сложные Таблицы

| Имя студента       | Возраст | Курс | Средний балл | Статус       |
|-------------------|--------:|:----:|:------------:|:------------:|
| Иванов Иван       | 20      | 2    | 4.8          | ✅ Активен   |
| Петрова Мария     | 19      | 1    | 5.0          | ✅ Активен   |
| Сидоров Алексей   | 22      | 3    | 3.9          | ⚠️ Академический отпуск |
| Кузнецова Анна    | 21      | 2    | 4.5          | ✅ Активен   |
| Васильев Дмитрий  | 23      | 4    | 4.2          | ❌ Отчислен  |

## 3. Галерея Изображений

![Горный пейзаж](https://images.unsplash.com/photo-1506744038136-46273834b3fb?w=300&h=200&fit=crop)
![Лесное озеро](https://images.unsplash.com/photo-1475924156734-496f6cac6ec1?w=300&h=200&fit=crop)
![Океанский закат](https://images.unsplash.com/photo-1473496169904-658ba7c44d8a?w=300&h=200&fit=crop)

## 4. Вложенные Списки

### Список покупок:

- **Овощи и фрукты**
  - 🥕 Морковь - 1 кг
  - 🥔 Картофель - 2 кг
  - 🍎 Яблоки - 1.5 кг
  - 🍅 Помидоры - 0.5 кг

- **Молочные продукты**
  - 🥛 Молоко - 2 л
  - 🧀 Сыр - 300 г
  - 🍶 Йогурт - 4 шт.
  - 🧈 Сливочное масло - 200 г

- **Бакалея**
  - 🍚 Рис - 1 кг
  - 🍝 Макароны - 2 упаковки
  - 🫒 Оливковое масло - 1 бутылка
  - ☕ Кофе - 250 г

## 5. Подсветка Синтаксиса

### Python код:

```python
def calculate_quadratic_roots(a, b, c):
    """
    Вычисляет корни квадратного уравнения ax² + bx + c = 0
    """
    import math
    
    # Вычисляем дискриминант
    discriminant = b**2 - 4*a*c
    
    if discriminant > 0:
        # Два действительных корня
        root1 = (-b + math.sqrt(discriminant)) / (2*a)
        root2 = (-b - math.sqrt(discriminant)) / (2*a)
        return root1, root2
    elif discriminant == 0:
        # Один действительный корень
        root = -b / (2*a)
        return root,
    else:
        # Комплексные корни
        real_part = -b / (2*a)
        imaginary_part = math.sqrt(-discriminant) / (2*a)
        return complex(real_part, imaginary_part), complex(real_part, -imaginary_part)

# Пример использования
roots = calculate_quadratic_roots(1, -3, 2)
print(f"Корни уравнения: {roots}")
// Функция для вычисления корней квадратного уравнения
function solveQuadraticEquation(a, b, c) {
    // Вычисляем дискриминант
    const discriminant = b * b - 4 * a * c;
    
    if (discriminant > 0) {
        // Два действительных корня
        const root1 = (-b + Math.sqrt(discriminant)) / (2 * a);
        const root2 = (-b - Math.sqrt(discriminant)) / (2 * a);
        return [root1, root2];
    } else if (discriminant === 0) {
        // Один действительный корень
        const root = -b / (2 * a);
        return [root];
    } else {
        // Комплексные корни
        const realPart = -b / (2 * a);
        const imaginaryPart = Math.sqrt(-discriminant) / (2 * a);
        return [
            { real: realPart, imaginary: imaginaryPart },
            { real: realPart, imaginary: -imaginaryPart }
        ];
    }
}

// Пример использования
const solutions = solveQuadraticEquation(1, -5, 6);
console.log('Решения уравнения:', solutions);
