Третья лаба будет посвящена Наивному Байесовскому классификатору. Собственно в аттаче находится архив, в котором датасет уже разбит на 10 частей для кросс-валидации. Задача состоит в классификации спама. Спам сообщения содержат в своем названии spmsg, нормальные сообщения содержат legit. Сам текст письма состоит из двух частей: темы и тела письма. Все слова заменены на инты, соответствующие их индексу в некотором глобальном словаре (своего рода анонимизация). Соответственно от вас требуется построить наивный Байесовский классификатор и при этом:

1) Придумать, либо протестировать, что можно делать с темой и телом письма для улучшения качества работы.
2) Как учитывать (или не учитывать) слова, которые могут встретиться в обучающей выборке, но могут не встретится в тестовой или наоборот.
3) Как наложить дополнительные ограничения на ваш классификатор так, чтобы хорошие письма практически никогда не попадали в спам, но при этом, возможно, общее качество классификации несколько уменьшилось.
4) Понимать как устроен классификатор внутри и уметь отвечать на какие-никакие вопросы по теории с ним связанной.

Для написания классификатора не разрешается использовать библиотеки, наподобие weka и sklearn, а также реализации из них. Кросс-валидацию можно производить любыми средствами.