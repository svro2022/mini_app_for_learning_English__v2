# Mini app for learning English (loops_lists) <br>

> **app.py** - файл запуска программы <br>

---

## Описание
Дорабатываем нашу программу, которая по очереди задает вопросы и предлагает вписать пропущенное слово. <br> 

---

## Реализация
**Часть 1. Простая**

В этом задании мы дорабатываем приложение из прошлого урока.

Создайте два списка  с вопросами и ответами.

```python
questions = ["My name ___  Vova", "I ___ a coder", "I live ___ Moscow"]
answers = ["is", "am", "in"]
```

**Как работает готовая программа?**

---

Сперва программа здоровается и предлагает начать:

`Привет! Предлагаю проверить свои знания английского! Наберите "ready", чтобы начать!`

Если пользователь набрал `"ready"` — программа начинает задавать вопросы.

Если нет – программа завершается с сообщением:

`Кажется, вы не хотите играть. Очень жаль`.

---

Когда первый вопрос задан, приложение ждет ввод пользователя.

Если ответ правильный, приложение говорит: `Ответ верный!`

Если нет, говорит: 

`Неправильно. Правильный ответ: ______`

Затем приложение задает следующий вопрос.

После ответа на  все вопросы приложение говорит:

`Вот и все! Вы ответили на ___ вопросов из ___ верно, это ____ процентов.`

<aside>
💡 Кстати, если вы поменяете количество вопросов, приложение всё еще должно верно считать статистику!

</aside>

**Часть 2. Задание со звездочкой**

Решайте это задание, только если у вас достаточно времени и вы справились со всеми остальными задачами!

Давайте доработаем логику вашего приложения.

Теперь, если ответ правильный, приложение говорит: `Ответ верный!`

Если ответ неверный, приложение говорит: `Осталось попыток: 2, попробуйте еще раз!`

Если ответ опять неверный, говорит: `Осталось попыток: 1, попробуйте еще раз!`

Если еще раз вводится неправильный ответ, то приложение говорит: 

`Увы, но нет. Верный ответ: ____________`

За каждый ответ начисляются баллы.

Если с первой попытки введен правильный ответ — 3 балла, со второй — 2, с третьей — 1. После ответа на все вопросы приложение говорит:

`Вот и все! Вы ответили на ___ вопросов из ___ верно, вы набрали ___ баллов.`

**Подсказки:**

Создайте отдельную переменную для подсчета баллов.

Внутри цикла по вопросам создайте еще один цикл — по попыткам.

Придумайте, как считать количество баллов за попытку, исходя из номера попытки.