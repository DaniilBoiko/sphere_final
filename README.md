# sphere_final
Финальный проект на Техносфере

![](https://static.wikia.nocookie.net/meme/images/9/92/No_God_Please_No.gif/revision/latest/scale-to-width-down/480?cb=20200923075339)

## scraping
Здесь мы решаем две задачи:
1. Обкачать все страницы, чтобы по меньшей мере понять существуют они или нет, как много там содержимого, а в идеале в будущем использовать для генерации новых фичей,
2. Обкачать поисковые системы (получилось только с гуглом) и посмотреть есть ли наши страницы в топе поисковой выдачи

## processing_click_data
Обрабатываем данные о пользовательских сессиях для того, чтобы получить поведенческие фичи. Все операции разделены на получение данных об отдельных страницах, запросах, по которым они находятся и их доменах

## processing_text_data
Здесь делаем USE-qa-multiplingual ембеддинги для текстов запросов и документов, а также проводим лемматизацию текстов

## did_not_work
Просто лежат идеи того, что можно было бы сделать, но не успел или не получилось. Больше всего конечно же хотелось кластеризовать ембеддинги, чтобы использовать id кластера как фичу, но за адекватное время скластеризоваться оно не смогло.

## prepare_data_and_train.ipynb
Наконец, объединение всего, добавление новых фичей и получение предиктов ансамблем из YetiRankPairwise, StchocaticRank и LambdaRank

## submissions
Отдельно отправленные файлы и файлы обученных моделей
