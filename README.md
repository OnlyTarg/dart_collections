# 📝 Домашнє завдання: Колекції в Dart

## 📁 Налаштування проєкту

1. Створи окремий проєкт із назвою `dart_collections_journey` за допомогою команди:

   ```bash
   dart create dart_collections_journey
   ```

   або за допомогою середовища **VS Code** чи **Android Studio**.

2. Ініціалізуй Git та зроби перший коміт:

   ```bash
   git init
   git add .
   git commit -m "feat: initial commit"
   ```

3. Створи віддалений репозиторій (наприклад, на GitHub) та синхронізуй зміни:

   ```bash
   git remote add origin <your-repo-url>
   git push -u origin main
   ```

4. Створи окрему гілку `feat-DART-08-homework` і виконуй домашнє завдання у ній:

   ```bash
   git checkout -b feat-DART-08-homework
   ```

5. Домашнє завдання виконуй у файлі `lib/main.dart`.

6. Після завершення **кожного завдання** (усього три) роби окремий коміт і пуш до гілки:

   ```bash
   git add .
   git commit -m "feat: complete Task 1"
   git push
   ```

## 🧠 Структура виконання

- Кожне завдання реалізуй в окремому методі:  
  `runTask1()`, `runTask2()`, `runTask3()`

- Виклич усі методи з методу `main`.

- Для зручності, можеш розділити завдання виводом тексту:

   ```dart
   print('---------------------------------------- Task 1 ----------------------------------------');
   ```

---

## ✅ Task 1 — Lists

1. Створи список `numbers` зі 100 елементів.  
   Кожен елемент — випадкове число від 0 до 100.  
   _(Можна використати `Random().nextInt(101)`)_.

2. Виведи список на екран.

3. Виведи 65-й елемент списку у форматі:  
   `"65-й елемент: 42"`

4. Встав число `1000000000` на 50-ту позицію списку.

5. Видали зі списку елементи зі значеннями: `24`, `45`, `66`, `88`.

6. За допомогою циклу `for`:
   - порахуй суму всіх елементів, що діляться на 3 без залишку;
   - виведи цю суму.

7. Створи порожній список `temp`. За допомогою `for-in`:
   - додай до нього всі елементи `numbers`, що діляться на 2.

8. Виведи довжину списку `temp`.

---

## 🔁 Task 2 — Sets

1. Створи файл `names.dart`.

2. У ньому створи дві змінні:

   ```dart
   List<String> ukrainianNames1 = [...];
   List<String> ukrainianNames2 = [...];
   ```

   - Список `ukrainianNames1` згенеруй за допомогою **ChatGPT**.
   - Список `ukrainianNames2` — за допомогою **DeepSeek**.

3. У файлі `main.dart`:

   - Створи `Set uniqueNames1` з `ukrainianNames1`
   - Створи `Set uniqueNames2` з `ukrainianNames2`
   - Створи `Set` з іменами, які є в обох множинах (перетин)  
     → виведи кількість імен
   - Створи `Set` з іменами, які є в `uniqueNames1`, але **не в** `uniqueNames2`  
     → виведи список
   - Створи `Set` з іменами, які є в `uniqueNames2`, але **не в** `uniqueNames1`  
     → виведи список

---

## 🗺️ Task 3 — Maps

1. Додай у `pubspec.yaml` залежність:

   ```yaml
   dependencies:
     word_generator: ^2.0.0
   ```

2. Створи список `nounsList` з 50 випадкових іменників, використовуючи функціонал пакета.  
   Дивись приклад у документації:  
   [https://pub.dev/packages/word_generator#randomnouns](https://pub.dev/packages/word_generator#randomnouns)

3. Із `nounsList` створи `Map<String, int> nounsMap`, де:
   - ключ — слово;
   - значення — довжина цього слова.

4. Створи нову мапу `tempNouns` та:
   - додай у неї лише ті слова з `nounsMap`, довжина яких **парна**.

5. Виведи всі **ключі** з `tempNouns`.

---

✅ Успіхів у виконанні!