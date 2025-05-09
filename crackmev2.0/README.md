# crackmes-solutions

# Решение CrackMe "Simple Code"
https://crackmes.one/crackme/6793a6eb73b486c1ed429e84

## Информация
- **Платформа**: Windows PE32
- **Защита**: Пароль
- **Сложность**: Легкая

## Анализ


## Решение
1. **Статический анализ**:
   - Через de4dot "очищается" сам exe-файл
   - Переносим в dnspy и ищем проверку ввода пароля
   - Нашли закодированное число
   ![изображение](https://github.com/user-attachments/assets/593587ff-d8c6-411b-8ecb-f97cd3ae8f88)
   - Текст "MjAwNQ==" закодирован в формате Base64
   - Расшифровываем его и получаем число 2005
   - Ищем дальше!
   - Нашли опять закодированные буквы в ASCII формате
   - ![изображение](https://github.com/user-attachments/assets/25b8edb5-de20-49d8-8da8-ae4ae7aababc)
   - Расшифровавываем 67  → 'C' 82  → 'R' 65  → 'A'  67  → 'C' 75  → 'K' 77  → 'M' 69  → 'E'
   - Получилось слово CRACKME
   - Нашли опять закодированные буквы
   - ![изображение](https://github.com/user-attachments/assets/cd400782-edb9-4e87-9d64-b9ef910f162b)
   - Расшифровываем потому же принципу что и слово CRACKME и получаем HAIBALLAD
   - У нас получилось HAIBALLAD-2005-CRACKME
   - Проверяем!
   ![изображение](https://github.com/user-attachments/assets/5de90c1f-4865-4594-adcf-f8f2bf646f92)
   ![изображение](https://github.com/user-attachments/assets/9d3022f8-384d-4a60-b733-3c287136415d)
   -Да и всё верно в итоге


   
