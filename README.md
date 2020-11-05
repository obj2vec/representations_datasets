# external_models

В этом репозитории должны находиться векторные представления. Всё остальное должно быть в других репозиториях.

Векторные представления можно использовать двояко.

1. Их качество мы можем оценивать в лаборатории качества и затем сравнивать с качеством других представлений.

2. Некоторые из таких представлений могут стать основой золотого стандарта.

Представления делятся на слежующие типы по учету контекста и предварительному расчету.

1. У объекта одно представление (контекстно-независимые представления). Это представление один раз рассчитывается и хранится как данные. Контекстно-независимые представления (функция от одного аргумента, объекта):
- Google word2vec
- Microsoft GLOVE
- EVE [http://mlg.ucd.ie/eve/]
- iPavlov
- fastText

2. У объекта одно или более представлений, каждое из которых однозначно определяется по контексту (контекстно-зависимые представления). Но этих представлений для конкретного объекта фиксированный набор, эти представления один раз рассчитываются. (Как выбирать вариант из нескольких предопределенных представлений?) (Такие на практике бывают?)

3. Представление объекта в каждом контексте вычисляется. Обычно это процедура, которая применяется к тексту для получения представлений каждого объекта в тексте, т. е. это настроенная модель. Контекстно-зависимые (функция от двух аргументов, объекта и контекста):
- AdaGram [http://proceedings.mlr.press/v51/bartunov16.pdf]
- Elmo [https://github.com/ltgoslo/simple_elmo]
- Bert [http://files.deeppavlov.ai/deeppavlov_data/bert/rubert_cased_L-12_H-768_A-12_v1.tar.gz]

Часть представлений можно скачать с https://rusvectores.org/ru/models/

Также было бы очень здорово получить у Анны Потапенко тематические представления для Википедии. (Они контекстно-независимые?)
