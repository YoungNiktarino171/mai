## ФИО, Группа
Иванов Никита Антонович, М8О-308Б-17

## Алгоритмы
Тут я решил взять чисто определения с интернета, чуть-чуть лишь "отсебятины":
1. "Случайный лес" — алгоритм машинного обучения, предложенный Лео Брейманом и Адель Катлер, заключающийся в использовании комитета (ансамбля) решающих деревьев. Случайный лес, как и следует из его названия, состоит из большого количества отдельных деревьев решений, которые работают как ансамбль методов. Каждое дерево в случайном лесу возвращает прогноз класса, и класс с наибольшим количеством голосов становится прогнозом леса.
2. KNN. Для классификации каждого из объектов тестовой выборки необходимо последовательно выполнить несколько операций. Вычислить расстояние до каждого из объектов обучающей выборки. Затем отобрать k объектов обучающей выборки, расстояние до которых минимально. В итоге получаем класс классифицируемого объекта — это класс, наиболее часто встречающийся среди k ближайших соседей.
3. Решающее дерево — это объединение логических правил вида "Значение признака a меньше x И Значение признака b меньше y… => Класс 1" в структуру данных "Дерево"
4. Логистическая регрессия — это статистическая модель, используемая для прогнозирования вероятности возникновения некоторого события путём его сравнения с логистической кривой.

##  Результаты

Ну в выводе я уж постараюсь. Первым делом хотел бы извиниться за то, что я сказал, что во второй лабораторной я использовал plotly. Честно сказать, я думал что да... Но у меня этот модуль работал, там графики кривые были, не красивые. Все равно же красивенько вышло:) Я честное слово разобрался!!!

Чуть не забыл сказать насчет выбранной мною метркии. Я советовался с другом, он сказал, что так как данные не очень хорошо сбалансированны, лучше всего использовать f1-меру.

Теперь хотелось бы пояснить за каждый алгоритм:

1. Честно говоря я не ожидал такой "подставы" от него... Он отработал хуже всех... Мне кажется это связано с тем, что нету параллельного исполнения. Ибо почему целых 11 секунд?)
2. KNN такой же результат как и алгоритма из Sklearn, дать жучть быстрее. Тут вообще без понятия с чем это связано. Хотя 4 мс вообще хоть кто-то заметит?) Мне кажется +- 5 мс не ощутимо. А вот 10... думаю уже "жоска"...
3. Вот тут, то самое "ощутимое". Хоть и такой же результат как у алгоритма из Sklearn, однако "мой" алгоритм в 31 раз медленне!!! Вроде это всего милисекунда, но звучит страшно, если не мс...
4. Логистическая регрессия - худший результат. Однако по времени не самое худшее место. Тут больше ничего не могу сказать, так как устал... Простите...