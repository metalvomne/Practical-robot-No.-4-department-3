# Користувач вводить список
elements = input("Введіть елементи списку через пробіл: ").split()

# Виводимо початковий список
print("Початковий список:", elements)

# Елемент, перед яким треба вставити новий
target = input("Введіть елемент, перед яким потрібно вставити новий: ")

# Новий елемент, який потрібно вставити
new_element = input("Введіть новий елемент для вставки: ")

# Перевіряємо, чи існує target у списку
if target in elements:
    index = elements.index(target)
    elements.insert(index, new_element)
    print("Оновлений список:", elements)
else:
    print(f"Елемент '{target}' не знайдено у списку.")
