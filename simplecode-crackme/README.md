# crackmes-solutions

# Решение CrackMe "Simple Code"
https://crackmes.one/crackme/66a64ff190c4c2830c8212da 

## Информация
- **Платформа**: Windows PE32
- **Защита**: Проверка ключа через SHA256
- **Сложность**: Легкая

## Анализ
1. Программа генерирует случайный ключ при запуске.
2. Сохраняет его в переменных окружения `key` и `key2`.
3. Сравнивает ввод пользователя с этим ключом.

## Решение
1. **Статический анализ**:
   - Через de4dot "очищается" сам exe-файл
   - Переносим в dnspy и ищем функцию отвечающую за создание кода
   - Найдена функция `Retrieve_Key()`
   - После неё мы прописываем скрипт который будет выводить нам сгенерированый ключ
   - ![изображение](https://github.com/user-attachments/assets/81c638f3-8570-4c7b-b9eb-e1c9b694adb8)
   - Сам скрипт: Console.WriteLine("Key: " + Environment.GetEnvironmentVariable("key"));
   - ![изображение](https://github.com/user-attachments/assets/3841fd83-01f4-4c6c-923c-d3dfce96b803)
   - Задача решена

       
   
